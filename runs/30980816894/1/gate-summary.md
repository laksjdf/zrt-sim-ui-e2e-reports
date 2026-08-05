# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：23
- 通过：22
- 失败：1
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 13.276 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 9.602 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 5.647 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 26.864 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 23.921 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 10.736 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 8.231 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 9.508 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 120.933 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 9.317 |
| failed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 37.649 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 81.570 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 41.135 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 11.543 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 9.407 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 3.639 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 24.209 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 79.737 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 260.199 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 16.523 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 10.080 |
| passed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 36.748 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 13.286 |
