# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：31
- 通过：28
- 失败：3
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 5.787 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 7.976 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 5.422 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 27.446 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 27.788 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 3.178 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.831 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 5.956 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.552 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 4.753 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.993 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.350 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 260.115 |
| failed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 17.772 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 8.484 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 8.610 |
| failed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 325.158 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 68.659 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 28.512 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 12.800 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.749 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.789 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 5.122 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.811 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 12.885 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 33.844 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 8.426 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 13.432 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 14.241 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 8.515 |
| failed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 17.173 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：468
- Warning：3

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | POST | `/api/user/decrypt` | 200 | 556.0 | @L1 硬件资产 CRUD 与内置保护 |
| warning | POST | `/api/user/decrypt` | 200 | 513.0 | @L0 首页与核心入口可达 |
| warning | POST | `/api/user/decrypt` | 200 | 512.0 | @L1 重跑、终止、单删和批删 |

