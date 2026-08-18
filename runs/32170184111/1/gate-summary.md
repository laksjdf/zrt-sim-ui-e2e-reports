# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：31
- 通过：30
- 失败：1
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 8.006 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 1.553 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 7.662 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 1.756 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 28.194 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 23.521 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.102 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.114 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 10.031 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 1.590 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 1.670 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.376 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 259.335 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 7.893 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 6.359 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 59.047 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 18.408 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 17.973 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 7.452 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.604 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 0.667 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 1.574 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 0.603 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 10.054 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 29.586 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 7.258 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 7.682 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 8.429 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.405 |
| failed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 743.545 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 8.318 |
