# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：195
- 通过：188
- 失败：5
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/inference/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 15.723 |
| passed | `l0/shell/home.spec.ts` | @L0 首页与核心入口可达 | 9.352 |
| passed | `l0/shell/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 5.228 |
| passed | `l0/shell/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 3.354 |
| passed | `l0/training/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 30.489 |
| passed | `l0/training/training-operator.spec.ts` | @L0 训练算子性能评估 | 9.211 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 infer两层硬件文件导入后编辑与保存保持有效规格 | 2.540 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train两层硬件文件导入后编辑与保存保持有效规格 | 2.272 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 新建硬件仅提供四种拓扑，Clos 选择可往返 YAML | 2.372 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 双场景硬件芯片型号在表单与高级YAML及保存间同步 | 2.161 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 infer旧硬件未配置芯片型号可保存及重新编辑 | 2.399 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train旧硬件未配置芯片型号可保存及重新编辑 | 2.307 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train,infer旧硬件未配置芯片型号可保存及重新编辑 | 2.505 |
| passed | `l1/assets/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.934 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 2.775 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 3.295 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 3.380 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 6.810 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 模型初始化完成前不可输入且加载后保存名称不丢失 | 4.936 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.923 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 2.177 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 2.145 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 2.130 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 2.252 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 2.089 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 2.111 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 2.105 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.413 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 5.051 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 2.241 |
| passed | `l1/assets/table-search.spec.ts` | @L1 model-management 跨页搜索、表头联合筛选和清空恢复 | 2.624 |
| passed | `l1/assets/table-search.spec.ts` | @L1 hardware-management 跨页搜索、表头联合筛选和清空恢复 | 2.325 |
| passed | `l1/assets/table-search.spec.ts` | @L1 operator-management 跨页搜索、表头联合筛选和清空恢复 | 2.410 |
| passed | `l1/assets/table-search.spec.ts` | @L1 module-management 跨页搜索、表头联合筛选和清空恢复 | 2.395 |
| passed | `l1/calibration/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 8.736 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 14.293 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 14.266 |
| passed | `l1/calibration/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 11.657 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 1.757 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.821 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 2.036 |
| passed | `l1/calibration/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 9.464 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手工校准和规则预览的算子候选随阶段筛选 | 2.432 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准优先顺序可调整保存且预览命中首个同级版本 | 2.446 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 2.096 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 2.351 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 1.817 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 1.957 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 2.188 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 1.942 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.980 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling受控构建中刷新恢复保持运行身份 | 4.182 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选完成后刷新恢复与精确报告 | 16.478 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 单条Profiling无源任务构建仅精确Shape候选 | 10.912 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 2.307 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 2.743 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 2.431 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 8.605 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 33.217 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 9.287 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 14.836 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 8.768 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 17.135 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 17.600 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 5.986 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 2.906 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 3.217 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 1.910 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 2.372 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 2.041 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 2.466 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 6.285 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 15.003 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 29.607 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 统一阶段联动、单独覆盖和 P/D 共用量化 | 3.452 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 推理对比复用统一阶段并独立复制配置 | 2.129 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 批量 P/D 预检发送实际阶段精度而非界面草稿 | 2.246 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle decode 提交、算子结果与配置恢复 | 11.853 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 decode 提交、算子结果与配置恢复 | 12.014 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 prefill 提交、算子结果与配置恢复 | 11.955 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 4.807 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 4.939 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 4.748 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 5.365 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.984 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 3.811 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 3.979 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 4.696 |
| passed | `l1/inference/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.498 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.992 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.991 |
| passed | `l1/inference/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 78.556 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.857 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 2.942 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 2.556 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 2.668 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 CP 能力延迟返回不覆盖任务恢复中的并行配置 | 2.351 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 缺少跨 P 能力字段时保留 CP 控件并明确禁用跨 P 传输 | 2.461 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 能力请求失败时 CP 与跨 P 均给出失败提示 | 2.321 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 Diffusion 的序列并行仍受模型图 CP 能力约束 | 2.402 |
| passed | `l1/inference/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.898 |
| passed | `l1/inference/inference-diffusion-pipeline-api.spec.ts` | @L1 MiniMax-H3 PP2 真实任务返回两个 stage 并展示去噪结果 | 9.972 |
| passed | `l1/inference/inference-diffusion-pipeline.spec.ts` | @L1 Diffusion PP3 恢复后可编辑并提交，组件候选不跨 stage | 2.782 |
| passed | `l1/inference/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.855 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 4.372 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 4.125 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 2.037 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.992 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.964 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 6.128 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 5.978 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 6.077 |
| passed | `l1/inference/inference-operator.spec.ts` | @L1 推理算子性能评估 | 13.696 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 2.576 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 2.274 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 121.461 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 2.259 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 2.678 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 2.431 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 2.377 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 80.191 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比显存不足时无可行解 | 18.978 |
| passed | `l1/inference/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 19.457 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 首次进入等待慢解密和慢管理员角色查询，不提前请求 access | 5.352 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 普通用户首次进入不请求 access，不产生观测接口403 | 1.900 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 真实后端管理员首次进入 access 成功，且角色查询先完成 | 1.798 |
| passed | `l1/shell/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.723 |
| passed | `l1/shell/release-info.spec.ts` | @L1 管理员版本信息 › 编辑版本信息并恢复 | 1.865 |
| failed | `l1/shell/theme.spec.ts` | @L1 共享主题默认浅色、持久化、跨标签页与键盘切换 | 6.243 |
| failed | `l1/shell/theme.spec.ts` | @L1 推理主题切换保持模型、负载、量化与硬件编辑流程 | 5.752 |
| failed | `l1/shell/theme.spec.ts` | @L1 训练/资产/图表共用主题且切换不提交请求 | 5.698 |
| failed | `l1/shell/theme.spec.ts` | @L1 独立模型编辑页和移动端复用主题入口 | 5.630 |
| failed | `l1/shell/theme.spec.ts` | @L1 深色统计图打印使用浅色画布且结束后恢复原偏好 | 5.715 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 详细看板P95复用一位小数格式和未知状态 | 2.110 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 行为筛选不支持时不给全量表格并解释恢复路径 | 2.189 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 用户行为口径显示可理解类别且不冒充真实登录 | 2.077 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻 MCP/API 标签和错误码继承筛选 | 2.166 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻任务到执行逐层返回保留父主题 | 2.324 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻用户会话返回后保留用户选择 | 2.292 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 个人会话权限撤销后不继续展示观测内容 | 2.097 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.646 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 2.152 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.918 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 2.303 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 3.977 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 2.331 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 2.066 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 2.690 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.851 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 2.126 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 2.318 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 2.307 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 2.031 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 2.208 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 2.049 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.975 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.773 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 2.038 |
| passed | `l1/statistics/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.891 |
| passed | `l1/tasks/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 3.635 |
| passed | `l1/tasks/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 2.833 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.999 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.907 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 1.777 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 1.816 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 1.822 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 11.890 |
| passed | `l1/tasks/task-lifecycle.spec.ts` | @L1 重跑、单删和批删 | 42.762 |
| passed | `l1/tasks/task-table-search.spec.ts` | @L1 任务联合搜索防抖请求、分页与清空 | 4.390 |
| passed | `l1/tasks/task-table-search.spec.ts` | @L1 任务重置回到第一页并丢弃旧条件的延迟响应 | 3.009 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 16.621 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 2.043 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 进度帧与持久化结果 | 24.113 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 进度帧与持久化结果 | 30.122 |
| passed | `l1/training/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 14.365 |
| passed | `l1/training/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 26.461 |
| passed | `l1/training/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 16.216 |
| passed | `l1/training/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 46.288 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 1440px | 2.131 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 1440px | 1.947 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 1440px | 2.118 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 390px | 1.911 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 390px | 2.092 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 390px | 2.095 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 1440px | 2.105 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 1440px | 1.914 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 1440px | 2.070 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 390px | 1.985 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 390px | 1.867 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 390px | 2.056 |
| passed | `l1/training/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 12.134 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 19.276 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 20.123 |
| skipped | `l2/shell/observability.spec.ts` | @L2 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l2/shell/observability.spec.ts` | @L2 真实后端接受首页浏览器采集批次 | 0.000 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：3678
- Warning：4

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | GET | `/api/calibrations/versions/297b0f46ad1f4f8a8830b08fb2d7b29e` | 200 | 8624.0 | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 |
| warning | GET | `/api/tasks?status=succeeded&exclude_internal=true&page=1&page_size=10` | 200 | 845.0 | @L1 任务重置回到第一页并丢弃旧条件的延迟响应 |
| warning | POST | `/api/jobs/62-1/result-viewed` | 202 | 530.0 | @L1 训练hardware真实任务进度与结果 |
| warning | GET | `/api/jobs/44-1` | 200 | 527.0 | @L1 推理策略寻优与应用策略 |

