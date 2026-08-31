# Browser E2E Gate

- 结论：**PASS**
- Playwright 退出码：`0`
- 总数：31
- 通过：31
- 失败：0
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.157 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 6.902 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 2.924 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 24.409 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 23.811 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.591 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.851 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.485 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.304 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.236 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.137 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.551 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 167.678 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 7.694 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 7.658 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 9.604 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 339.733 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 48.046 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 27.963 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 7.151 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.880 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 0.950 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 2.532 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 0.943 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 8.791 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 24.590 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 7.545 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 10.794 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 12.639 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.508 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 8.376 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：468
- Warning：0

> 未发现超过阈值的浏览器 API 请求。

