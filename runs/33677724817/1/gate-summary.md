# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：31
- 通过：29
- 失败：2
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 5.281 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 12.264 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 4.672 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 26.477 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 25.380 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 2.719 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.471 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 5.143 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.067 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 4.069 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.776 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.171 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 218.246 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 8.566 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 8.336 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 7.464 |
| failed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 279.990 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 58.641 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 38.537 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 12.529 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.553 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.662 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 4.814 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.597 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 10.145 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 30.299 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 8.262 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 10.977 |
| failed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 7.362 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 8.178 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 9.265 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：462
- Warning：4

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | POST | `/api/user/decrypt` | 200 | 600.0 | @L1 推理任务提交用户新增的通信中间层 |
| warning | POST | `/api/user/decrypt` | 200 | 591.0 | @L1 训练多硬件性能对比 |
| warning | POST | `/api/user/decrypt` | 200 | 569.0 | @L1 批量训练实验服务闭环 |
| warning | POST | `/api/user/decrypt` | 200 | 539.0 | @L0 首页与核心入口可达 |

