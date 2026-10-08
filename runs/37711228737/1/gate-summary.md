# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：156
- 通过：149
- 失败：5
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle decode 提交、算子结果与配置恢复 | 12.154 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 decode 提交、算子结果与配置恢复 | 10.249 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 prefill 提交、算子结果与配置恢复 | 13.211 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 2.397 |
| skipped | `l0/home.spec.ts` | @L0 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l0/home.spec.ts` | @L0 真实后端接受首页浏览器采集批次 | 0.000 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 13.177 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 3.020 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 25.632 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 27.892 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 共用量化 | 2.261 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 1.282 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 1.375 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.650 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.896 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 1.585 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 1.649 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 2.491 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.332 |
| passed | `l1/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.086 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.257 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.254 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.228 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 1.423 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.189 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.232 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.203 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.582 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.487 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.221 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 3.819 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 3.775 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 3.669 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 3.998 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.086 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 3.134 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 2.998 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 3.244 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.569 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.111 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.129 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 217.768 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.037 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 1.852 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.611 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 1.684 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.131 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.174 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 2.622 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 2.621 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 1.073 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.067 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.298 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 5.312 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 5.347 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 5.343 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 10.170 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 1.532 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 1.450 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 12.808 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.388 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.566 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.402 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.414 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 99.737 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 48.153 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 14.202 |
| passed | `l1/operations-insights.spec.ts` | @L1 详细看板P95复用一位小数格式和未知状态 | 1.270 |
| passed | `l1/operations-insights.spec.ts` | @L1 行为筛选不支持时不给全量表格并解释恢复路径 | 1.286 |
| passed | `l1/operations-insights.spec.ts` | @L1 用户行为口径显示可理解类别且不冒充真实登录 | 1.192 |
| passed | `l1/operations-insights.spec.ts` | @L1 下钻 MCP/API 标签和错误码继承筛选 | 1.387 |
| passed | `l1/operations-insights.spec.ts` | @L1 下钻任务到执行逐层返回保留父主题 | 1.381 |
| passed | `l1/operations-insights.spec.ts` | @L1 下钻用户会话返回后保留用户选择 | 1.304 |
| passed | `l1/operations-insights.spec.ts` | @L1 个人会话权限撤销后不继续展示观测内容 | 1.225 |
| passed | `l1/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 0.921 |
| passed | `l1/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.252 |
| passed | `l1/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.045 |
| passed | `l1/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 1.239 |
| passed | `l1/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 3.378 |
| passed | `l1/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 1.360 |
| passed | `l1/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.148 |
| passed | `l1/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 1.784 |
| passed | `l1/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.133 |
| passed | `l1/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 1.358 |
| passed | `l1/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 1.333 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 1.344 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 1.170 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 1.411 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.206 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.955 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.035 |
| passed | `l1/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 1.907 |
| passed | `l1/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 1.467 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 2.661 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.077 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.084 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.126 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.151 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.155 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.064 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 1.124 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 1.155 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 0.905 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 9.662 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 27.522 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 13.692 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 1.169 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 19.639 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 28.716 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 13.632 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 67.423 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 14.396 |
| passed | `l1/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 45.174 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 8.407 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 8.873 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 17.641 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 18.449 |
| passed | `l1/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 7.695 |
| passed | `l1/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 13.440 |
| passed | `l1/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 13.427 |
| passed | `l1/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 9.910 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 0.965 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.052 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 1.121 |
| passed | `l1/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 8.581 |
| passed | `l1/user-calibration.spec.ts` | @L1 手工校准和规则预览的算子候选随阶段筛选 | 1.417 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准优先顺序可调整保存且预览命中首个同级版本 | 1.409 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 1.298 |
| passed | `l1/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 1.709 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 1.173 |
| passed | `l1/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 1.215 |
| passed | `l1/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 1.309 |
| passed | `l1/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 1.253 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.288 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选提交、刷新恢复与精确报告 | 13.629 |
| passed | `l1/user-calibration.spec.ts` | @L1 单条Profiling无源任务构建仅精确Shape候选 | 9.992 |
| passed | `l1/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 1.567 |
| passed | `l1/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 1.917 |
| passed | `l1/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 1.657 |
| passed | `l1/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 7.701 |
| passed | `l1/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 31.019 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 3.248 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 3.309 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 3.301 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 3.196 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 3.216 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 4.114 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 2.020 |
| passed | `l1/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 2.306 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 1.136 |
| passed | `l1/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 1.475 |
| passed | `l1/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 1.304 |
| passed | `l1/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 1.419 |
| passed | `l1/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 4.317 |
| passed | `l1/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 14.153 |
| passed | `l1/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 22.216 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：3017
- Warning：0

> 未发现超过阈值的浏览器 API 请求。

