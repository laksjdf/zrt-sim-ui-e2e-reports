# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：50
- 通过：47
- 失败：3
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.113 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 7.034 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 3.107 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 26.396 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 24.107 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.685 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.811 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.453 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.192 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.428 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.130 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 1.433 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.327 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.306 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.294 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.871 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.638 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.153 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.563 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.055 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 1.982 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 287.729 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 1.957 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 1.723 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.577 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 1.761 |
| failed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 17.099 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 7.856 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 10.367 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 1.558 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 1.410 |
| failed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 264.332 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.408 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.462 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.343 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.361 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 57.912 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 27.920 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 7.363 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.942 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 0.968 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 2.581 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.062 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 10.388 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 24.065 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 7.474 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 64.305 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 12.571 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 7.528 |
| failed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 16.364 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：622
- Warning：0

> 未发现超过阈值的浏览器 API 请求。

