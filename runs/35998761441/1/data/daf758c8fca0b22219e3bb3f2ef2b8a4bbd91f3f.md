# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: l1/user-calibration.spec.ts >> @L1 Profiling迟到打开版本响应不覆盖较新的构建候选
- Location: e2e/specs/l1/user-calibration.spec.ts:304:1

# Error details

```
TimeoutError: locator.click: Timeout 15000ms exceeded.
Call log:
  - waiting for getByTestId('calibration-create-open')

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
      - link "版本信息" [ref=e16] [cursor=pointer]:
        - /url: /zrt-sim/release-notes
      - link "用户管理" [ref=e17] [cursor=pointer]:
        - /url: /zrt-sim/user-manage
      - link "用户手册" [ref=e18] [cursor=pointer]:
        - /url: /zrt-sim/user-manual
      - button "pw_user_10_1790254464925" [ref=e19] [cursor=pointer]:
        - img [ref=e20]
        - generic [ref=e23]: pw_user_10_1790254464925
      - generic [ref=e25]: Idle
  - main [ref=e26]:
    - generic [ref=e28]: ZRT
    - generic [ref=e29]:
      - generic [ref=e30]: ✦ Scenario Hub
      - heading "AI负载建模仿真平台" [level=1] [ref=e31]
      - paragraph [ref=e32]: 选择建模场景，进入对应领域的性能评估、硬件对比与系统寻优工具链。
    - generic [ref=e33]:
      - article [ref=e34]:
        - generic [ref=e35]:
          - generic [ref=e36]:
            - generic [ref=e37]: 🏋️
            - text: TRAIN
          - generic [ref=e38]: 训练
          - paragraph [ref=e39]: 大规模分布式训练性能建模，对比不同并行策略与硬件配置下的训练吞吐与 MFU。
          - generic [ref=e40]:
            - generic [ref=e41]: 性能评估
            - button "算子性能评估 →" [ref=e42] [cursor=pointer]:
              - generic [ref=e43]: 算子性能评估
              - text: →
            - button "模型性能评估 →" [ref=e44] [cursor=pointer]:
              - generic [ref=e45]: 模型性能评估
              - text: →
            - generic [ref=e46]: 多硬件性能对比
            - button "多硬件性能对比 →" [ref=e47] [cursor=pointer]:
              - generic [ref=e48]: 多硬件性能对比
              - text: →
            - generic [ref=e49]: 系统寻优
            - button "模型策略自动寻优 →" [ref=e50] [cursor=pointer]:
              - generic [ref=e51]: 模型策略自动寻优
              - text: →
            - button "批量训练实验 →" [ref=e52] [cursor=pointer]:
              - generic [ref=e53]: 批量训练实验
              - text: →
            - button "硬件寻优 →" [ref=e54] [cursor=pointer]:
              - generic [ref=e55]: 硬件寻优
              - text: →
            - button "硬件配比量化分析 →" [ref=e56] [cursor=pointer]:
              - generic [ref=e57]: 硬件配比量化分析
              - text: →
      - article [ref=e58]:
        - generic [ref=e59]:
          - generic [ref=e60]:
            - generic [ref=e61]: ⚡
            - text: INFER
          - generic [ref=e62]: 推理
          - paragraph [ref=e63]: LLM 推理负载建模，分析 Prefill / Decode 阶段的时延、吞吐与显存占用。
          - generic [ref=e64]:
            - generic [ref=e65]: 性能评估
            - button "算子性能评估 →" [ref=e66] [cursor=pointer]:
              - generic [ref=e67]: 算子性能评估
              - text: →
            - button "模型性能评估 →" [ref=e68] [cursor=pointer]:
              - generic [ref=e69]: 模型性能评估
              - text: →
            - generic [ref=e70]: 多硬件性能对比
            - button "多硬件性能对比 →" [ref=e71] [cursor=pointer]:
              - generic [ref=e72]: 多硬件性能对比
              - text: →
            - generic [ref=e73]: 系统寻优
            - button "模型策略自动寻优 →" [ref=e74] [cursor=pointer]:
              - generic [ref=e75]: 模型策略自动寻优
              - text: →
            - button "批量推理实验 →" [ref=e76] [cursor=pointer]:
              - generic [ref=e77]: 批量推理实验
              - text: →
            - button "PD分离实例配比寻优 →" [ref=e78] [cursor=pointer]:
              - generic [ref=e79]: PD分离实例配比寻优
              - text: →
      - article [ref=e80]:
        - generic [ref=e81]:
          - generic [ref=e82]:
            - generic [ref=e83]: 🎯
            - text: REC
          - generic [ref=e84]: 推荐
          - paragraph [ref=e85]: 推荐系统建模，评估 Embedding、特征交互等算子的计算与通信瓶颈。
          - generic [ref=e86]:
            - generic [ref=e87]: 性能评估
            - button "算子性能评估 →" [ref=e88]:
              - generic [ref=e89]: 算子性能评估
              - text: →
            - button "模型性能评估 →" [ref=e90]:
              - generic [ref=e91]: 模型性能评估
              - text: →
```

