# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：59
- 通过：50
- 失败：9
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 7.037 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 12.685 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 4.760 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 28.428 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 28.702 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 隔离 | 3.404 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 1.975 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 2.056 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 2.691 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.702 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 5.255 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.729 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.885 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.660 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 2.037 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.835 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.851 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.745 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 3.951 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 3.959 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.886 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.163 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.818 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.729 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 138.151 |
| failed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 17.430 |
| failed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 17.310 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 2.263 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 2.235 |
| failed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 17.529 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 8.437 |
| failed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 16.900 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 2.254 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 1.985 |
| failed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 344.926 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 2.072 |
| failed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 7.083 |
| failed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 7.160 |
| failed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 7.217 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 68.610 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 28.361 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 8.097 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.505 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.574 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 4.604 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.601 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 10.526 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 36.474 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 14.012 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 1.719 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 17.673 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 38.688 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 8.080 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 73.954 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 13.647 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 10.221 |
| failed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 17.106 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 28.421 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 29.585 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：728
- Warning：4

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | POST | `/api/user/decrypt` | 200 | 581.0 | @L0 训练模型评估从浏览器提交到报告和任务历史 |
| warning | POST | `/api/user/decrypt` | 200 | 581.0 | @L1 任务筛选、详情和历史 Run |
| warning | POST | `/api/user/decrypt` | 200 | 535.0 | @L1 新增算子失败显示错误并保持弹窗打开 |
| warning | POST | `/api/user/decrypt` | 200 | 501.0 | @L0 首页与核心入口可达 |

