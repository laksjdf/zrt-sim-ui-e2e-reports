# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：26
- 通过：24
- 失败：2
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 11.404 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 8.049 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 5.007 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 29.710 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 22.695 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册且不可见 API Docs | 4.686 |
| failed | `l0/user-manual-navigation.spec.ts` | @L0 管理员可见 API Docs | 8.017 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 10.174 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 7.331 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 7.373 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 420.783 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 10.002 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 11.706 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 233.335 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 130.350 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 60.606 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 14.986 |
| failed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 8.927 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 3.066 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 22.691 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 72.333 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 235.409 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 15.387 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 11.599 |
| passed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 37.553 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 11.949 |
