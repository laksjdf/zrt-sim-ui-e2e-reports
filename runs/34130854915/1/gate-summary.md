# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：39
- 通过：35
- 失败：4
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.135 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 7.096 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 2.839 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 24.329 |
| failed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 6.451 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.758 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.860 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.636 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.499 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.407 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.168 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.480 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 268.502 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 1.719 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 1.615 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.372 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 1.384 |
| failed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 17.084 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 7.729 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 7.326 |
| failed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 264.097 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.383 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.460 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.327 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.236 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 47.619 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 27.752 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 11.697 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.913 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 0.932 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 2.589 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 0.959 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 8.799 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 24.399 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 7.489 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 63.543 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 12.596 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 7.513 |
| failed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 16.486 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：541
- Warning：0

> 未发现超过阈值的浏览器 API 请求。

