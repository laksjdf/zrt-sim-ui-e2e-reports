# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：228
- 通过：214
- 失败：12
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/inference/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 18.953 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 仿真提交立即显示状态，422 原因可见且允许重试 | 1.508 |
| passed | `l0/shell/home.spec.ts` | @L0 首页与核心入口可达 | 2.925 |
| passed | `l0/shell/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 2.175 |
| passed | `l0/shell/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.624 |
| passed | `l0/training/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 29.641 |
| passed | `l0/training/training-operator.spec.ts` | @L0 训练算子性能评估 | 8.228 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 infer两层硬件文件导入后编辑与保存保持有效规格 | 1.205 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train两层硬件文件导入后编辑与保存保持有效规格 | 1.176 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 新建硬件仅提供四种拓扑，Clos 选择可往返 YAML | 1.277 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 双场景硬件芯片型号在表单与高级YAML及保存间同步 | 1.338 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 infer旧硬件未配置芯片型号可保存及重新编辑 | 1.243 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train旧硬件未配置芯片型号可保存及重新编辑 | 1.222 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train,infer旧硬件未配置芯片型号可保存及重新编辑 | 1.295 |
| passed | `l1/assets/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.010 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 1.856 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 1.651 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 2.461 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.080 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 模型初始化完成前不可输入且加载后保存名称不丢失 | 2.468 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 0.990 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.438 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.127 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.092 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 1.323 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.113 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.105 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.089 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 1.983 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.070 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.092 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 模型详情和规模扩充主题覆盖表单、预览和错误，并保持浅色及打印 | 1.318 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 算子和 Module 编辑选择器在深色下可选择并保留输入 | 1.831 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 硬件详情和新增表单统一深色且校验不改写数值 | 1.179 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 独立模型编辑的画布节点、活动页签和 JSON 深色适配 | 1.229 |
| passed | `l1/assets/scaled-nextn.spec.ts` | @L1 派生模型扩充布尔字段预览和创建保持显式选择 | 0.736 |
| passed | `l1/assets/scaled-nextn.spec.ts` | @L1 Decode 页面实际展示 RecoverSSM 开关并提交到工作负载 | 0.439 |
| passed | `l1/assets/table-search.spec.ts` | @L1 model-management 跨页搜索、表头联合筛选和清空恢复 | 1.315 |
| passed | `l1/assets/table-search.spec.ts` | @L1 hardware-management 跨页搜索、表头联合筛选和清空恢复 | 1.308 |
| passed | `l1/assets/table-search.spec.ts` | @L1 operator-management 跨页搜索、表头联合筛选和清空恢复 | 1.511 |
| passed | `l1/assets/table-search.spec.ts` | @L1 module-management 跨页搜索、表头联合筛选和清空恢复 | 1.297 |
| passed | `l1/calibration/calibration-rule-cache.spec.ts` | @L1 校准规则搜索保留已选摘要，分页回包不覆盖完整详情且提交顺序保持 | 1.319 |
| passed | `l1/calibration/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 7.600 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 25.841 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 31.536 |
| passed | `l1/calibration/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 13.105 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 1.004 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.046 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 1.078 |
| passed | `l1/calibration/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 11.634 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手工校准和规则预览的算子候选随阶段筛选 | 1.329 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准优先顺序可调整保存且预览命中首个同级版本 | 1.489 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 1.258 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 1.390 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 0.969 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 1.102 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 1.310 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 1.030 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.095 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling受控构建中刷新恢复保持运行身份 | 2.347 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选完成后刷新恢复与精确报告 | 67.675 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 单条Profiling无源任务构建仅精确Shape候选 | 7.922 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 1.471 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 1.954 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 1.696 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 67.468 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 24.604 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 22.691 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 22.515 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 22.595 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 22.334 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 22.568 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 3.560 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 1.658 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 1.994 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 0.819 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 1.156 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 0.853 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 1.138 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 4.009 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 13.732 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 10.476 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 统一阶段联动、单独覆盖和 P/D 共用量化 | 1.916 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 推理对比复用统一阶段并独立复制配置 | 1.093 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 批量 P/D 预检发送实际阶段精度而非界面草稿 | 1.027 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle decode 提交、算子结果与配置恢复 | 9.725 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 decode 提交、算子结果与配置恢复 | 9.552 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 prefill 提交、算子结果与配置恢复 | 9.725 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 2.957 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 3.308 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 2.979 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 3.564 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 2.660 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 2.691 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 2.610 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 2.978 |
| passed | `l1/inference/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.213 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 1.725 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 1.810 |
| passed | `l1/inference/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 17.405 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 1.715 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 1.657 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.226 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 1.331 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 CP 能力延迟返回不覆盖任务恢复中的并行配置 | 1.076 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 缺少跨 P 能力字段时保留 CP 控件并明确禁用跨 P 传输 | 1.169 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 能力请求失败时 CP 与跨 P 均给出失败提示 | 1.025 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 Diffusion 的序列并行仍受模型图 CP 能力约束 | 1.139 |
| passed | `l1/inference/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 8.718 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 DCP 位于 Decode 并行设置之后，默认折叠并提示先配置 TP | 1.190 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 DCP 开关、分片和高级页大小保持原请求合同与总卡数 | 1.362 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 未适配模型使用普通状态说明，恢复后仍可关闭 DCP | 1.188 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 窄屏和深色模式的 DCP 控件不横向溢出 | 1.319 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 切换部署场景后可直接关闭保留的 DCP 配置 | 1.208 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 DCP 与投机解码冲突时显示处理入口并阻止下一步 | 1.259 |
| passed | `l1/inference/inference-dcp.spec.ts` | @L1 DCP 配置提交、Worker 结果和历史恢复完整闭环 | 13.487 |
| passed | `l1/inference/inference-dcp.spec.ts` | @L1 旧后端缺少能力时保留恢复值并允许显式关闭 DCP | 1.198 |
| passed | `l1/inference/inference-diffusion-pipeline-api.spec.ts` | @L1 MiniMax-H3 PP2 真实任务返回两个 stage 并展示去噪结果 | 12.746 |
| passed | `l1/inference/inference-diffusion-pipeline.spec.ts` | @L1 Diffusion PP3 恢复后可编辑并提交，组件候选不跨 stage | 1.399 |
| passed | `l1/inference/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 8.808 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 1.961 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 1.896 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 0.747 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 0.723 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.001 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 4.962 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 4.944 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 4.810 |
| passed | `l1/inference/inference-operator.spec.ts` | @L1 推理算子性能评估 | 9.885 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 1.274 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 0.991 |
| failed | `l1/inference/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 64.537 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.104 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.215 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.074 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.059 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 189.382 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比显存不足时无可行解 | 17.938 |
| passed | `l1/inference/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 13.956 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理E2E通信下钻与算子统计主题切换保持结果和滚动 | 3.577 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理PD配比KPI及SVG在深色和打印中保持固定快照 | 0.857 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理寻优候选结果主题往返保留筛选与SVG数据 | 0.842 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 A/B结果保持比较语义和主题可读性 | 0.789 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 A/B抽屉的基线、量化和输入在主题往返时保持选择 | 1.514 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理硬件对比结果规格表、倍数标签与折叠在深色和打印间保持数据 | 1.313 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 首次进入等待慢解密和慢管理员角色查询，不提前请求 access | 3.995 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 普通用户首次进入不请求 access，不产生观测接口403 | 0.813 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 真实后端管理员首次进入 access 成功，且角色查询先完成 | 0.704 |
| passed | `l1/shell/pdf-canvas-theme.spec.ts` | @L1 真实 html2canvas 导出解析模型节点变量回退，保留原始字色且隔离深色页面 | 0.670 |
| passed | `l1/shell/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.654 |
| passed | `l1/shell/release-info.spec.ts` | @L1 管理员版本信息 › 编辑版本信息并恢复 | 0.722 |
| passed | `l1/shell/theme-operations.spec.ts` | @L1 用户管理的角色和 Key 弹窗随主题切换，保留浅色及打印样式 | 1.117 |
| passed | `l1/shell/theme-operations.spec.ts` | @L1 版本信息卡片和表头随主题切换，编辑草稿保持不变 | 0.997 |
| passed | `l1/shell/theme-operations.spec.ts` | @L1 校准工作台隐私提示与创建弹窗保持深色可读性和输入状态 | 1.590 |
| passed | `l1/shell/theme.spec.ts` | @L1 共享主题默认浅色、持久化、跨标签页与键盘切换 | 2.185 |
| passed | `l1/shell/theme.spec.ts` | @L1 推理主题切换保持模型、负载、量化与硬件编辑流程 | 1.443 |
| passed | `l1/shell/theme.spec.ts` | @L1 训练/资产/图表共用主题且切换不提交请求 | 2.382 |
| passed | `l1/shell/theme.spec.ts` | @L1 独立模型编辑页和移动端复用主题入口 | 1.044 |
| passed | `l1/shell/theme.spec.ts` | 打印画布主题 › @L1 深色统计图打印使用浅色画布且结束后恢复原偏好 | 1.906 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 详细看板P95复用一位小数格式和未知状态 | 1.098 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 行为筛选不支持时不给全量表格并解释恢复路径 | 1.231 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 用户行为口径显示可理解类别且不冒充真实登录 | 0.973 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻 MCP/API 标签和错误码继承筛选 | 1.300 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻任务到执行逐层返回保留父主题 | 1.180 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻用户会话返回后保留用户选择 | 1.194 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 个人会话权限撤销后不继续展示观测内容 | 0.966 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 0.742 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.094 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 0.837 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 1.199 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 3.085 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 1.041 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 0.827 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 1.512 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 0.914 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 1.131 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 1.152 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 1.173 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 0.842 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 1.284 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.101 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 0.807 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 0.856 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 0.873 |
| passed | `l1/statistics/statistics.spec.ts` | @L1 信息统计访问与导出 | 0.907 |
| failed | `l1/tasks/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 0.855 |
| passed | `l1/tasks/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 1.115 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 0.862 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 0.773 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 0.879 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 0.858 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 0.684 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 9.161 |
| passed | `l1/tasks/task-lifecycle.spec.ts` | @L1 重跑、单删和批删 | 35.125 |
| passed | `l1/tasks/task-table-search.spec.ts` | @L1 任务联合搜索防抖请求、分页与清空 | 3.278 |
| passed | `l1/tasks/task-table-search.spec.ts` | @L1 任务重置回到第一页并丢弃旧条件的延迟响应 | 1.929 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 estimate 嵌入报告实时切换深色，展开和打印下载保留数据 | 1.169 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 strategy_search 嵌入报告实时切换深色，展开和打印下载保留数据 | 1.222 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 hardware_search 嵌入报告实时切换深色，展开和打印下载保留数据 | 1.164 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 TileSim 官方 HTML 复用屏幕主题且离线加载不依赖 CDN | 1.006 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 10.487 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 0.907 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 进度帧与持久化结果 | 21.512 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 进度帧与持久化结果 | 30.351 |
| passed | `l1/training/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 13.291 |
| passed | `l1/training/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 25.078 |
| passed | `l1/training/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 13.642 |
| passed | `l1/training/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 44.143 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 1440px | 0.842 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 1440px | 0.780 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 1440px | 0.788 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 390px | 0.791 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 390px | 0.842 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 390px | 0.809 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 1440px | 0.698 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 1440px | 0.748 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 1440px | 0.792 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 390px | 0.778 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 390px | 0.774 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 390px | 0.883 |
| passed | `l1/training/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 12.794 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 17.903 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 28.944 |
| passed | `l1/training/training-theme.spec.ts` | @L1 train 批量实验四步深色适配保持输入、编排与打印外观 | 1.822 |
| failed | `l1/training/training-theme.spec.ts` | @L1 infer 批量实验四步深色适配保持输入、编排与打印外观 | 1.301 |
| passed | `l1/training/training-theme.spec.ts` | @L1 规格分析基线结果、SVG、旋钮与打印复用同一份数据 | 3.288 |
| skipped | `l2/shell/observability.spec.ts` | @L2 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l2/shell/observability.spec.ts` | @L2 真实后端接受首页浏览器采集批次 | 0.000 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：3581
- Warning：1

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | GET | `/api/tasks?status=succeeded&exclude_internal=true&page=1&page_size=10` | 200 | 826.0 | @L1 任务重置回到第一页并丢弃旧条件的延迟响应 |

