# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：172
- 通过：164
- 失败：6
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/inference/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 10.848 |
| passed | `l0/shell/home.spec.ts` | @L0 首页与核心入口可达 | 4.533 |
| passed | `l0/shell/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 2.887 |
| passed | `l0/shell/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.679 |
| passed | `l0/training/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 28.858 |
| passed | `l0/training/training-operator.spec.ts` | @L0 训练算子性能评估 | 8.355 |
| passed | `l1/assets/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.900 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 1.647 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 1.678 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 2.523 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.887 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 模型初始化完成前不可输入且加载后保存名称不丢失 | 2.629 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.067 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.277 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.269 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.225 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 1.405 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.194 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.203 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.223 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.472 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.527 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.224 |
| passed | `l1/calibration/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 7.645 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 13.484 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 13.496 |
| passed | `l1/calibration/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 9.903 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 0.991 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.085 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 1.155 |
| passed | `l1/calibration/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 8.688 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手工校准和规则预览的算子候选随阶段筛选 | 1.444 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准优先顺序可调整保存且预览命中首个同级版本 | 1.406 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 1.346 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 1.551 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 1.140 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 1.143 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 1.408 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 1.131 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.161 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选提交、刷新恢复与精确报告 | 11.868 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 单条Profiling无源任务构建仅精确Shape候选 | 7.643 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 1.414 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 1.829 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 1.620 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 0.117 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 33.556 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 8.018 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 16.170 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 7.929 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 16.152 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 14.229 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 4.035 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 1.925 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 2.231 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 1.134 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 1.512 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 1.135 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 1.434 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 4.451 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 13.986 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 24.036 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 统一阶段联动、单独覆盖和 P/D 共用量化 | 2.325 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 推理对比复用统一阶段并独立复制配置 | 1.291 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 批量 P/D 预检发送实际阶段精度而非界面草稿 | 1.312 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle decode 提交、算子结果与配置恢复 | 10.218 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 decode 提交、算子结果与配置恢复 | 10.145 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 prefill 提交、算子结果与配置恢复 | 10.192 |
| failed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 16.622 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 3.596 |
| failed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 16.593 |
| failed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 16.518 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.065 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 3.054 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 3.136 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 3.736 |
| passed | `l1/inference/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.559 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.129 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.111 |
| passed | `l1/inference/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 77.736 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.002 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 1.954 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.595 |
| failed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 16.644 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 CP 能力延迟返回不覆盖任务恢复中的并行配置 | 1.501 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 Diffusion 的序列并行仍受模型图 CP 能力约束 | 1.526 |
| passed | `l1/inference/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.151 |
| passed | `l1/inference/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.240 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 2.530 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 2.575 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 1.077 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.045 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.296 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 5.361 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 5.313 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 5.327 |
| passed | `l1/inference/inference-operator.spec.ts` | @L1 推理算子性能评估 | 10.106 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 1.529 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 1.452 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 60.112 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.395 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.582 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.431 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.423 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 79.446 |
| failed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比显存不足时无可行解 | 10.813 |
| passed | `l1/inference/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 14.213 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 首次进入等待慢解密和慢管理员角色查询，不提前请求 access | 4.442 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 普通用户首次进入不请求 access，不产生观测接口403 | 1.018 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 真实后端管理员首次进入 access 成功，且角色查询先完成 | 0.905 |
| passed | `l1/shell/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.010 |
| passed | `l1/shell/release-info.spec.ts` | @L1 管理员版本信息 › 编辑版本信息并恢复 | 1.029 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 详细看板P95复用一位小数格式和未知状态 | 1.185 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 行为筛选不支持时不给全量表格并解释恢复路径 | 1.290 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 用户行为口径显示可理解类别且不冒充真实登录 | 1.232 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻 MCP/API 标签和错误码继承筛选 | 1.366 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻任务到执行逐层返回保留父主题 | 1.320 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻用户会话返回后保留用户选择 | 1.268 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 个人会话权限撤销后不继续展示观测内容 | 1.237 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 0.825 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.256 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.069 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 1.351 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 3.319 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 1.302 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.114 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 1.770 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.133 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 1.328 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 1.323 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 1.389 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 1.101 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 1.313 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.196 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.043 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.031 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.109 |
| passed | `l1/statistics/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.112 |
| passed | `l1/tasks/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 1.943 |
| passed | `l1/tasks/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 1.601 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.159 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.028 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 1.116 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 1.147 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 0.903 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 10.011 |
| passed | `l1/tasks/task-lifecycle.spec.ts` | @L1 重跑、单删和批删 | 33.556 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 13.657 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 1.146 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 进度帧与持久化结果 | 16.660 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 进度帧与持久化结果 | 21.954 |
| passed | `l1/training/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 13.636 |
| passed | `l1/training/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 19.350 |
| passed | `l1/training/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 14.462 |
| passed | `l1/training/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 45.162 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 1440px | 1.205 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 1440px | 1.157 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 1440px | 1.166 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 390px | 1.154 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 390px | 1.129 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 390px | 1.179 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 1440px | 1.131 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 1440px | 1.165 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 1440px | 1.136 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 390px | 1.119 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 390px | 1.114 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 390px | 1.130 |
| passed | `l1/training/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 8.990 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 17.643 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 18.451 |
| skipped | `l2/shell/observability.spec.ts` | @L2 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l2/shell/observability.spec.ts` | @L2 真实后端接受首页浏览器采集批次 | 0.000 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：3374
- Warning：1

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | GET | `/api/calibrations/versions/c5ff9cf49f314454ac3cbe55eb1834e1` | 200 | 6258.0 | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 |

