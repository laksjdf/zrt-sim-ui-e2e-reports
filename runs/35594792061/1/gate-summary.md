# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：108
- 通过：96
- 失败：10
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle decode 提交、算子结果与配置恢复 | 16.568 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 decode 提交、算子结果与配置恢复 | 14.847 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 prefill 提交、算子结果与配置恢复 | 14.900 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.552 |
| skipped | `l0/home.spec.ts` | @L0 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l0/home.spec.ts` | @L0 真实后端接受首页浏览器采集批次 | 0.000 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 30.868 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 5.391 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 29.658 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 30.363 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 共用量化 | 3.358 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 2.154 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 2.227 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 3.099 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.755 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 2.787 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 2.851 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 3.304 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 5.539 |
| passed | `l1/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.831 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 2.082 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.936 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 2.073 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 2.236 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 2.039 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 2.127 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 2.122 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.516 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 4.835 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.987 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 4.783 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 4.882 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 4.833 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 5.504 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.951 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 3.877 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 4.024 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 4.457 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 11.126 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.978 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.850 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 128.653 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 3.005 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 2.850 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 2.321 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 2.553 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 24.857 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 24.694 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 4.230 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 4.290 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 2.038 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 2.008 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 6.109 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 6.158 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 6.318 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 6.168 |
| failed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 8.030 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 2.576 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 2.307 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 20.371 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 2.370 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 2.621 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 2.488 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 2.453 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 90.219 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 38.878 |
| failed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 18.827 |
| passed | `l1/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.891 |
| passed | `l1/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 2.051 |
| passed | `l1/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.873 |
| passed | `l1/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 2.085 |
| failed | `l1/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 2.806 |
| passed | `l1/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 2.299 |
| passed | `l1/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.977 |
| passed | `l1/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 2.642 |
| passed | `l1/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 2.027 |
| passed | `l1/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 1.987 |
| failed | `l1/operations-insights.spec.ts` | @L1 多部门必须选择，409回首页，403撤回全部数据 | 7.005 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 2.249 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 2.100 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 2.289 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.886 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.649 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.759 |
| passed | `l1/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 3.460 |
| passed | `l1/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 2.946 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 5.152 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.754 |
| failed | `l1/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 2.014 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.991 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.840 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.772 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.660 |
| failed | `l1/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 7.136 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 13.550 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 41.826 |
| failed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 15.752 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 2.067 |
| failed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 17.117 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 39.063 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 14.100 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 85.536 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 23.772 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.116 |
| failed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 17.257 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 18.585 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 29.909 |
| failed | `l1/user-calibration.spec.ts` | @L1 PostgreSQL 用户手工校准UI闭环与训练数值应用 | 7.090 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：1395
- Warning：2

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | POST | `/api/jobs/26-1/result-viewed` | 202 | 522.0 | @L1 训练hardware真实任务进度与结果 |
| warning | POST | `/api/user/decrypt` | 200 | 515.0 | @L1 重跑、终止、单删和批删 |

