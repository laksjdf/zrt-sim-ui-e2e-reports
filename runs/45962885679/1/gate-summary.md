# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：334
- 通过：317
- 失败：15
- 跳过：2

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/inference/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 14.048 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 未启用硬件时推理评估留在硬件步骤 | 1.244 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 未启用硬件时推理寻优留在硬件步骤 | 1.585 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 取消勾选全部硬件后禁止提交推理评估 | 1.445 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 空白硬件须先填写峰值算力才能提交 | 1.392 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 仿真提交立即显示状态，422 原因可见且允许重试 | 1.404 |
| passed | `l0/inference/inference-submission-errors.spec.ts` | @L0 同布局 P/D 寻优由模型能力开放并提交两侧实例数 | 1.612 |
| passed | `l0/shell/home.spec.ts` | @L0 首页与核心入口可达 | 2.994 |
| passed | `l0/shell/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 2.133 |
| passed | `l0/shell/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.367 |
| passed | `l0/training/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 31.170 |
| passed | `l0/training/training-operator.spec.ts` | @L0 训练算子性能评估 | 8.237 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 空硬件创建两条场景曲线、取消修改并回读已保存的实测值 | 3.110 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 删除仅限当前固定形状，同名场景的其他形状和 FA 实测值保留 | 1.539 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 仿真参考组在编辑后保持顺序，选择另一组可保存并回读 | 2.467 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 沿折线移动显示各场景当前 shape 的实测值或插值 | 1.360 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 FA 按 H 同组对比，Q 始终线性插值，短曲线按端点取值 | 1.383 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 FA 只填 H 与 Q 实测点即可保存，禁止新增重复 H，历史草稿需主动启用 | 1.879 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 跨精度 FA 冲突按场景和 H 选择共享曲线并保留其他测量 | 1.422 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 编辑同名 FA 草稿不会更改已启用的共享曲线 | 1.354 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 PPU 示例按算子和精度展示真实场景 | 1.309 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 infer两层硬件文件导入后编辑与保存保持有效规格 | 1.395 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train两层硬件文件导入后编辑与保存保持有效规格 | 1.460 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 新建硬件仅提供四种拓扑，Clos 选择可往返 YAML | 1.363 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 双场景硬件芯片型号在表单与高级YAML及保存间同步 | 1.621 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 infer旧硬件未配置芯片型号可保存及重新编辑 | 1.533 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train旧硬件未配置芯片型号可保存及重新编辑 | 1.463 |
| passed | `l1/assets/asset-hardware-import.spec.ts` | @L1 train,infer旧硬件未配置芯片型号可保存及重新编辑 | 1.405 |
| passed | `l1/assets/asset-hardware-lifecycle.spec.ts` | @L1 管理员确认后按原资产 ID 编辑、双向转换及删除 | 1.640 |
| passed | `l1/assets/asset-hardware-lifecycle.spec.ts` | @L1 普通用户看不到转换操作且不能修改内置硬件 | 1.135 |
| passed | `l1/assets/asset-hardware-lifecycle.spec.ts` | @L1 读取原始规格期间打开新增，迟到响应不会替换当前表单 | 1.278 |
| passed | `l1/assets/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 2.098 |
| passed | `l1/assets/asset-hardware.spec.ts` | @L1 管理员通过真实资产接口设为内置、编辑、转为非内置及软删除 | 2.120 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 models 管理员使用原始规格编辑、双向转换和按 ID 删除 | 1.589 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 operators 管理员使用原始规格编辑、双向转换和按 ID 删除 | 1.623 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 modules 管理员使用原始规格编辑、双向转换和按 ID 删除 | 1.571 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 普通用户无内置资产生命周期入口，仍可创建模型副本 | 3.192 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 models 真实接口按 ID 维护并保留原始规格 | 1.506 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 operators 真实接口按 ID 维护并保留原始规格 | 1.373 |
| passed | `l1/assets/asset-lifecycle.spec.ts` | @L1 modules 真实接口按 ID 维护并保留原始规格 | 1.380 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页同名保存显示客户端去重错误 | 1.462 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 手搓模型页 409 服务端冲突显示错误提示 | 2.020 |
| passed | `l1/assets/asset-model-conflict.spec.ts` | @L1 训练提交配额超限展示错误提示 | 2.527 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 3.955 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 模型初始化完成前不可输入且加载后保存名称不丢失 | 2.702 |
| passed | `l1/assets/asset-model.spec.ts` | @L1 不同用户可导入同名私有模型且只看到自己的版本 | 1.065 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 乱序成功响应不覆盖当前场景，旧请求结束不提前关闭 loading | 1.620 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭重开后旧查询失败不清空新查询的选项 | 1.244 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 关闭旧编辑后迟到回调不改写新表单的 Spec JSON | 1.190 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首屏仅加载模块，新增时查询算子并随场景切换 | 1.456 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 首次编辑按模块场景读取算子并保留已选项和保存能力 | 1.216 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 新增算子查询失败时结束加载，保留表单且再次打开可重试 | 1.226 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module 算子按需加载 › 编辑算子查询失败时结束加载，保留表单且再次打开可重试 | 1.269 |
| passed | `l1/assets/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 2.285 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 2.419 |
| passed | `l1/assets/asset-operator.spec.ts` | @L1 新增算子失败显示错误并保持弹窗打开 | 1.194 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 模型详情和规模扩充主题覆盖表单、预览和错误，并保持浅色及打印 | 1.473 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 算子和 Module 编辑选择器在深色下可选择并保留输入 | 2.301 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 硬件详情和新增表单统一深色且校验不改写数值 | 1.300 |
| passed | `l1/assets/asset-theme.spec.ts` | @L1 独立模型编辑的画布节点、活动页签和 JSON 深色适配 | 1.315 |
| passed | `l1/assets/scaled-nextn.spec.ts` | @L1 派生模型扩充布尔字段预览和创建保持显式选择 | 0.835 |
| passed | `l1/assets/scaled-nextn.spec.ts` | @L1 Decode 页面实际展示 RecoverSSM 开关并提交到工作负载 | 0.491 |
| passed | `l1/assets/search-curve-scenario.spec.ts` | @L1 寻优提交保留硬件的实现场景 train/optimize/strategy | 2.442 |
| passed | `l1/assets/search-curve-scenario.spec.ts` | @L1 寻优提交保留硬件的实现场景 train/optimize/hardware | 2.484 |
| passed | `l1/assets/search-curve-scenario.spec.ts` | @L1 寻优提交保留硬件的实现场景 infer/optimize/strategy | 3.430 |
| passed | `l1/assets/search-curve-scenario.spec.ts` | @L1 寻优提交保留硬件的实现场景 infer/optimize/pd-ratio | 2.984 |
| passed | `l1/assets/table-search.spec.ts` | @L1 model-management 跨页搜索、表头联合筛选和清空恢复 | 1.632 |
| passed | `l1/assets/table-search.spec.ts` | @L1 hardware-management 跨页搜索、表头联合筛选和清空恢复 | 1.650 |
| passed | `l1/assets/table-search.spec.ts` | @L1 operator-management 跨页搜索、表头联合筛选和清空恢复 | 1.542 |
| passed | `l1/assets/table-search.spec.ts` | @L1 module-management 跨页搜索、表头联合筛选和清空恢复 | 1.544 |
| passed | `l1/assets/task-curve-scenario.spec.ts` | @L1 train 硬件步骤按场景提交，保留资产引用 | 6.270 |
| passed | `l1/assets/task-curve-scenario.spec.ts` | @L1 infer 硬件步骤按场景提交，保留资产引用 | 7.094 |
| passed | `l1/calibration/calibration-rule-cache.spec.ts` | @L1 校准规则搜索保留已选摘要，分页回包不覆盖完整详情且提交顺序保持 | 1.436 |
| failed | `l1/calibration/user-calibration-batch.spec.ts` | @L1 可行批量训练子结果必须命中冻结的用户校准 | 15.961 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 decode 批量任务使用冻结硬件身份命中校准 | 31.880 |
| passed | `l1/calibration/user-calibration-inference-batch.spec.ts` | @L1 prefill 批量任务使用冻结硬件身份命中校准 | 31.638 |
| passed | `l1/calibration/user-calibration-inference.spec.ts` | @L1 推理默认手工校准从页面提交到实际利用率命中 | 13.188 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 校准总览区分启用版本和自动规则 | 1.046 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 版本列表保持整宽并可找回归档版本 | 1.243 |
| passed | `l1/calibration/user-calibration-overview.spec.ts` | @L1 关闭详情后迟到的读取不能重新打开面板 | 1.175 |
| passed | `l1/calibration/user-calibration-task-drawer.spec.ts` | @L1 训练任务一次性校准从设置抽屉进入执行与结果 | 11.841 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手工校准和规则预览的算子候选随阶段筛选 | 1.461 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准优先顺序可调整保存且预览命中首个同级版本 | 1.637 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准已选阶段不隐藏其他候选 | 1.360 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 阶段先选后仅显示同域资产并清除失效选择 | 1.528 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 校准算子目录可搜索原始 key 且支持手输 | 1.067 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 全部 dtype 预览逐项显示局部命中而不误报全回退 | 1.159 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 规则预览输入改变后忽略旧响应且可立即重查 | 1.420 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 修改采集并行策略后必须重新确认 | 1.109 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 首批导入后原弹框继续完成构建准备 | 1.160 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling受控构建中刷新恢复保持运行身份 | 2.466 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选完成后刷新恢复与精确报告 | 67.547 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 单条Profiling无源任务构建仅精确Shape候选 | 10.230 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 源任务不兼容在构建前解释原因且不创建构建任务 | 1.599 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输源任务仅确认后诊断且失败可重试 | 1.940 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 手输任务切换到下拉任务只检查最终选择 | 2.062 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 重查源任务失败后不沿用旧的兼容性通过状态 | 67.651 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 真实训练页面任务可作为 Profiling 候选来源 | 24.511 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选期间修改批次使旧运行失效 | 22.436 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选显式终止后回到草稿 | 22.609 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling终止重载完成前不允许重试并保留新运行终止能力 | 22.354 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling构建候选同页关闭重开从服务器恢复 | 22.497 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling迟到打开版本响应不覆盖较新的构建候选 | 22.674 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling批次迟到错误不污染同版本或另一版本重开 | 4.461 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling追加导入迟到成功不关闭重开的弹窗 | 2.628 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户 Profiling CSV 私有批次导入与移除 | 2.875 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 Profiling 导入明确格式与采集来源 | 1.364 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟补全的原始 kernel_details CSV 可导入并保留原件 | 1.701 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 原始Profiling首次导入失败不遗留空草稿 | 1.533 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 旧草稿拟合响应不能污染新草稿报告 | 1.734 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 用户手工校准工作台闭环 | 5.191 |
| passed | `l1/calibration/user-calibration.spec.ts` | @L1 工作台自动规则作用于普通训练任务且失效前置决策 | 14.535 |
| failed | `l1/calibration/user-calibration.spec.ts` | @L1 模拟原始Profiling从浏览器发布并作用于下一次训练 | 14.418 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 统一阶段联动、单独覆盖和 P/D 共用量化 | 2.607 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 推理对比复用统一阶段并独立复制配置 | 1.467 |
| passed | `l1/configuration/unified-quant-ui.spec.ts` | @L1 批量 P/D 预检发送实际阶段精度而非界面草稿 | 1.564 |
| failed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=16 八项结果 | 6.137 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=32 八项结果 | 1.873 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=48 八项结果 | 1.948 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=64 八项结果 | 1.721 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=96 八项结果 | 1.806 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=128 八项结果 | 1.773 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=192 八项结果 | 1.776 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑页面 N=384 S=384 八项结果 | 1.717 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑直接计算 N=100 S=64 取整边界 | 1.247 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑直接计算 N=8 S=384 取整边界 | 1.240 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑直接计算 N=400 S=384 取整边界 | 1.172 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑直接计算 N=96 S=48 取整边界 | 1.174 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 默认拓扑直接计算 N=1000 S=384 取整边界 | 1.270 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=1 T=1 M=1 | 1.453 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=2 T=1 M=1 | 1.316 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=3 T=1 M=1 | 1.259 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=4 T=1 M=1 | 1.342 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=5 T=1 M=1 | 1.269 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=6 T=1 M=1 | 1.262 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=32 N=3 T=1 M=1 | 1.624 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=128 N=3 T=1 M=1 | 1.331 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=48 N=3 T=1 M=1 | 1.310 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=3 T=2 M=1 | 1.338 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=3 T=1 M=2 | 1.439 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树 R=64 N=3 T=2 M=2 | 1.339 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 真实失焦纠偏 p=100 | 1.418 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 真实失焦纠偏 p=20000000 | 1.428 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 真实失焦纠偏 r=33 | 1.471 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 真实失焦纠偏 n=9 | 1.380 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 真实失焦纠偏 t=100 | 1.349 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 真实失焦纠偏 m=-3 | 1.389 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 初值、空输入跳过、选项顺序、模块独立和重置 | 2.362 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 tooltip、公式和零规模说明完整可见 | 2.239 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 硬件管理入口、链接直达、返回和刷新 | 3.581 |
| failed | `l1/hardware/network-sizing.spec.ts` | @L1 计算无需业务接口、浅深色与移动端无横向溢出 | 3.582 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树Enter提交校验 n=9 | 1.686 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树Enter提交校验 r=33 | 1.622 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树Enter提交校验 t=100 | 1.657 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 胖树Enter提交校验 m=-3 | 1.607 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 折叠的配置无效时自动展开并显示错误 | 2.074 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 通用标题、1520可选及自定义交换型号 | 2.976 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 自定义拓扑、超节点规模和卡数倍数纠偏 | 2.294 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 不统计交换芯片时保留未知状态及CPU加速卡配比 | 2.233 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 参数变更清除旧结果且不影响胖树，重置恢复参考参数 | 1.895 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 超节点卡数及拓扑非法参数有可见错误并阻止计算 | 2.765 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 卡数加减默认按8步进并保持上下限和倍数对齐 | 1.281 |
| passed | `l1/hardware/network-sizing.spec.ts` | @L1 单层交换方案只统计L1并支持自定义8卡超节点 | 1.807 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle decode 提交、算子结果与配置恢复 | 10.588 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 decode 提交、算子结果与配置恢复 | 10.431 |
| passed | `l1/inference/eagle-single-chain.spec.ts` | @L1 eagle3 prefill 提交、算子结果与配置恢复 | 10.684 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Prefill 可编辑 EP 与自动 EDP | 3.897 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate Decode 可编辑 EP 与自动 EDP | 3.878 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 混布 可编辑 EP 与自动 EDP | 3.832 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 evaluate PD 分离 可编辑 EP 与自动 EDP | 4.307 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Prefill 可编辑 EP 与自动 EDP | 3.111 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize Decode 可编辑 EP 与自动 EDP | 2.667 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 optimize PD 混布 可编辑 EP 与自动 EDP | 3.218 |
| passed | `l1/inference/inference-auto-ep.spec.ts` | @L1 pd-ratio PD 分离 可编辑 EP 与自动 EDP | 3.887 |
| passed | `l1/inference/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.765 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：strategy_search | 2.255 |
| passed | `l1/inference/inference-batch-optimization-toggle.spec.ts` | @L1 推理批量实验寻优开关可往返切换：hardware_sensitivity | 2.228 |
| passed | `l1/inference/inference-compare-sla.spec.ts` | @L1 固定物理卡多档对比与复评下载 | 28.455 |
| passed | `l1/inference/inference-compare-sla.spec.ts` | @L1 复制旧扁平硬件任务按冻结拓扑恢复设备规模 | 16.650 |
| passed | `l1/inference/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 18.092 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 evaluate Decode 配置在前后步骤往返时完整保留 | 2.275 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 optimize Decode 配置在前后步骤往返时完整保留 | 2.302 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=1 切分不增加总卡数并保留步骤编辑 | 1.748 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 独立 O-TP=2 CP=2 切分不增加总卡数并保留步骤编辑 | 1.711 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 CP 能力延迟返回不覆盖任务恢复中的并行配置 | 1.507 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 缺少跨 P 能力字段时保留 CP 控件并明确禁用跨 P 传输 | 1.507 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 能力请求失败时 CP 与跨 P 均给出失败提示 | 1.530 |
| passed | `l1/inference/inference-config-navigation.spec.ts` | @L1 Diffusion 的序列并行仍受模型图 CP 能力约束 | 1.480 |
| passed | `l1/inference/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 12.261 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 DCP 位于 Decode 并行设置之后，默认折叠并提示先配置 TP | 1.557 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 DCP 开关、分片和高级页大小保持原请求合同与总卡数 | 1.798 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 未适配模型使用普通状态说明，恢复后仍可关闭 DCP | 1.501 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 窄屏和深色模式的 DCP 控件不横向溢出 | 1.714 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 切换部署场景后可直接关闭保留的 DCP 配置 | 1.611 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 DCP 与投机解码冲突时显示处理入口并阻止下一步 | 1.642 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 Decode 自动寻优独立选择 PP 和 DCP，恢复已保存候选 | 1.665 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 P/D 混布可编辑两个批量并切回整体批量 | 1.714 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 Kimi 混布限制卸载、PP 和最短输出，显示固定搜索批量 | 1.622 |
| passed | `l1/inference/inference-dcp-ui.spec.ts` | @L1 恢复单侧固定批量后清空仍可编辑 | 1.561 |
| passed | `l1/inference/inference-dcp.spec.ts` | @L1 DCP 配置提交、Worker 结果和历史恢复完整闭环 | 20.767 |
| passed | `l1/inference/inference-dcp.spec.ts` | @L1 旧后端缺少能力时保留恢复值并允许显式关闭 DCP | 1.493 |
| passed | `l1/inference/inference-diffusion-pipeline-api.spec.ts` | @L1 MiniMax-H3 PP2 真实任务返回两个 stage 并展示去噪结果 | 13.009 |
| passed | `l1/inference/inference-diffusion-pipeline.spec.ts` | @L1 Diffusion PP3 恢复后可编辑并提交，组件候选不跨 stage | 1.861 |
| passed | `l1/inference/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 12.322 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 配置恢复与性能评估结果 | 2.944 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 配置恢复 | 2.699 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 HiCache 冻结最优解寻优结果 | 1.146 |
| passed | `l1/inference/inference-hicache.spec.ts` | @L1 标准 KV Offload 冻结最优解带宽结果 | 1.165 |
| passed | `l1/inference/inference-memory-estimates.spec.ts` | @L1 实际寻优任务的估算诊断在历史页面和下载中保持 | 10.542 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_UNSUPPORTED | 5.451 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.MODEL.O_TP_GRAPH_INVALID | 5.496 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.CONFIG.O_TP_INVALID | 5.423 |
| passed | `l1/inference/inference-o-tp-errors.spec.ts` | @L1 O-TP 轮询错误展示 TASK.UNKNOWN | 5.224 |
| passed | `l1/inference/inference-operator.spec.ts` | @L1 推理算子性能评估 | 13.052 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置统计表硬件过滤与自适应高度 | 1.625 |
| passed | `l1/inference/inference-optimal-table.spec.ts` | @L1 推理最优配置分档表硬件过滤与自适应高度 | 1.401 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 150.631 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置恢复 Chunked Prefill Size | 1.348 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置在第 2 → 1 → 2 步保留量化和编辑值 | 1.553 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 禁用 Chunked Prefill Size | 1.357 |
| passed | `l1/inference/inference-optimize.spec.ts` | @L1 Prefill 重用配置兼容 缺失 Chunked Prefill Size | 1.308 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 419.873 |
| passed | `l1/inference/inference-pd-ratio.spec.ts` | @L1 PD 配比显存不足时无可行解 | 17.935 |
| passed | `l1/inference/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 18.549 |
| passed | `l1/inference/inference-run-clock.spec.ts` | @L1 main 推理历史按本次执行恢复计时，终态停止展示等待 | 4.677 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 结果页按冻结运行调参并复用已另存硬件 | 2.632 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理E2E通信下钻与算子统计主题切换保持结果和滚动 | 4.991 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理PD配比KPI及SVG在深色和打印中保持固定快照 | 1.857 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理寻优候选结果主题往返保留筛选与SVG数据 | 3.128 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 A/B结果保持比较语义和主题可读性 | 1.141 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 A/B抽屉的基线、量化和输入在主题往返时保持选择 | 1.863 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 推理硬件对比结果规格表、倍数标签与折叠在深色和打印间保持数据 | 1.701 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 同布局 P/D 寻优恢复冻结的 TTFT 和实例数 | 1.880 |
| passed | `l1/inference/inference-theme.spec.ts` | @L1 同布局 P/D 寻优没有候选时仍显示系统输出吞吐口径 | 1.187 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 首次进入等待慢解密和慢管理员角色查询，不提前请求 access | 1.632 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 普通用户首次进入不请求 access，不产生观测接口403 | 1.094 |
| passed | `l1/operations-access-ready.spec.ts` | @L1 真实后端管理员首次进入 access 成功，且角色查询先完成 | 1.023 |
| passed | `l1/shell/log-viewer.spec.ts` | @L1 log search reveals the last match after window growth and switches nodes | 1.601 |
| passed | `l1/shell/pdf-canvas-theme.spec.ts` | @L1 真实 html2canvas 导出解析模型节点变量回退，保留原始字色且隔离深色页面 | 1.205 |
| passed | `l1/shell/preferences-navigation.spec.ts` | @L1 基础导航常驻、运维分组权限及键盘菜单 | 1.316 |
| passed | `l1/shell/preferences-navigation.spec.ts` | @L1 主题独立按钮、重建浏览器上下文记忆及个人偏好保存 | 2.646 |
| passed | `l1/shell/preferences-navigation.spec.ts` | @L1 管理员在二级菜单进入管理功能且返回主页不被起始页重定向 | 1.346 |
| passed | `l1/shell/preferences-navigation.spec.ts` | @L1 偏好读取缓慢不会阻塞列表或迟到覆盖本次筛选 | 1.294 |
| passed | `l1/shell/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.976 |
| passed | `l1/shell/release-info.spec.ts` | @L1 管理员版本信息 › 编辑版本信息并恢复 | 1.092 |
| passed | `l1/shell/theme-consistency.spec.ts` | @L1 train 算子输入与原生分组选项随主题切换并保持编辑值 | 1.277 |
| passed | `l1/shell/theme-consistency.spec.ts` | @L1 recommend 算子输入与原生分组选项随主题切换并保持编辑值 | 1.357 |
| passed | `l1/shell/theme-consistency.spec.ts` | @L1 infer 算子输入与原生分组选项随主题切换并保持编辑值 | 1.373 |
| passed | `l1/shell/theme-consistency.spec.ts` | @L1 硬件浮层、选中项与主按钮使用同一主题且明暗别名一致 | 3.402 |
| passed | `l1/shell/theme-consistency.spec.ts` | @L1 组网测算主按钮继承统一主色并保持计算结果 | 1.903 |
| passed | `l1/shell/theme-consistency.spec.ts` | @L1 日志工具栏与备份确认框随主题切换，保留终端语义色和输入 | 2.234 |
| passed | `l1/shell/theme-operations.spec.ts` | @L1 用户管理的角色和 Key 弹窗随主题切换，保留浅色及打印样式 | 1.579 |
| passed | `l1/shell/theme-operations.spec.ts` | @L1 版本信息卡片和表头随主题切换，编辑草稿保持不变 | 1.286 |
| passed | `l1/shell/theme-operations.spec.ts` | @L1 校准工作台隐私提示与创建弹窗保持深色可读性和输入状态 | 2.667 |
| passed | `l1/shell/theme.spec.ts` | @L1 共享主题默认浅色、持久化、跨标签页与键盘切换 | 3.318 |
| passed | `l1/shell/theme.spec.ts` | @L1 推理主题切换保持模型、负载、量化与硬件编辑流程 | 2.022 |
| passed | `l1/shell/theme.spec.ts` | @L1 训练/资产/图表共用主题且切换不提交请求 | 3.716 |
| passed | `l1/shell/theme.spec.ts` | @L1 独立模型编辑页和移动端复用主题入口 | 1.564 |
| passed | `l1/shell/theme.spec.ts` | 打印画布主题 › @L1 深色统计图打印使用浅色画布且结束后恢复原偏好 | 2.781 |
| passed | `l1/shell/user-management-access.spec.ts` | @L1 用户管理仅接受明确的本地初始化许可，创建后重新检查本人角色 | 4.245 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 详细看板P95复用一位小数格式和未知状态 | 1.627 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 行为筛选不支持时不给全量表格并解释恢复路径 | 1.574 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 用户行为口径显示可理解类别且不冒充真实登录 | 1.603 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻 MCP/API 标签和错误码继承筛选 | 2.168 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻任务到执行逐层返回保留父主题 | 2.260 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 下钻用户会话返回后保留用户选择 | 1.880 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 个人会话权限撤销后不继续展示观测内容 | 1.705 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 产品运行与洞察真实接口或未启用路径 | 1.161 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 MCP服务健康展示调用趋势和工具拆分 | 1.647 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 无权限不得展示敏感内容和入口 | 1.315 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 闭环与页面行为只展示后端聚合事实 | 1.725 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 日期竞态、筛选与实时独立口径 | 3.709 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 主题分页、排序、标签保留与Escape恢复焦点 | 1.853 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 局部失败、新鲜度和未知Worker不冒充空闲 | 1.503 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 账号切换立即清空并拒绝旧权限响应 | 2.198 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 弹窗返回保持原滚动位置 | 1.582 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 后台暂停轮询且离页后只保留轻量权限 | 1.997 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 多部门默认全量，409回首页，403撤回全部数据 | 1.962 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 live刷新和全局草稿不重置主题第二页 | 1.886 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 直达主题Escape只移除topic保留其他query | 1.777 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 跨上海午夜点击预设刷新服务端锚点而固定日期不漂移 | 1.982 |
| passed | `l1/statistics/operations-insights.spec.ts` | @L1 R1 排序实参和200无心跳Worker未知 | 1.793 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计空数据态展示暂无数据 | 1.459 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计部分子请求失败展示降级提示 | 1.539 |
| passed | `l1/statistics/statistics-edge.spec.ts` | @L1 信息统计导出失败展示错误提示 | 1.584 |
| passed | `l1/statistics/statistics.spec.ts` | @L1 信息统计访问与导出 | 1.659 |
| failed | `l1/tasks/resource-quotas.spec.ts` | @L1 管理员角色配额与搜索页额度提示 | 2.280 |
| passed | `l1/tasks/resource-quotas.spec.ts` | @L1 本地普通用户遵守管理员配置的精度校准菜单禁用 | 2.111 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 失败任务详情展示结构化错误卡片 | 1.538 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 任务空列表态与筛选无结果 | 1.444 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 进程启动失败展示后端异常原文 | 1.412 |
| passed | `l1/tasks/task-failure-detail.spec.ts` | @L1 历史遗留失败任务展示 legacy 错误信息 | 1.540 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务管理只请求业务任务列表 | 1.108 |
| passed | `l1/tasks/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 14.197 |
| passed | `l1/tasks/task-lifecycle.spec.ts` | @L1 重跑、单删和批删 | 55.112 |
| passed | `l1/tasks/task-table-search.spec.ts` | @L1 任务联合搜索防抖请求、分页与清空 | 3.945 |
| passed | `l1/tasks/task-table-search.spec.ts` | @L1 任务重置回到第一页并丢弃旧条件的延迟响应 | 2.642 |
| passed | `l1/training/batch-role-limits.spec.ts` | @L1 train 批量预算默认交由角色配置 | 1.576 |
| passed | `l1/training/batch-role-limits.spec.ts` | @L1 train 批量预算保留高级配置 | 2.721 |
| passed | `l1/training/batch-role-limits.spec.ts` | @L1 infer 批量预算默认交由角色配置 | 1.494 |
| passed | `l1/training/batch-role-limits.spec.ts` | @L1 infer 批量预算保留高级配置 | 2.167 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 训练结果调参仅提交指定运行的改动并保留原报告 | 2.542 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 estimate 嵌入报告实时切换深色，展开和打印下载保留数据 | 2.157 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 strategy_search 嵌入报告实时切换深色，展开和打印下载保留数据 | 2.226 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 hardware_search 嵌入报告实时切换深色，展开和打印下载保留数据 | 1.867 |
| passed | `l1/training/report-frame-theme.spec.ts` | @L1 TileSim 官方 HTML 复用屏幕主题且离线加载不依赖 CDN | 1.695 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 baseline renders server frames and hides failures | 16.298 |
| passed | `l1/training/task10-layout.spec.ts` | @L1 Task10 desktop columns and responsive quant controls | 1.674 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 baseline 进度帧与持久化结果 | 35.455 |
| passed | `l1/training/training-analysis-progress.spec.ts` | @L1 真实训练分析 compare 进度帧与持久化结果 | 47.428 |
| passed | `l1/training/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 22.166 |
| passed | `l1/training/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 40.064 |
| passed | `l1/training/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 22.490 |
| passed | `l1/training/training-multimodal-pp-submit.spec.ts` | @L1 多模态训练 PP1 与 PP8 均能提交并完成评估 | 50.762 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 1440px | 1.377 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 1440px | 1.318 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 1440px | 1.364 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-full at 390px | 1.340 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute dense-attention at 390px | 1.386 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training strategy recompute legacy at 390px | 1.381 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 1440px | 1.271 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 1440px | 1.190 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 1440px | 1.238 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-full at 390px | 1.219 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute dense-attention at 390px | 1.323 |
| passed | `l1/training/training-recompute-label.spec.ts` | @L1 training hardware recompute legacy at 390px | 1.223 |
| passed | `l1/training/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 13.768 |
| passed | `l1/training/training-task-progress.spec.ts` | @L1 训练strategy真实任务进度与结果 | 27.739 |
| failed | `l1/training/training-task-progress.spec.ts` | @L1 训练hardware真实任务进度与结果 | 0.072 |
| passed | `l1/training/training-theme.spec.ts` | @L1 train 批量实验四步深色适配保持输入、编排与打印外观 | 1.373 |
| passed | `l1/training/training-theme.spec.ts` | @L1 infer 批量实验四步深色适配保持输入、编排与打印外观 | 1.371 |
| failed | `l1/training/training-theme.spec.ts` | @L1 规格分析基线结果、SVG、旋钮与打印复用同一份数据 | 2.732 |
| skipped | `l2/shell/observability.spec.ts` | @L2 显式开启时首页发送受控浏览器采集批次 | 0.000 |
| skipped | `l2/shell/observability.spec.ts` | @L2 真实后端接受首页浏览器采集批次 | 0.000 |

## 接口响应时延观测（不阻断）

- 阈值：500ms
- 已记录接口请求：4774
- Warning：2

| 状态 | 方法 | 接口 | HTTP | 耗时（ms） | 用例 |
| --- | --- | --- | ---: | ---: | --- |
| warning | GET | `/api/tasks?status=succeeded&exclude_internal=true&page=1&page_size=10` | 200 | 842.0 | @L1 任务重置回到第一页并丢弃旧条件的延迟响应 |
| warning | GET | `/api/jobs/36-1` | 200 | 587.0 | @L1 推理策略寻优与应用策略 |

