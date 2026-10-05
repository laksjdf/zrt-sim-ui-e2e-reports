# Browser E2E Gate

- 结论：**PASS**
- Playwright 退出码：`0`
- 总数：156
- 通过：154
- 失败：0
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle decode 提交、算子结果与配置恢复 | 12.973 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 decode 提交、算子结果与配置恢复 | 11.526 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 prefill 提交、算子结果与配置恢复 | 11.582 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.334 |
| skipped | `l0/home.spec.ts` | @L0 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l0/home.spec.ts` | @L0 真实后端接受首页浏览器采集批次 | 0.000 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 13.915 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 4.951 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 34.085 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 29.898 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 共用量化 | 3.166 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 2.035 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 2.022 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 2.864 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.684 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 2.506 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 2.646 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 3.031 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 5.134 |
| passed | `l1/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.741 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 2.065 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.843 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.933 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 2.547 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.911 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.951 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.793 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.752 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 4.631 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 2.061 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 4.588 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 4.592 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 4.844 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 5.221 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.738 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 3.665 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 3.817 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 4.567 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.670 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.850 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.898 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 168.523 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.779 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 2.680 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 2.412 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 2.490 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.611 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.747 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 4.102 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 4.062 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 1.953 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.706 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.728 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 5.868 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 5.848 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 5.934 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 13.576 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 2.419 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 2.022 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 13.304 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 2.099 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 2.413 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 2.202 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 2.177 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 49.969 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 28.550 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 14.665 |
| passed | `l1/operations-insights.spec.ts` | @L1 详细看板P95复用一位小数格式和未知状态 | 2.048 |
| passed | `l1/operations-insights.spec.ts` | @L1 行为筛选不支持时不给全量表格并解释恢复路径 | 2.044 |
| passed | `l1/operations-insights.spec.ts` | @L1 用户行为口径显示可理解类别且不冒充真实登录 | 1.992 |
| passed | `l1/operations-insights.spec.ts` | @L1 下钻 MCP/API 标签和错误码继承筛选 | 2.244 |
| passed | `l1/operations-insights.spec.ts` | @L1 下钻任务到执行逐层返回保留父主题 | 2.041 |
| passed | `l1/operations-insights.spec.ts` | @L1 下钻用户会话返回后保留用户选择 | 2.145 |
| passed | `l1/operations-insights.spec.ts` | @L1 个人会话权限撤销后不继续展示观测内容 | 1.886 |
| passed | `l1/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.474 |
| passed | `l1/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.950 |
| passed | `l1/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.735 |
| passed | `l1/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 2.115 |
| passed | `l1/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 4.038 |
| passed | `l1/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 2.231 |
| passed | `l1/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.722 |
| passed | `l1/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 2.473 |
| passed | `l1/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.899 |
| passed | `l1/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 2.092 |
| passed | `l1/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 2.210 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 1.995 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 1.870 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 2.319 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.905 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 1.501 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.641 |
| passed | `l1/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 3.402 |
| passed | `l1/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 2.556 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 4.730 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.735 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.597 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.827 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.732 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.853 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.908 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 1.734 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 1.772 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 1.511 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 17.346 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 33.315 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 13.612 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 2.020 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 23.823 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 36.015 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 14.246 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 77.155 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 23.647 |
| passed | `l1/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 46.116 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.037 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 10.397 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 19.330 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 19.776 |
| passed | `l1/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 8.361 |
| passed | `l1/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 14.140 |
| passed | `l1/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 14.270 |
| passed | `l1/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 11.167 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 1.717 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.844 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 1.832 |
| passed | `l1/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 12.398 |
| passed | `l1/user-calibration.spec.ts` | @L1 手工校准和规则预览的算子候选随阶段筛选 | 2.104 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准优先顺序可调整保存且预览命中首个同级版本 | 2.145 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 1.973 |
| passed | `l1/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 2.219 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 1.817 |
| passed | `l1/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 1.786 |
| passed | `l1/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 1.874 |
| passed | `l1/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 1.698 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.786 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选提交、刷新恢复与精确报告 | 15.114 |
| passed | `l1/user-calibration.spec.ts` | @L1 单条Profiling无源任务构建仅精确Shape候选 | 8.373 |
| passed | `l1/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 2.169 |
| passed | `l1/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 2.588 |
| passed | `l1/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 2.356 |
| passed | `l1/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 8.315 |
| passed | `l1/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 32.894 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 8.529 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 16.917 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 8.694 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 14.537 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 15.001 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 5.569 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 2.697 |
| passed | `l1/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 3.024 |
| passed | `l1/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 1.747 |
| passed | `l1/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 2.098 |
| passed | `l1/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 1.900 |
| passed | `l1/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 2.158 |
| passed | `l1/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 5.824 |
| passed | `l1/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 11.678 |
| passed | `l1/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 29.077 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：3313
- Warning：13

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | GET | `/api/calibrations/versions/74b6596e25424170baa8fbf7159f9257` | 200 | 6363.0 | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 |
| warning | GET | `/api/assets/models` | 200 | 2703.0 | @L1 Profiling构建候选期间修改批次使旧运行失效 |
| warning | GET | `/api/assets/hardwares?owner=pw_0_1791243964012` | 200 | 2702.0 | @L1 Profiling构建候选期间修改批次使旧运行失效 |
| warning | GET | `/api/tasks?domain=train&operation=estimate&status=succeeded&page_size=50` | 200 | 2689.0 | @L1 Profiling构建候选期间修改批次使旧运行失效 |
| warning | GET | `/api/assets/operators` | 200 | 2689.0 | @L1 Profiling构建候选期间修改批次使旧运行失效 |
| warning | GET | `/api/calibrations/versions/014c964164e74b1ca1bd2090eec1d4a3` | 200 | 2689.0 | @L1 Profiling构建候选期间修改批次使旧运行失效 |
| warning | GET | `/api/calibrations/versions/014c964164e74b1ca1bd2090eec1d4a3/batches` | 200 | 2684.0 | @L1 Profiling构建候选期间修改批次使旧运行失效 |
| warning | POST | `/api/user/decrypt` | 200 | 2481.0 | @L1 自定义模型 CRUD 与内置保护 |
| warning | POST | `/api/user/decrypt` | 200 | 610.0 | @L1 硬件资产 CRUD 与内置保护 |
| warning | POST | `/api/user/decrypt` | 200 | 610.0 | @L1 训练strategy真实任务进度与结果 |
| warning | POST | `/api/user/decrypt` | 200 | 592.0 | @L1 版本列表保持整宽并可找回归档版本 |
| warning | POST | `/api/user/decrypt` | 200 | 569.0 | @L1 prefill 批量任务使用冻结硬件身份命中校准 |
| warning | POST | `/api/jobs/31-1/result-viewed` | 202 | 501.0 | @L1 训练hardware真实任务进度与结果 |

