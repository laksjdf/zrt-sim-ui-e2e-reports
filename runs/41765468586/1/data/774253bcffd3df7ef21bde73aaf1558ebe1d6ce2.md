# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: l1/calibration/user-calibration.spec.ts >> @L1 重查源任务失败后不沿用旧的兼容性通过状态
- Location: e2e/specs/l1/calibration/user-calibration.spec.ts:715:1

# Error details

```
Error: Navigation bootstrap GET http://127.0.0.1:57415/zrt-sim/src/inference/utils/native-model-edit.ts failed: net::ERR_NETWORK_CHANGED
```

# Page snapshot

```yaml
- generic [ref=e3]:
  - banner [ref=e4]:
    - generic [ref=e5]: ZRT
    - generic [ref=e6]: AI负载建模仿真平台
    - generic [ref=e7]:
      - link "返回主页" [ref=e8] [cursor=pointer]:
        - /url: /zrt-sim/
        - img [ref=e9]
        - generic [ref=e12]: 返回主页
      - link "任务管理" [ref=e13] [cursor=pointer]:
        - /url: /zrt-sim/tasks
      - link "资产管理" [ref=e14] [cursor=pointer]:
        - /url: /zrt-sim/assets
      - link "信息统计" [ref=e15] [cursor=pointer]:
        - /url: /zrt-sim/statistics
      - link "精度校准" [ref=e16] [cursor=pointer]:
        - /url: /zrt-sim/calibration
      - link "版本信息" [ref=e17] [cursor=pointer]:
        - /url: /zrt-sim/release-notes
      - link "用户管理" [ref=e18] [cursor=pointer]:
        - /url: /zrt-sim/user-manage
      - link "用户手册" [ref=e19] [cursor=pointer]:
        - /url: /zrt-sim/user-manual
      - button "切换至深色模式" [ref=e20] [cursor=pointer]:
        - img [ref=e21]
      - button "pw_user_4_1793762256655" [ref=e23] [cursor=pointer]:
        - img [ref=e24]
        - generic [ref=e27]: pw_user_4_1793762256655
      - generic [ref=e29]: Calibration
  - main [ref=e30]:
    - generic [ref=e31]:
      - link "首页" [ref=e32] [cursor=pointer]:
        - /url: /zrt-sim/
      - generic [ref=e33]: /
      - generic [ref=e34]: 精度校准
    - generic [ref=e35]:
      - generic [ref=e36]:
        - generic [ref=e37]:
          - heading "用户精度校准" [level=1] [ref=e38]
          - paragraph [ref=e39]: 管理仅自己可见的手工校准版本与 Profiling 导入批次；未验证数据不会用于任务。
        - button "新建校准版本" [ref=e40] [cursor=pointer]
      - note [ref=e41]:
        - strong [ref=e42]: Profiling 校准
        - generic [ref=e43]: 支持原始 kernel_details.csv 与规范 CSV/ZIP 增量导入；仅正式验证通过的 Profiling 版本可发布并用于后续训练任务。
      - generic [ref=e44]:
        - navigation "校准工作台导航" [ref=e45]:
          - button "总览 资产与能力边界" [ref=e46] [cursor=pointer]:
            - strong [ref=e47]: 总览
            - generic [ref=e48]: 资产与能力边界
          - button "我的校准版本 筛选、修订与启停" [ref=e49] [cursor=pointer]:
            - strong [ref=e50]: 我的校准版本
            - generic [ref=e51]: 筛选、修订与启停
          - button "默认规则与预览 真实规则与命中结果" [ref=e52] [cursor=pointer]:
            - strong [ref=e53]: 默认规则与预览
            - generic [ref=e54]: 真实规则与命中结果
        - main [ref=e55]:
          - status [ref=e56]: 正在加载校准版本…
          - generic [ref=e57]:
            - generic [ref=e58]:
              - generic [ref=e59]:
                - heading "总览" [level=2] [ref=e60]
                - paragraph [ref=e61]: 账户聚合来自数据库，不从当前页推算；启用和自动应用不代表任务已实际命中。
              - button "刷新" [ref=e62] [cursor=pointer]
            - generic [ref=e63]:
              - article [ref=e64]:
                - generic [ref=e65]: 账户版本总数
                - strong [ref=e66]: —
              - article [ref=e67]:
                - generic [ref=e68]: 已启用版本
                - strong [ref=e69]: —
              - article [ref=e70]:
                - generic [ref=e71]: 已启用版本明确覆盖的算子
                - strong [ref=e72]: —
              - article [ref=e73]:
                - generic [ref=e74]: 开启自动应用的规则范围
                - strong [ref=e75]: —
            - article [ref=e76]:
              - generic [ref=e77]:
                - heading "开始一次校准" [level=3] [ref=e78]
                - paragraph [ref=e79]: 选择手工利用率，或导入具体硬件、模型和阶段的实测批次。
              - button "新建校准版本" [ref=e80] [cursor=pointer]
            - article [ref=e81]:
              - strong [ref=e82]: Profiling 可构建并验证
              - paragraph [ref=e83]: 可追加原始或规范 CSV/ZIP、查看 Shape 与 t0 对照；验证通过后再发布和启用。
```

