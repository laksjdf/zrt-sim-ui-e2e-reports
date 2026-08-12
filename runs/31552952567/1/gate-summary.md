# Browser E2E Gate

- 结论：**PASS**
- Playwright 退出码：`0`
- 总数：8
- 通过：8
- 失败：0
- 跳过：0

| 状态 | 用例文件 | 用例 | 耗时（秒） |
| --- | --- | --- | ---: |
| passed | `l0/failed-task.spec.ts` | @L0 不存在的配置文件产生可诊断失败 | 8.133 |
| passed | `l0/home.spec.ts` | @L0 首页与核心入口可达 | 1.680 |
| passed | `l0/inference-model.spec.ts` | @L0 推理模型性能评估完整闭环 | 6.967 |
| passed | `l0/service-availability.spec.ts` | @L0 服务读取链路的浏览器请求全部成功 | 1.749 |
| passed | `l0/task-history.spec.ts` | @L0 任务管理与历史结果回跳 | 9.079 |
| passed | `l0/training-model-estimate.spec.ts` | @L0 训练模型评估从浏览器提交到报告和任务历史 | 8.783 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 普通用户可打开用户手册且不可见 API Docs | 1.152 |
| passed | `l0/user-manual-navigation.spec.ts` | @L0 管理员可见 API Docs | 0.702 |
