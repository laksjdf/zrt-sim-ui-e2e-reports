# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：146
- 通过：114
- 失败：30
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle decode 提交、算子结果与配置恢复 | 14.053 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 decode 提交、算子结果与配置恢复 | 12.115 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 prefill 提交、算子结果与配置恢复 | 11.665 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 4.896 |
| skipped | `l0/home.spec.ts` | @L0 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l0/home.spec.ts` | @L0 真实后端接受首页浏览器采集批次 | 0.000 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 14.208 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 5.665 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 35.080 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 34.958 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 共用量化 | 3.627 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 2.333 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 2.412 |
| failed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 6.778 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.820 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 2.940 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 2.864 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 3.499 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 6.109 |
| passed | `l1/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 2.091 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 2.228 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 2.181 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 2.166 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 2.376 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 2.167 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 2.193 |
| failed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 2.168 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 4.851 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 4.539 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 2.044 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 4.796 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 4.936 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 5.057 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 5.446 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 4.076 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 4.207 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 4.132 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 4.673 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 8.320 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.987 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 3.248 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 179.587 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 3.171 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 3.150 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 2.585 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 2.838 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.984 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.779 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 4.399 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 3.975 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 2.043 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 2.008 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 6.252 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 6.369 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 6.263 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 6.422 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 10.910 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 2.693 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 2.546 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 13.876 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 2.519 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 2.563 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 2.370 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 2.386 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 60.119 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 28.924 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 24.291 |
| passed | `l1/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.745 |
| passed | `l1/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.957 |
| passed | `l1/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.922 |
| passed | `l1/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 2.217 |
| passed | `l1/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 4.177 |
| passed | `l1/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 2.504 |
| passed | `l1/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 2.208 |
| passed | `l1/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 2.858 |
| passed | `l1/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 2.010 |
| passed | `l1/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 2.440 |
| passed | `l1/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 2.347 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 2.470 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 2.276 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 2.421 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 2.102 |
| failed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 15.529 |
| failed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 15.151 |
| passed | `l1/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 3.537 |
| passed | `l1/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 3.178 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 5.580 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 2.228 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 2.212 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 2.190 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 2.025 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 2.061 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.928 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 2.084 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 2.053 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 1.813 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 14.182 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 47.617 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 17.008 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 2.329 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 27.172 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 39.203 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 14.167 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 88.742 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 24.075 |
| passed | `l1/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 46.523 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 9.205 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 11.201 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 19.530 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 21.105 |
| passed | `l1/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 8.625 |
| passed | `l1/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 14.399 |
| passed | `l1/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 14.442 |
| passed | `l1/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 11.448 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 1.788 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.921 |
| passed | `l1/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 1.910 |
| passed | `l1/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 12.480 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 2.165 |
| passed | `l1/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 2.232 |
| passed | `l1/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 1.841 |
| passed | `l1/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 2.034 |
| passed | `l1/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 2.143 |
| failed | `l1/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 2.001 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.936 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选提交、刷新恢复与诊断报告 | 8.062 |
| failed | `l1/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 1.932 |
| failed | `l1/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 1.980 |
| failed | `l1/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 2.129 |
| failed | `l1/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 8.072 |
| failed | `l1/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 27.064 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 8.188 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 8.042 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 8.248 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 8.152 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 8.065 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 2.010 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 1.995 |
| passed | `l1/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 3.398 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 7.297 |
| failed | `l1/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 2.225 |
| failed | `l1/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 2.133 |
| passed | `l1/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 2.523 |
| passed | `l1/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 7.371 |
| failed | `l1/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 15.295 |
| failed | `l1/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 0.485 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：2539
- Warning：1

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | POST | `/api/user/decrypt` | 200 | 574.0 | @L0 eagle decode 提交、算子结果与配置恢复 |