# Test source

```ts
  1   | import { test, expect } from '../../fixtures/test'
  2   | import { buildTestUserHeaders } from '../../fixtures/users'
  3   | import { E2E_MULTI_TASK_TIMEOUT_MS } from '../../support/timeouts'
  4   | import { readFileSync } from 'node:fs'
  5   | import { join } from 'node:path'
  6   | import type { Page } from '@playwright/test'
  7   | import type { TestFixtures } from '../../fixtures/test'
  8   | 
  9   | const backend = process.env.E2E_BACKEND_URL
  10  | const profilingFixture = join(process.env.E2E_BACKEND_ROOT || '', 'tests/opcalib/fixtures/MatMulV3.csv')
  11  | 
  12  | async function acceptWorkbenchConfirmation(page: Page) {
  13  |   const confirmation = page.getByRole('dialog', { name: '提示' }).last()
  14  |   await expect(confirmation).toBeVisible()
  15  |   await confirmation.getByRole('button', { name: '继续', exact: true }).click()
  16  | }
  17  | 
  18  | async function prepareCandidateHardware(page: Page, api: TestFixtures['api'], owner: TestFixtures['testOwner']) {
  19  |   if (!backend) throw new Error('E2E_BACKEND_URL is required')
  20  |   const hardware = await api.getTrainHardware()
  21  |   const base = hardware.find(row => row.name === 'H100_Server') as Record<string, unknown> | undefined
  22  |   expect(base).toBeTruthy()
  23  |   const fields = [
  24  |     'borrowed_from', 'chip_name', 'compute', 'device_type', 'ep_overlap_waves',
  25  |     'flash_attention_bwd_coefficient', 'flash_attention_fwd_coefficient',
  26  |     'gpus_per_node', 'host_dma', 'interconnect', 'memory', 'nodes', 'overlap_ratio', 'vendor',
  27  |   ]
  28  |   const name = `Candidate_${owner.account}`
  29  |   const spec = Object.fromEntries(fields.filter(field => base![field] !== undefined)
  30  |     .map(field => [field, base![field]]))
  31  |   const created = await page.request.post(`${backend}/api/assets/hardwares`, {
  32  |     headers: buildTestUserHeaders(owner),
  33  |     data: { name, vendor: base!.vendor, domain: 'train', spec_format: 'json',
  34  |       spec_json: { ...spec, name, label: name } },
  35  |   })
  36  |   expect(created.ok(), await created.text()).toBe(true)
  37  |   return name
  38  | }
  39  | 
  40  | async function prepareCandidateSource(
  41  |   page: Page, api: TestFixtures['api'], catalogs: TestFixtures['catalogs'], owner: TestFixtures['testOwner'],
  42  |   useBuiltin = false,
  43  | ): Promise<{ taskId: number; hardwareName: string }> {
  44  |   if (!backend) throw new Error('E2E_BACKEND_URL is required')
  45  |   const hardwareName = useBuiltin ? catalogs.train.hardwareName : await prepareCandidateHardware(page, api, owner)
  46  |   const models = await api.getTrainModels()
  47  |   const selected = models.find(model => String(model.key || model.id) === catalogs.train.modelId)
  48  |   expect(selected).toBeTruthy()
  49  |   const response = await page.request.get(`${backend}/api/assets/models/${selected!.id}`, {
  50  |     headers: buildTestUserHeaders(owner),
  51  |   })
  52  |   expect(response.ok(), await response.text()).toBe(true)
  53  |   const asset = await response.json()
  54  |   const spec = asset.model_spec_json
  55  |   const modelJson = {
  56  |     ...spec, name: spec.name ?? catalogs.train.modelId,
  57  |     domain: spec.domain ?? 'train', hf_config_json: spec.hf_config_json ?? {},
  58  |   }
  59  |   const devices = catalogs.train.hardwareNodes * catalogs.train.hardwareGpusPerNode
  60  |   const config = `model: {base: "${catalogs.train.modelId}", layers: "[dense]*32", seq_len: 128}
  61  | system: {hw: "${hardwareName}", nodes: ${catalogs.train.hardwareNodes}, gpus_per_node: ${catalogs.train.hardwareGpusPerNode}, host_mem_gb: 2048}
  62  | strategy: {tp: 1, cp: 1, pp: 1, ep: 1, dp: ${devices}, micro_batch: 1, global_batch: ${devices}, pp_schedule: 1f1b, zero_stage: 1, recompute: {per_layer: {dense: [], moe: []}}, optimizer: adam}
  63  | `
  64  |   const submitted = await page.request.post(`${backend}/api/train/estimate`, {
  65  |     headers: buildTestUserHeaders(owner),
  66  |     data: { config_content: config, model_name: catalogs.train.modelId, model_json: modelJson,
  67  |       account: owner.account, username: owner.username },
  68  |   })
  69  |   expect(submitted.status(), await submitted.text()).toBe(202)
  70  |   const job = await submitted.json()
  71  |   await api.waitForJob(String(job.run_id), 'succeeded', E2E_MULTI_TASK_TIMEOUT_MS)
  72  |   return { taskId: Number(job.task_id), hardwareName }
  73  | }
  74  | 
  75  | async function openCandidateDraft(page: Page, catalogs: TestFixtures['catalogs'], hardwareName: string, name: string) {
  76  |   await page.goto('/zrt-sim/calibration')
> 77  |   await page.getByTestId('calibration-create-open').click()
      |                                                     ^ TimeoutError: locator.click: Timeout 15000ms exceeded.
  78  |   await page.getByRole('button', { name: /导入 Profiling/ }).click()
  79  |   await page.getByTestId('calibration-version-name').fill(name)
  80  |   await page.getByTestId('calibration-version-hardware').fill(hardwareName)
  81  |   await page.getByTestId('calibration-version-model').fill(catalogs.train.modelId)
  82  |   await page.getByTestId('calibration-version-phase').fill('train')
  83  |   await page.getByTestId('calibration-profile-file').setInputFiles({
  84  |     name: 'MatMulV3.csv', mimeType: 'text/csv', buffer: readFileSync(profilingFixture),
  85  |   })
  86  |   await expect(page.getByTestId('calibration-version-save')).toHaveClass(/primary-button/)
  87  |   await expect(page.getByTestId('calibration-build-candidate')).not.toHaveClass(/primary-button/)
  88  |   await page.getByTestId('calibration-version-save').click()
  89  |   await page.getByTestId('calibration-nav-versions').click()
  90  |   const row = page.locator('tbody tr').filter({ hasText: name })
  91  |   await expect(row).toContainText('待构建')
  92  |   await row.getByRole('button', { name: '编辑' }).click()
  93  |   await expect(page.getByText('有效 5 / 总 5')).toBeVisible()
  94  |   await expect(page.getByTestId('calibration-build-candidate')).toHaveClass(/primary-button/)
  95  |   await expect(page.getByTestId('calibration-version-save')).not.toHaveClass(/primary-button/)
  96  |   return row
  97  | }
  98  | 
  99  | async function candidateVersionId(page: Page, owner: TestFixtures['testOwner'], name: string): Promise<string> {
  100 |   if (!backend) throw new Error('E2E_BACKEND_URL is required')
  101 |   const response = await page.request.get(`${backend}/api/calibrations/versions`, {
  102 |     headers: buildTestUserHeaders(owner),
  103 |   })
  104 |   expect(response.ok(), await response.text()).toBe(true)
  105 |   const version = (await response.json()).items.find((item: { name: string }) => item.name === name)
  106 |   expect(version).toBeTruthy()
  107 |   return version.id
  108 | }
  109 | 
  110 | async function holdFirstVersionRead(page: Page, versionId: string) {
  111 |   let release: (() => void) | undefined
  112 |   let reached: (() => void) | undefined
  113 |   let first = true
  114 |   const held = new Promise<void>(resolve => { reached = resolve })
  115 |   await page.route(`**/api/calibrations/versions/${versionId}`, async route => {
  116 |     if (route.request().method() !== 'GET' || !first) return route.continue()
  117 |     first = false
  118 |     const response = await route.fetch()
  119 |     await new Promise<void>(resolve => { release = resolve; reached?.() })
  120 |     await route.fulfill({ response })
  121 |   })
  122 |   return { held, release: () => release?.() }
  123 | }
  124 | 
  125 | test('@L1 Profiling构建候选提交、刷新恢复与诊断报告', async ({ page, api, catalogs, testOwner }) => {
  126 |   test.setTimeout(E2E_MULTI_TASK_TIMEOUT_MS)
  127 |   // 内置 H100 路径验证快照与资产别名元数据的真实端到端对照。
  128 |   expect(catalogs.train.hardwareName).toBe('H100_Server')
  129 |   const { taskId: sourceTaskId, hardwareName } = await prepareCandidateSource(page, api, catalogs, testOwner, true)
  130 |   const row = await openCandidateDraft(page, catalogs, hardwareName, `Profiling构建-${Date.now()}`)
  131 |   await page.getByTestId('calibration-source-task-id').fill('0')
  132 |   await page.getByTestId('calibration-build-candidate').click()
  133 |   await expect(page.getByTestId('calibration-build-error')).toContainText('正整数')
  134 |   await page.getByTestId('calibration-source-task-id').fill(String(sourceTaskId))
  135 |   await page.keyboard.press('Tab')
  136 |   await expect(page.getByTestId('calibration-build-candidate')).toBeFocused()
  137 |   const submitted = page.waitForResponse(response => response.request().method() === 'POST'
  138 |     && response.url().includes('/build-candidate'))
  139 |   await page.getByTestId('calibration-build-candidate').click()
  140 |   const buildResponse = await submitted
  141 |   expect(buildResponse.status(), await buildResponse.text()).toBe(202)
  142 |   const build = await buildResponse.json()
  143 |   await expect(page.getByTestId('calibration-build-progress')).toContainText(/排队|运行/)
  144 |   await page.reload()
  145 |   await page.getByTestId('calibration-nav-versions').click()
  146 |   await expect(row).toContainText('构建中')
  147 |   await row.locator('td').first().getByRole('button').click()
  148 |   await expect(page.getByTestId('calibration-build-progress')).toBeVisible()
  149 |   await api.waitForJob(String(build.run_id), 'succeeded', E2E_MULTI_TASK_TIMEOUT_MS)
  150 |   const report = page.getByTestId('calibration-build-candidate-report')
  151 |   await expect(report).toContainText('诊断候选，不可发布、不可用于任务', { timeout: 30_000 })
  152 |   await expect(report).toContainText(`来源训练任务 #${sourceTaskId}`)
  153 |   await expect(report).toContainText(build.input_hash)
  154 |   await expect(report).toContainText('样本 5 / 原始 5 行')
  155 |   await expect(report).toContainText('分组 1')
  156 |   await expect(report).toContainText('Shape')
  157 |   const evidence = page.getByTestId('calibration-build-shape-evidence')
  158 |   await expect(evidence).toContainText('精确 Shape / t0 证据')
  159 |   await expect(evidence).toContainText('中位数')
  160 |   await expect(evidence).toContainText('相对误差')
  161 |   await expect(report).toContainText('阻断项')
  162 |   await page.getByRole('button', { name: '取消' }).click()
  163 |   await expect(row.getByRole('button', { name: '发布' })).toHaveCount(0)
  164 | })
  165 | 
  166 | test('@L1 Profiling构建候选期间修改批次使旧运行失效', async ({ page, api, catalogs, testOwner }) => {
  167 |   test.setTimeout(E2E_MULTI_TASK_TIMEOUT_MS)
  168 |   if (!backend) throw new Error('E2E_BACKEND_URL is required')
  169 |   const { taskId: sourceTaskId, hardwareName } = await prepareCandidateSource(page, api, catalogs, testOwner)
  170 |   const versionName = `Profiling失效-${Date.now()}`
  171 |   await openCandidateDraft(page, catalogs, hardwareName, versionName)
  172 |   await page.getByTestId('calibration-source-task-id').fill(String(sourceTaskId))
  173 |   const submitted = page.waitForResponse(response => response.request().method() === 'POST'
  174 |     && response.url().includes('/build-candidate'))
  175 |   await page.getByTestId('calibration-build-candidate').click()
  176 |   const buildResponse = await submitted
  177 |   expect(buildResponse.status(), await buildResponse.text()).toBe(202)
```