# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：26
- 通过：24
- 失败：2
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 12.879 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 8.116 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 5.276 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 34.383 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 27.835 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册且不可见 API Docs | 5.509 |
| failed | `l0/user-manual-navigation.spec.ts` | @L0 管理员可见 API Docs | 8.631 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 11.024 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 8.139 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 8.448 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 541.538 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 10.609 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 15.043 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 304.620 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 161.339 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 80.931 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 15.387 |
| failed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 9.868 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 3.289 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 27.239 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 82.950 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 280.866 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 15.761 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.307 |
| passed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 42.155 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 12.454 |
