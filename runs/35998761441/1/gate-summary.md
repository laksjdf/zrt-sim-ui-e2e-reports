# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：119
- 通过：101
- 失败：16
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle decode 提交、算子结果与配置恢复 | 12.878 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 decode 提交、算子结果与配置恢复 | 10.163 |
| passed | `l0/eagle-single-chain.spec.ts` | @L0 eagle3 prefill 提交、算子结果与配置恢复 | 10.271 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 2.417 |
| skipped | `l0/home.spec.ts` | @L0 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l0/home.spec.ts` | @L0 真实后端接受首页浏览器采集批次 | 0.000 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 8.576 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 2.984 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 25.501 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 27.828 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 统一阶段联动、单独覆盖和 P/D 共用量化 | 2.379 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 推理对比复用统一阶段并独立复制配置 | 1.295 |
| passed | `l0/unified-quant-ui.spec.ts` | @L0 批量 P/D 预检发送实际阶段精度而非界面草稿 | 1.375 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.599 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.887 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 1.715 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 1.680 |
| passed | `l1/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 2.436 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.194 |
| passed | `l1/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.052 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.243 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.283 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.212 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 1.378 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.194 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.265 |
| passed | `l1/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.305 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.432 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.478 |
| passed | `l1/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.180 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 3.578 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 3.677 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 3.580 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 4.107 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.078 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 2.947 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 3.078 |
| passed | `l1/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 3.261 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.585 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.063 |
| passed | `l1/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.155 |
| passed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 217.826 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.036 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 2.036 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.629 |
| passed | `l1/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 1.671 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 9.129 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 9.076 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 2.664 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 2.574 |
| passed | `l1/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 1.082 |
| passed | `l1/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.085 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.349 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 5.327 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 5.339 |
| passed | `l1/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 5.186 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 9.964 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 1.533 |
| passed | `l1/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 1.437 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 12.843 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.405 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.549 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.476 |
| passed | `l1/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.429 |
| failed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 6.542 |
| failed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 6.504 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 18.636 |
| passed | `l1/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.025 |
| passed | `l1/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.161 |
| passed | `l1/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.014 |
| passed | `l1/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 1.268 |
| passed | `l1/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 3.413 |
| passed | `l1/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 1.348 |
| passed | `l1/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.146 |
| passed | `l1/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 1.785 |
| passed | `l1/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.151 |
| passed | `l1/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 1.248 |
| failed | `l1/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 6.235 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 1.346 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 1.163 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 1.420 |
| passed | `l1/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.182 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.942 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 1.000 |
| passed | `l1/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 1.867 |
| passed | `l1/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 1.784 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 2.602 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.040 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.080 |
| passed | `l1/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.141 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.133 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.149 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.012 |
| failed | `l1/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 1.122 |
| passed | `l1/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 1.180 |
| failed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 24.810 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 29.219 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 13.582 |
| passed | `l1/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 1.143 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 两帧进度与持久化结果 | 19.716 |
| passed | `l1/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 两帧进度与持久化结果 | 28.694 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 13.618 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 67.400 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 14.384 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 8.319 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 12.965 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 17.602 |
| passed | `l1/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 18.446 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选提交、刷新恢复与诊断报告 | 22.370 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 22.418 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 22.410 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 22.465 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 22.447 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 22.449 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 16.376 |
| failed | `l1/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 16.353 |
| failed | `l1/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 16.392 |
| failed | `l1/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 16.442 |
| failed | `l1/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 6.194 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：1541
- Warning：1

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | POST | `/api/user/decrypt` | 200 | 613.0 | @L0 eagle decode 提交、算子结果与配置恢复 |

