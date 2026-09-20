# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：106
- 通过：87
- 失败：17
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle decode 提交、算子结果与配置恢复 | 14.788 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 decode 提交、算子结果与配置恢复 | 11.449 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 prefill 提交、算子结果与配置恢复 | 11.632 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.412 |
| skipped | `l0/home.spec.ts` | @L0 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l0/home.spec.ts` | @L0 真实后端接受首页浏览器采集批次 | 0.000 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 13.952 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 5.253 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 34.175 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 30.111 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 共用量化 | 3.422 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 1.925 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 2.056 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 2.813 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.535 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 2.452 |
| failed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 17.692 |
| failed | `l1/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 2.145 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 5.678 |
| passed | `l1/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.807 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 2.120 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 2.178 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.914 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 2.319 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 2.047 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.918 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 2.119 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.507 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 4.057 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.780 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 4.467 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 4.705 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 4.804 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 5.270 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.955 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 3.924 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 3.960 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 4.682 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.233 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.931 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.741 |
| failed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 17.133 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.920 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 2.889 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 2.407 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 2.512 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.899 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.693 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 4.361 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 4.045 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 1.960 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.985 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 6.192 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 5.948 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 6.025 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 6.126 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 10.648 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 2.585 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 2.212 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 20.090 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 2.289 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 2.407 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.981 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 2.129 |
| failed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 736.911 |
| failed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 737.220 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 9.592 |
| passed | `l1/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.823 |
| passed | `l1/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.889 |
| passed | `l1/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.717 |
| passed | `l1/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 1.967 |
| passed | `l1/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 2.571 |
| passed | `l1/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 2.005 |
| passed | `l1/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.818 |
| passed | `l1/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 2.450 |
| passed | `l1/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.848 |
| passed | `l1/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 2.093 |
| failed | `l1/operations-insights.spec.ts` | @L1 多部门必须选择，409回首页，403撤回全部数据 | 17.277 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 2.286 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 2.076 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 2.121 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 2.130 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.631 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.739 |
| passed | `l1/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 2.961 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 5.004 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.890 |
| failed | `l1/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.948 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.778 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.810 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.766 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.837 |
| failed | `l1/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 7.083 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 17.512 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 41.869 |
| failed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 15.734 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 1.937 |
| failed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 17.079 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 39.030 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 14.366 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 82.431 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 23.720 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.064 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 9.925 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 19.337 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 19.893 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：1334
- Warning：8

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | GET | `/api/resource-quotas/me` | 200 | 10672.0 | @L0 首页与核心入口可达 |
| warning | GET | `/api/resource-quotas/me` | 200 | 10662.0 | @L0 推理对比复用统一阶段并独立复制配置 |
| warning | GET | `/api/settings` | 200 | 10649.0 | @L0 首页与核心入口可达 |
| warning | GET | `/api/observability/access` | 403 | 10649.0 | @L0 首页与核心入口可达 |
| warning | GET | `/api/assets/models?domain=train` | 200 | 10649.0 | @L0 首页与核心入口可达 |
| warning | GET | `/api/assets/hardwares?domain=train&owner=pw_0_1789892832907` | 200 | 10649.0 | @L0 首页与核心入口可达 |
| warning | POST | `/api/user/decrypt` | 200 | 527.0 | @L0 eagle3 prefill 提交、算子结果与配置恢复 |
| warning | POST | `/api/jobs/26-1/result-viewed` | 202 | 512.0 | @L1 训练hardware真实任务进度与结果 |

