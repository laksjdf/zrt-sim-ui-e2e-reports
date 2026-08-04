# Browser E2E Gate

- 结论：**PASS**
- Playwright 退出码：`0`
- 总数：23
- 通过：23
- 失败：0
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 11.965 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 7.604 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 5.013 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 33.281 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 25.594 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 11.287 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 8.004 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 7.950 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 71.064 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 11.927 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 102.028 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 80.904 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 40.874 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 10.960 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 9.402 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 3.171 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 27.485 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 73.357 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 8.995 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 14.223 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 8.906 |
| passed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 34.918 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 15.394 |
