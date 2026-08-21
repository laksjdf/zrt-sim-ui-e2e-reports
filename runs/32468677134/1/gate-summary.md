# Browser E2E Gate

- 结论：**FAIL（阻断）**
- Playwright 退出码：`1`
- 总数：32
- 通过：31
- 失败：1
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 7.968 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 1.573 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 6.810 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 1.626 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 25.866 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 23.350 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册 | 1.113 |
| passed | `l1/asset-hardware.spec.ts` | @L1 硬件资产 CRUD 与内置保护 | 1.194 |
| passed | `l1/asset-model.spec.ts` | @L1 自定义模型 CRUD 与内置保护 | 2.634 |
| passed | `l1/asset-module.spec.ts` | @L1 Module CRUD 与复用 | 1.680 |
| passed | `l1/asset-operator.spec.ts` | @L1 自定义算子 CRUD | 1.701 |
| passed | `l1/inference-batch-experiment.spec.ts` | @L1 推理批量实验服务闭环 | 7.414 |
| failed | `l1/inference-compare.spec.ts` | @L1 推理硬件性能对比 | 25.062 |
| passed | `l1/inference-custom-communication-tiers.spec.ts` | @L1 推理任务提交用户新增的通信中间层 | 7.407 |
| passed | `l1/inference-hardware-editable.spec.ts` | @L1 推理任务提交修改后的硬件规格并生效 | 7.300 |
| passed | `l1/inference-operator.spec.ts` | @L1 推理算子性能评估 | 9.371 |
| passed | `l1/inference-optimize.spec.ts` | @L1 推理策略寻优与应用策略 | 169.191 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比可行结果 | 27.421 |
| passed | `l1/inference-pd-ratio.spec.ts` | @L1 PD 配比无可行解/OOM | 17.805 |
| passed | `l1/inference-result.spec.ts` | @L1 推理结果筛选和多硬件切换 | 6.805 |
| passed | `l1/release-info.spec.ts` | @L1 版本信息当前和历史读取 | 0.596 |
| passed | `l1/release-info.spec.ts` | @L1 管理员编辑版本信息并恢复 | 0.668 |
| passed | `l1/route-proxy.spec.ts` | @L1 部署前缀和深层路由 | 1.613 |
| passed | `l1/statistics.spec.ts` | @L1 信息统计访问与导出 | 0.665 |
| passed | `l1/task-filter-history.spec.ts` | @L1 任务筛选、详情和历史 Run | 8.349 |
| passed | `l1/task-lifecycle.spec.ts` | @L1 重跑、终止、单删和批删 | 26.849 |
| passed | `l1/training-batch-experiment.spec.ts` | @L1 批量训练实验服务闭环 | 7.261 |
| passed | `l1/training-compare.spec.ts` | @L1 训练多硬件性能对比 | 7.269 |
| passed | `l1/training-hardware-search.spec.ts` | @L1 训练硬件寻优 | 8.214 |
| passed | `l1/training-operator.spec.ts` | @L1 训练算子性能评估 | 11.264 |
| passed | `l1/training-source.spec.ts` | @L1 训练 YAML 与 file 来源 | 18.316 |
| passed | `l1/training-strategy-search.spec.ts` | @L1 训练策略自动寻优 | 11.838 |