# Test source

```ts
  1  | import type { Page, Request, Response } from '@playwright/test'
  2  | 
  3  | const networkChanged = 'net::ERR_NETWORK_CHANGED'
  4  | 
  5  | function observeNavigation(page: Page) {
  6  |   const state = { origin: '', topLevelGet: false, blocked: false, failure: undefined as Error | undefined }
  7  |   const onRequest = (request: Request) => {
  8  |     if (!['GET', 'HEAD'].includes(request.method())) state.blocked = true
  9  |     if (!request.isNavigationRequest() || request.frame() !== page.mainFrame()) return
  10 |     state.topLevelGet = request.method() === 'GET' && /^https?:/.test(request.url())
  11 |     if (state.topLevelGet) state.origin = new URL(request.url()).origin
  12 |   }
  13 |   const onFailed = (request: Request) => {
  14 |     if (request.frame() !== page.mainFrame()) return
  15 |     if (request.method() !== 'GET'
  16 |       || !['document', 'script', 'stylesheet'].includes(request.resourceType())
  17 |       || new URL(request.url()).origin !== state.origin
  18 |       || request.failure()?.errorText !== networkChanged) {
  19 |       state.blocked = true
  20 |       return
  21 |     }
> 22 |     state.failure = new Error(`Navigation bootstrap GET ${request.url()} failed: ${networkChanged}`)
     |                     ^ Error: Navigation bootstrap GET http://127.0.0.1:57415/zrt-sim/src/inference/utils/native-model-edit.ts failed: net::ERR_NETWORK_CHANGED
  23 |   }
  24 |   const onResponse = (response: Response) => { if (response.status() >= 400) state.blocked = true }
  25 |   const onPageError = () => { state.blocked = true }
  26 |   page.on('request', onRequest)
  27 |   page.on('requestfailed', onFailed)
  28 |   page.on('response', onResponse)
  29 |   page.on('pageerror', onPageError)
  30 |   return { state, detach: () => {
  31 |     page.off('request', onRequest)
  32 |     page.off('requestfailed', onFailed)
  33 |     page.off('response', onResponse)
  34 |     page.off('pageerror', onPageError)
  35 |   } }
  36 | }
  37 | 
  38 | async function navigate(page: Page, goto: Page['goto'], url: string, options: Parameters<Page['goto']>[1]) {
  39 |   for (let attempt = 0; attempt < 2; attempt += 1) {
  40 |     const { state, detach } = observeNavigation(page)
  41 |     let response: Response | null = null
  42 |     let failure: unknown
  43 |     try { response = await goto.call(page, url, options) }
  44 |     catch (error) { failure = error }
  45 |     finally { detach() }
  46 |     // A successful document response can still leave a broken static module graph.
  47 |     if (failure && (!(failure instanceof Error) || !/^page\.goto: net::ERR_NETWORK_CHANGED(?: at |\n|$)/.test(failure.message))) {
  48 |       throw failure
  49 |     }
  50 |     if (!state.failure) {
  51 |       if (failure) throw failure
  52 |       return response
  53 |     }
  54 |     if (attempt === 1 || !state.topLevelGet || state.blocked) throw failure ?? state.failure
  55 |   }
  56 |   throw new Error('Navigation recovery exhausted')
  57 | }
  58 | 
  59 | export function installNavigationRecovery(page: Page): () => void {
  60 |   const original = page.goto
  61 |   page.goto = (url, options) => navigate(page, original, url, options)
  62 |   return () => { page.goto = original }
  63 | }
  64 | 
```