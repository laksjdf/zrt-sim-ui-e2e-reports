# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: l1/inference-pd-ratio.spec.ts >> @L1 PD 配比无可行解/OOM
- Location: e2e/specs/l1/inference-pd-ratio.spec.ts:44:1

# Error details

```
Error: expect(locator).toBeVisible() failed

Locator: getByTestId('pd-hardware-summary')
Expected: visible
Timeout: 5000ms
Error: element(s) not found

Call log:
  - Expect "toBeVisible" with timeout 5000ms
  - waiting for getByTestId('pd-hardware-summary')

```

```yaml
- banner:
  - text: ZRT AI负载建模仿真平台
  - link "返回主页":
    - /url: /zrt-sim/
    - img
    - text: 返回主页
  - link "任务管理":
    - /url: /zrt-sim/tasks
  - link "资产管理":
    - /url: /zrt-sim/assets
  - link "信息统计":
    - /url: /zrt-sim/statistics
  - link "精度校准":
    - /url: /zrt-sim/calibration
  - link "版本信息":
    - /url: /zrt-sim/release-notes
  - link "用户管理":
    - /url: /zrt-sim/user-manage
  - link "用户手册":
    - /url: /zrt-sim/user-manual
  - button "pw_user_4_1790173142038":
    - img
    - text: pw_user_4_1790173142038
  - text: Idle
- main:
  - link "ZRT":
    - /url: /zrt-sim/
  - text: /
  - link "推理":
    - /url: /zrt-sim/
  - text: / PD分离实例配比寻优
  - heading "PD分离实例配比寻优" [level=1]
  - text: 排队/运行 0 / 10 单次搜索最多 2048 次评估 提交时以服务端实时配额为准
  - navigation:
    - button "✓ 选择模型"
    - button "✓ PD配比寻优负载配置"
    - button "3 选择一个硬件环境"
    - button "4 PD配比寻优结果"
  - main:
    - text: 选择硬件环境 硬件厂商
    - combobox:
      - option "全部厂商" [selected]
      - option "HUAWEI"
      - option "NVIDIA"
    - text: 硬件配置模板
    - combobox
    - text: 选择硬件配置模板
    - img
    - text: 请先选择一个硬件配置模板 PD 分离部署方式 PP 多 P 实例间部署 POD 内部署 P→P 间 KV Cache 复用走 intra_node 或 pod_fabric 跨 POD 部署 P→P 间 KV Cache 复用走 scale_out PD P→D 实例间部署 POD 内部署 P→D 间 KV Cache 复用走 intra_node 或 pod_fabric 跨 POD 部署 P→D 间 KV Cache 传输走 scale_out
    - paragraph:
      - text: 💡 本地命中率根据 P 实例数自动计算，无需手动配置。P 实例数可在
      - strong: 负载配置
      - text: 页面中修改。
    - text: 引擎将按 P/D 侧容量需求自动搜索最优配比与实例数，预计耗时 2~15 秒
  - button "← 上一步"
  - button "PD配比寻优"
```

# Test source

