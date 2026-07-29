# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：23
- 通过：14
- 失败：5
- 跳过：4

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 10.000 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 7.286 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 4.645 |
| failed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 21.176 |
| failed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 19.811 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 11.274 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 7.798 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 7.975 |
| skipped | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 0.000 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 9.549 |
| skipped | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 0.000 |
| skipped | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 0.000 |
| skipped | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 0.000 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 11.040 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 9.390 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 3.042 |
| failed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 19.125 |
| failed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 19.563 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 13.557 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 10.941 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.916 |
| passed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 34.065 |
| failed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 19.285 |
