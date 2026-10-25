# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: l1/operations-access-ready.spec.ts >> @L1 普通用户首次进入不请求 access，不产生观测接口403
- Location: e2e/specs/l1/operations-access-ready.spec.ts:68:1

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByText('未启用或无权限访问')
Expected: visible
Timeout: 5000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 5000ms
  - waiting for getByText('未启用或无权限访问')

```

# Test source

```ts
  1   | import { test, expect, type Page } from '@playwright/test'
  2   | import { observationFixture } from '../../support/operations-fixture'
  3   | 
  4   | function gate() {
  5   |   let release!: () => void
  6   |   const waiting = new Promise<void>(resolve => { release = resolve })
  7   |   return { waiting, release }
  8   | }
  9   | 
  10  | async function browserIdentity(page: Page) {
  11  |   await page.addInitScript(() => {
  12  |     localStorage.setItem('zrt_user_info', JSON.stringify({
  13  |       account: 'encrypted-account', name: 'encrypted-name', l3Dept: 'encrypted-dept',
  14  |     }))
  15  |   })
  16  |   await page.route('**/api/settings', route => route.fulfill({ json: { auth_enabled: true, redirect_url: '' } }))
  17  |   await page.route('**/api/developers/check?*', route => route.fulfill({ json: { is_developer: true } }))
  18  |   await page.route('**/api/observability/events/batch', route => route.fulfill({ status: 202, json: {
  19  |     accepted: 1, dropped: 0, durable: false,
  20  |   } }))
  21  | }
  22  | 
  23  | test('@L1 首次进入等待慢解密和慢管理员角色查询，不提前请求 access', async ({ page }) => {
  24  |   // 原实现缺少角色等待会提前请求 access；真实浏览器头注入也必须使用解密后的身份。
  25  |   await browserIdentity(page)
  26  |   const decrypt = gate(), role = gate(), roleStarted = gate()
  27  |   let accessRequests = 0
  28  |   const forbidden: string[] = []
  29  |   page.on('response', response => {
  30  |     if (response.url().includes('/api/observability/') && response.status() === 403) forbidden.push(response.url())
  31  |   })
  32  |   await page.route('**/api/user/decrypt', async route => {
  33  |     await decrypt.waiting
  34  |     await route.fulfill({ json: { account: 'admin-user', username: 'Admin', l3Dept: 'Research' } })
  35  |   })
  36  |   await page.route('**/api/resource-quotas/me', async route => {
  37  |     expect(route.request().headers()['x-user-account']).toBe('admin-user')
  38  |     roleStarted.release()
  39  |     await role.waiting
  40  |     await route.fulfill({ json: { role: 'admin', max_active_runs: 5, max_search_evaluations: 1024, active_runs: 0 } })
  41  |   })
  42  |   await page.route('**/api/observability/**', route => {
  43  |     if (route.request().url().includes('/events/batch')) {
  44  |       return route.fulfill({ status: 202, json: { accepted: 1, dropped: 0, durable: false } })
  45  |     }
  46  |     if (route.request().url().includes('/access')) {
  47  |       accessRequests += 1
  48  |       expect(route.request().headers()['x-user-account']).toBe('admin-user')
  49  |       return route.fulfill({ json: { enabled: true, allowed: true, authorized_depts: ['Research'], operations: true } })
  50  |     }
  51  |     return route.fulfill({ json: observationFixture() })
  52  |   })
  53  |   try {
  54  |     await page.goto('/zrt-sim/operations-insights')
  55  |     await expect(page.getByText('正在验证访问权限…')).toBeVisible()
  56  |     expect(accessRequests).toBe(0)
  57  |     decrypt.release()
  58  |     await roleStarted.waiting
  59  |     await expect(page.getByText('正在验证访问权限…')).toBeVisible()
  60  |     expect(accessRequests).toBe(0)
  61  |     role.release()
  62  |     await expect(page.getByTestId('metric-runs')).toContainText('24')
  63  |     expect(accessRequests).toBe(1)
  64  |     expect(forbidden).toEqual([])
  65  |   } finally { decrypt.release(); role.release() }
  66  | })
  67  | 
  68  | test('@L1 普通用户首次进入不请求 access，不产生观测接口403', async ({ page }) => {
  69  |   // 普通用户不能为探测入口而请求管理员接口，页面也不能暴露管理员数据。
  70  |   await browserIdentity(page)
  71  |   await page.route('**/api/user/decrypt', route => route.fulfill({ json: {
  72  |     account: 'normal-user', username: 'Normal', l3Dept: 'Research',
  73  |   } }))
  74  |   await page.route('**/api/resource-quotas/me', route => route.fulfill({ json: {
  75  |     role: 'normal', max_active_runs: 5, max_search_evaluations: 1024, active_runs: 0,
  76  |   } }))
  77  |   let observationRequests = 0
  78  |   await page.route('**/api/observability/**', route => {
  79  |     if (!route.request().url().includes('/events/batch')) observationRequests += 1
  80  |     return route.fulfill({ status: 202, json: {} })
  81  |   })
  82  |   await page.goto('/zrt-sim/operations-insights')
> 83  |   await expect(page.getByText('未启用或无权限访问')).toBeVisible()
      |                                             ^ Error: expect(locator).toBeVisible() failed
  84  |   await expect(page.getByTestId('metric-runs')).toHaveCount(0)
  85  |   await expect(page.locator('.hdr-link', { hasText: '产品运行与洞察' })).toHaveCount(0)
  86  |   expect(observationRequests).toBe(0)
  87  | })
  88  | 
  89  | test('@L1 真实后端管理员首次进入 access 成功，且角色查询先完成', async ({ page }) => {
  90  |   // 使用隔离数据库预置的管理员，不 mock 身份、角色或 access 响应。
  91  |   const account = process.env.E2E_ADMIN_ACCOUNT || 'e2e-admin'
  92  |   const responses: Array<{ endpoint: string; status: number }> = []
  93  |   page.on('response', response => {
  94  |     const path = new URL(response.url()).pathname
  95  |     if (path.endsWith('/resource-quotas/me') || path.endsWith('/observability/access')) {
  96  |       responses.push({ endpoint: path.split('/').at(-1)!, status: response.status() })
  97  |     }
  98  |   })
  99  |   const granted = page.waitForResponse(response => new URL(response.url()).pathname.endsWith('/observability/access'))
  100 |   const params = new URLSearchParams({ account, name: 'E2E Admin', l3Dept: 'Research' })
  101 |   await page.goto(`/zrt-sim/operations-insights?${params}`)
  102 |   const response = await granted
  103 |   expect(response.status()).toBe(200)
  104 |   expect(await response.json()).toMatchObject({ enabled: true, allowed: true, operations: true })
  105 |   await expect(page.getByText('未启用或无权限访问')).toHaveCount(0)
  106 |   await expect(page.getByTestId('metric-runs')).toBeVisible()
  107 |   expect(responses).toEqual([{ endpoint: 'me', status: 200 }, { endpoint: 'access', status: 200 }])
  108 | })
  109 | 
```