```ts
  1  | import { test, expect } from '../../fixtures/test'
  2  | import { selectOption } from '../../support/select-option'
  3  | import { E2E_TASK_TIMEOUT_MS, E2E_TEST_TIMEOUT_MS } from '../../support/timeouts'
  4  | 
  5  | test('@L1 PD 配比可行结果', async ({ page }) => {
  6  |   test.setTimeout(E2E_TEST_TIMEOUT_MS)
  7  | 
  8  |   await page.goto('/zrt-sim/infer/optimize/pd-ratio')
  9  |   await expect(page.getByRole('heading', {
  10 |     name: /^(PD分离实例配比寻优|LLM 负载建模仿真)$/,
  11 |   })).toBeVisible()
  12 | 
  13 |   // Step 1: 选择第一个可用的模型（若页面已默认选中则直接继续）
  14 |   const modelInput = page.locator('#model-select-name')
  15 |   const current = await modelInput.inputValue().catch(() => '')
  16 |   if (!current) {
  17 |     await modelInput.click()
  18 |     const firstOption = page.locator('.model-name-option').first()
  19 |     await firstOption.click()
  20 |   }
  21 |   await page.getByTestId('infer-step-1-continue').click()
  22 | 
  23 |   // Step 2: PD 配置
  24 |   await expect(page.getByText('PD配比寻优负载配置')).toBeVisible()
  25 |   await page.getByTestId('infer-step-2-continue').click()
  26 | 
  27 |   // Step 3: 页面必须为数据库目录中的首个硬件建立可切换的初始配置。
  28 |   // 这会捕获“空配置时选择器被隐藏，用户无法选择第一条硬件”的回归。
  29 |   const hardwareTemplate = page.getByTestId('pd-hardware-template')
  30 |   const summary = page.getByTestId('pd-hardware-summary')
  31 |   await expect(hardwareTemplate).toBeVisible()
  32 |   await expect(summary).toBeVisible()
  33 |   const initialName = (await summary.locator('strong').textContent())?.trim()
  34 |   await selectOption(hardwareTemplate, { index: 1 })
  35 |   await expect(summary.locator('strong')).not.toHaveText(initialName || '')
  36 |   await page.getByTestId('infer-step-3-run').click()
  37 | 
  38 |   // Step 4 PD 结果
  39 |   await expect(page.getByRole('heading', { name: 'PD 配比寻优结果' })).toBeVisible({ timeout: E2E_TASK_TIMEOUT_MS })
  40 |   await expect(page.locator('.detail-table').filter({ hasText: 'World Size' })).toBeVisible()
  41 |   await expect(page.locator('.oom-warning')).not.toBeVisible()
  42 | })
  43 | 
  44 | test('@L1 PD 配比无可行解/OOM', async ({ page }) => {
  45 |   test.setTimeout(E2E_TEST_TIMEOUT_MS)
  46 | 
  47 |   await page.goto('/zrt-sim/infer/optimize/pd-ratio')
  48 |   await expect(page.getByRole('heading', {
  49 |     name: /^(PD分离实例配比寻优|LLM 负载建模仿真)$/,
  50 |   })).toBeVisible()
  51 | 
  52 |   const modelInput2 = page.locator('#model-select-name')
  53 |   const current2 = await modelInput2.inputValue().catch(() => '')
  54 |   if (!current2) {
  55 |     await modelInput2.click()
  56 |     await page.locator('.model-name-option').first().click()
  57 |   }
  58 |   await page.getByTestId('infer-step-1-continue').click()
  59 | 
  60 |   // 设置极大负载以触发 OOM/无可行解
  61 |   const inputCard = page.locator('.req-card').filter({ hasText: 'Input' })
  62 |   const outputCard = page.locator('.req-card').filter({ hasText: 'Output' })
  63 |   await inputCard.locator('input').fill('65536')
  64 |   await outputCard.locator('input').fill('65536')
  65 |   await page.getByTestId('infer-step-2-continue').click()
  66 | 
  67 |   // OOM 分支也必须先得到可提交的数据库硬件模板，不能因空配置静默停在 Step 3。
  68 |   await expect(page.getByTestId('pd-hardware-template')).toBeVisible()
> 69 |   await expect(page.getByTestId('pd-hardware-summary')).toBeVisible()
     |                                                         ^ Error: expect(locator).toBeVisible() failed
  70 |   await page.getByTestId('infer-step-3-run').click()
  71 | 
  72 |   const result = page.getByRole('heading', { name: 'PD 配比寻优结果' })
  73 |   const oom = page.locator('.oom-warning')
  74 |   const noResult = page.locator('.pd-no-result')
  75 |   await Promise.race([
  76 |     result.waitFor({ state: 'visible', timeout: E2E_TASK_TIMEOUT_MS }),
  77 |     oom.waitFor({ state: 'visible', timeout: E2E_TASK_TIMEOUT_MS }),
  78 |     noResult.waitFor({ state: 'visible', timeout: E2E_TASK_TIMEOUT_MS }),
  79 |   ])
  80 | })
  81 | 
```