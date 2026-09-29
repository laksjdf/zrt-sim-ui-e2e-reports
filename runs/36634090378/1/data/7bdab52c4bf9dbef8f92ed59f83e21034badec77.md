# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: l1/user-calibration.spec.ts >> @L1 原始Profiling首次导入失败不遗留空草稿
- Location: e2e/specs/l1/user-calibration.spec.ts:900:1

# Error details

```
Error: ENOENT: no such file or directory, open '/home/administrator/actions-runner/_work/zrt-sim-ui/zrt-sim-ui/backend-repo/tests/calibration/fixtures/kernel_details.csv'
```

# Page snapshot

```yaml
- generic [ref=e3]:
  - banner [ref=e4]:
    - generic [ref=e5]: ZRT
    - generic [ref=e6]: AI负载建模仿真平台
    - generic [ref=e7]:
      - link "返回主页" [ref=e8] [cursor=pointer]:
        - /url: /zrt-sim/
        - img [ref=e9]
        - generic [ref=e12]: 返回主页
      - link "任务管理" [ref=e13] [cursor=pointer]:
        - /url: /zrt-sim/tasks
      - link "资产管理" [ref=e14] [cursor=pointer]:
        - /url: /zrt-sim/assets
      - link "信息统计" [ref=e15] [cursor=pointer]:
        - /url: /zrt-sim/statistics
      - link "精度校准" [ref=e16] [cursor=pointer]:
        - /url: /zrt-sim/calibration
      - link "版本信息" [ref=e17] [cursor=pointer]:
        - /url: /zrt-sim/release-notes
      - link "用户管理" [ref=e18] [cursor=pointer]:
        - /url: /zrt-sim/user-manage
      - link "用户手册" [ref=e19] [cursor=pointer]:
        - /url: /zrt-sim/user-manual
      - button "pw_user_27_1790719105233" [ref=e20] [cursor=pointer]:
        - img [ref=e21]
        - generic [ref=e24]: pw_user_27_1790719105233
      - generic [ref=e26]: Calibration
  - main [ref=e27]:
    - generic [ref=e28]:
      - link "首页" [ref=e29] [cursor=pointer]:
        - /url: /zrt-sim/
      - generic [ref=e30]: /
      - generic [ref=e31]: 精度校准
    - generic [ref=e32]:
      - generic [ref=e33]:
        - generic [ref=e34]:
          - heading "用户精度校准" [level=1] [ref=e35]
          - paragraph [ref=e36]: 管理仅自己可见的手工校准版本与 Profiling 导入批次；未验证数据不会用于任务。
        - button "新建校准版本" [ref=e37] [cursor=pointer]
      - note [ref=e38]:
        - strong [ref=e39]: Profiling 校准
        - generic [ref=e40]: 支持原始 kernel_details.csv 与规范 CSV/ZIP 增量导入；仅正式验证通过的 Profiling 版本可发布并用于后续训练任务。
      - generic [ref=e41]:
        - navigation "校准工作台导航" [ref=e42]:
          - button "总览 资产与能力边界" [ref=e43] [cursor=pointer]:
            - strong [ref=e44]: 总览
            - generic [ref=e45]: 资产与能力边界
          - button "我的校准版本 筛选、修订与启停" [ref=e46] [cursor=pointer]:
            - strong [ref=e47]: 我的校准版本
            - generic [ref=e48]: 筛选、修订与启停
          - button "默认规则与预览 真实规则与命中结果" [ref=e49] [cursor=pointer]:
            - strong [ref=e50]: 默认规则与预览
            - generic [ref=e51]: 真实规则与命中结果
        - main [ref=e52]:
          - generic [ref=e53]:
            - generic [ref=e54]:
              - generic [ref=e55]:
                - heading "总览" [level=2] [ref=e56]
                - paragraph [ref=e57]: 账户聚合来自数据库，不从当前页推算；启用和自动应用不代表任务已实际命中。
              - button "刷新" [ref=e58] [cursor=pointer]
            - generic [ref=e59]:
              - article [ref=e60]:
                - generic [ref=e61]: 账户版本总数
                - strong [ref=e62]: "0"
              - article [ref=e63]:
                - generic [ref=e64]: 已启用版本
                - strong [ref=e65]: "0"
              - article [ref=e66]:
                - generic [ref=e67]: 已启用版本明确覆盖的算子
                - strong [ref=e68]: "0"
              - article [ref=e69]:
                - generic [ref=e70]: 开启自动应用的规则范围
                - strong [ref=e71]: "0"
            - generic [ref=e72]:
              - article [ref=e73]:
                - heading "已启用版本" [level=3] [ref=e74]
                - paragraph [ref=e75]: 仅表示允许被规则引用，不表示已作用于任务。
              - article [ref=e76]:
                - heading "自动应用范围" [level=3] [ref=e77]
                - paragraph [ref=e78]: 新任务仍需范围匹配及提交时校验，实际数值以任务详情为准。
            - article [ref=e79]:
              - generic [ref=e80]:
                - heading "开始一次校准" [level=3] [ref=e81]
                - paragraph [ref=e82]: 选择手工利用率，或导入具体硬件、模型和阶段的实测批次。
              - button "新建校准版本" [ref=e83] [cursor=pointer]
            - article [ref=e84]:
              - strong [ref=e85]: Profiling 可构建并验证
              - paragraph [ref=e86]: 可追加原始或规范 CSV/ZIP、查看 Shape 与 t0 对照；验证通过后再发布和启用。
    - dialog "新建校准版本" [ref=e88]:
      - generic [ref=e89]:
        - generic [ref=e90]:
          - heading "新建校准版本" [level=2] [ref=e91]
          - paragraph [ref=e92]: 校准资产仅自己可见，仅用于自己的任务。
        - button "关闭" [ref=e93] [cursor=pointer]
      - generic "校准来源" [ref=e94]:
        - button "手工填写 按具体算子填写利用率" [ref=e95] [cursor=pointer]:
          - strong [ref=e96]: 手工填写
          - generic [ref=e97]: 按具体算子填写利用率
        - button "导入 Profiling 当前支持训练所有已定义算子类型；先选择硬件和模型，再导入 CSV/ZIP 批次" [pressed] [ref=e98] [cursor=pointer]:
          - strong [ref=e99]: 导入 Profiling
          - generic [ref=e100]: 当前支持训练所有已定义算子类型；先选择硬件和模型，再导入 CSV/ZIP 批次
      - generic [ref=e101]:
        - generic [ref=e102]:
          - text: 版本名称
          - textbox "版本名称" [ref=e103]:
            - /placeholder: 例如：A3 BF16 算子校准
            - text: 原始失败回滚-1790719105262
        - generic [ref=e104]:
          - text: 阶段范围
          - combobox "阶段范围" [ref=e106]: train
        - generic [ref=e107]:
          - text: 硬件标识
          - combobox "硬件标识" [ref=e109]: H100_Server
        - generic [ref=e110]:
          - text: 模型范围
          - generic [ref=e111]:
            - combobox "模型范围 llama3-70b" [expanded] [active] [ref=e112]: llama3-70b
            - listbox [ref=e113]:
              - option "llama3-70b" [selected] [ref=e114]:
                - strong [ref=e115]: llama3-70b
      - generic [ref=e116]:
        - paragraph [ref=e117]: 流程：导入批次 → 检查数据质量 → 可选诊断预览 → 选择成功源任务并检查兼容性 → 构建正式候选 → 查看验证报告 → 发布启用。
        - paragraph [ref=e118]: 有效 0 行、无效 0 行；尚无可比较的系统基线，不能发布。
        - region "构建候选状态" [ref=e119]:
          - generic [ref=e121]:
            - heading "构建候选" [level=3] [ref=e122]
            - paragraph [ref=e123]: 状态：待构建
          - paragraph [ref=e124]: 需要本人已成功完成的源训练任务 ID。构建后按独立 Shape 留出与 t0 比较；仅通过正式验证的版本可发布。
          - generic [ref=e125]:
            - generic [ref=e126]:
              - text: 选择已完成的源训练任务
              - combobox "选择已完成的源训练任务" [ref=e127]:
                - option "选择任务" [selected]
            - generic [ref=e128]:
              - text: 或输入源训练任务 ID（预览可选）
              - textbox "或输入源训练任务 ID（预览可选）" [ref=e129]:
                - /placeholder: 本人已完成的评估任务
            - button "生成构建候选" [disabled] [ref=e130]
        - generic [ref=e132]:
          - heading "导入实测文件" [level=3] [ref=e133]
          - paragraph [ref=e134]: 每次导入保存独立采集来源；批次保存后可生成诊断候选，不影响任务。
        - generic [ref=e135]:
          - text: 导入 kernel_details.csv
          - button "导入 kernel_details.csv" [ref=e136]
        - paragraph [ref=e137]: 可执行构建支持训练已定义算子的受限 Shape、dtype 与布局组合。
        - group [ref=e138]:
          - generic "支持格式与限制" [ref=e139] [cursor=pointer]
        - strong [ref=e140]: 采集时实际并行策略
        - paragraph [ref=e141]: TP/DP/PP/EP/CP 必须与采集任务一致，构建时还会与源训练任务核对；下方默认 1 仅是输入初值，请逐项核实。
        - generic [ref=e142]:
          - generic [ref=e143]:
            - text: TP
            - spinbutton "TP" [ref=e144]: "1"
          - generic [ref=e145]:
            - text: DP
            - spinbutton "DP" [ref=e146]: "1"
          - generic [ref=e147]:
            - text: PP
            - spinbutton "PP" [ref=e148]: "1"
          - generic [ref=e149]:
            - text: EP
            - spinbutton "EP" [ref=e150]: "1"
          - generic [ref=e151]:
            - text: CP
            - spinbutton "CP" [ref=e152]: "1"
        - generic [ref=e153]:
          - checkbox "我已核对以上数值为本批次采集时的实际并行策略" [ref=e154]
          - text: 我已核对以上数值为本批次采集时的实际并行策略
        - group [ref=e155]:
          - generic "可选采集环境信息" [ref=e156] [cursor=pointer]
        - paragraph [ref=e157]: 文件限 20 MiB。每个转换后算子/Shape 组裁剪后至少 21 条有效采样；正式验证还需同组至少 5 个独立 Shape。原始记录通常需要更多行；解析失败会返回成员、行号和字段诊断。
      - generic [ref=e158]:
        - button "取消" [ref=e159] [cursor=pointer]
        - button "创建草稿并导入" [disabled] [ref=e160]
```

# Test source

```ts
  810  |   await expect(page.getByRole('dialog', { name: '版本详情' }).getByRole('button', { name: '发布' })).toHaveCount(0)
  811  |   await clickVersionAction(page, row, '管理草稿与批次')
  812  |   await expect(page.getByText('有效 1 / 总 1')).toBeVisible()
  813  |   // 批次载入即自动诊断，无需额外按钮；报告仍不是正式精度验证。
  814  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('输入准备检查不等于精度验证')
  815  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('缺少来源硬件或模型指纹')
  816  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('来源 TP 1')
  817  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('当前资产声明')
  818  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('未填写指纹')
  819  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('导入时已绑定选中资产')
  820  |   await expect(page.getByTestId('calibration-shape-fit-report')).toContainText('独立 Shape 少于 5 个')
  821  |   await expect(page.getByTestId('calibration-shape-fit-report')).toContainText('不能发布')
  822  |   await expect(page.getByTestId('calibration-shape-fit-report')).toContainText('不能证明真机采集来源')
  823  |   await page.getByTestId('calibration-source-task-id').fill('9999999')
  824  |   await expect(page.getByTestId('calibration-shape-fit-report')).toHaveCount(0)
  825  |   await page.getByTestId('calibration-source-task-id').press('Tab')
  826  |   await expect(page.getByTestId('calibration-source-task-error')).toContainText('源训练任务不存在或无权访问')
  827  |   await page.getByTestId('calibration-source-task-id').fill('')
  828  |   await page.getByTestId('calibration-profile-file').setInputFiles({
  829  |     name: 'MatMulV3.csv', mimeType: 'text/csv',
  830  |     buffer: Buffer.from(csv.toString().replace('12.5', '13.5')),
  831  |   })
  832  |   await page.getByTestId('calibration-source-strategy-confirmed').check()
  833  |   await page.getByTestId('calibration-version-save').click()
  834  |   await expect(page.getByText('有效 1 / 总 1')).toHaveCount(2)
  835  |   await expect(page.getByTestId('calibration-build-readiness-report')).toContainText('批次 2')
  836  |   await expect(page.getByTestId('calibration-shape-fit-report')).toContainText('批次 2')
  837  |   const downloadEvent = page.waitForEvent('download')
  838  |   await page.getByRole('button', { name: '下载原始文件' }).first().click()
  839  |   const download = await downloadEvent
  840  |   expect(download.suggestedFilename()).toBe('MatMulV3.csv')
  841  |   await page.getByRole('button', { name: '从草稿移除' }).first().click()
  842  |   await expect(page.getByText('有效 1 / 总 1')).toHaveCount(1)
  843  |   await page.getByRole('button', { name: '从草稿移除' }).click()
  844  |   await expect(page.getByText('有效 1 / 总 1')).toHaveCount(0)
  845  |   await page.getByRole('button', { name: '取消' }).click()
  846  |   await clickVersionAction(page, row, '删除')
  847  |   await acceptWorkbenchConfirmation(page)
  848  |   await expect(row).toHaveCount(0)
  849  | })
  850  | 
  851  | test('@L1 Profiling 导入明确格式与采集来源', async ({ page, catalogs }) => {
  852  |   // 观测点：可解析格式不等于可发布范围，默认并行策略未经用户确认不能上传。
  853  |   await page.goto('/zrt-sim/calibration')
  854  |   await page.getByTestId('calibration-create-open').click()
  855  |   await page.getByRole('button', { name: /导入 Profiling/ }).click()
  856  |   await page.getByTestId('calibration-version-name').fill(`E2E-来源说明-${Date.now()}`)
  857  |   await page.getByTestId('calibration-version-hardware').fill(catalogs.train.hardwareName)
  858  |   await page.getByTestId('calibration-version-model').fill(catalogs.train.modelId)
  859  |   await page.getByTestId('calibration-version-phase').fill('train')
  860  |   await expect(page.getByText('采集时实际并行策略')).toBeVisible()
  861  |   await page.getByText('可选采集环境信息').click()
  862  |   await expect(page.getByText(/CANN 版本与设备指纹是上传者的来源声明/)).toBeVisible()
  863  |   await expect(page.getByText(/首批可执行构建仅支持训练 MatMulV3/)).toBeVisible()
  864  |   await expect(page.getByTestId('calibration-profile-file')).toHaveAttribute('accept', '.csv,.zip')
  865  |   await page.getByTestId('calibration-profile-file').setInputFiles({
  866  |     name: 'kernel_details.csv', mimeType: 'text/csv', buffer: readFileSync(rawProfilingFixture),
  867  |   })
  868  |   await expect(page.getByTestId('calibration-version-save')).toBeDisabled()
  869  |   await page.getByTestId('calibration-source-strategy-confirmed').check()
  870  |   await expect(page.getByTestId('calibration-version-save')).toBeEnabled()
  871  | })
  872  | 
  873  | test('@L1 模拟补全的原始 kernel_details CSV 可导入并保留原件', async ({ page, catalogs }) => {
  874  |   const versionName = `E2E原始CSV-${Date.now()}`
  875  |   await page.goto('/zrt-sim/calibration')
  876  |   await page.getByTestId('calibration-create-open').click()
  877  |   await page.getByRole('button', { name: /导入 Profiling/ }).click()
  878  |   await page.getByTestId('calibration-version-name').fill(versionName)
  879  |   await page.getByTestId('calibration-version-hardware').fill(catalogs.train.hardwareName)
  880  |   await page.getByTestId('calibration-version-model').fill(catalogs.train.modelId)
  881  |   await page.getByTestId('calibration-profile-file').setInputFiles({
  882  |     name: 'kernel_details.csv', mimeType: 'text/csv', buffer: syntheticRawProfiling(),
  883  |   })
  884  |   await page.getByTestId('calibration-source-strategy-confirmed').check()
  885  |   await page.getByTestId('calibration-version-save').click()
  886  |   await expect(page.getByRole('dialog', { name: '新建校准版本' })).toBeVisible()
  887  |   await page.getByRole('button', { name: '关闭', exact: true }).click()
  888  |   await page.getByTestId('calibration-nav-versions').click()
  889  |   const row = page.locator('tbody tr').filter({ hasText: versionName })
  890  |   await expect(row).toContainText('Profiling 已导入 · 尚未生成诊断候选')
  891  |   await row.getByRole('button', { name: '查看/管理' }).click()
  892  |   await expect(page.getByRole('dialog', { name: '版本详情' }).getByRole('button', { name: '发布' })).toHaveCount(0)
  893  |   await clickVersionAction(page, row, '管理草稿与批次')
  894  |   await expect(page.getByText(/有效 6 \/ 总 11/)).toBeVisible()
  895  |   const downloadEvent = page.waitForEvent('download')
  896  |   await page.getByRole('button', { name: '下载原始文件' }).click()
  897  |   expect((await downloadEvent).suggestedFilename()).toBe('kernel_details.csv')
  898  | })
  899  | 
  900  | test('@L1 原始Profiling首次导入失败不遗留空草稿', async ({ page, catalogs }) => {
  901  |   // 原理：首次保存包含建版本和上传两步；观测点：无有效样本时可读提示且列表不留下空版本。
  902  |   const name = `原始失败回滚-${Date.now()}`
  903  |   await page.goto('/zrt-sim/calibration')
  904  |   await page.getByTestId('calibration-create-open').click()
  905  |   await page.getByRole('button', { name: /导入 Profiling/ }).click()
  906  |   await page.getByTestId('calibration-version-name').fill(name)
  907  |   await page.getByTestId('calibration-version-hardware').fill(catalogs.train.hardwareName)
  908  |   await page.getByTestId('calibration-version-model').fill(catalogs.train.modelId)
  909  |   await page.getByTestId('calibration-profile-file').setInputFiles({
> 910  |     name: 'kernel_details.csv', mimeType: 'text/csv', buffer: readFileSync(rawProfilingFixture),
       |                                                               ^ Error: ENOENT: no such file or directory, open '/home/administrator/actions-runner/_work/zrt-sim-ui/zrt-sim-ui/backend-repo/tests/calibration/fixtures/kernel_details.csv'
  911  |   })
  912  |   await page.getByTestId('calibration-source-strategy-confirmed').check()
  913  |   await page.getByTestId('calibration-version-save').click()
  914  |   await expect(page.getByRole('alert')).toBeVisible()
  915  |   await page.getByRole('button', { name: '取消', exact: true }).click()
  916  |   await page.getByTestId('calibration-nav-versions').click()
  917  |   await expect(page.locator('tbody tr').filter({ hasText: name })).toHaveCount(0)
  918  | })
  919  | 
  920  | test('@L1 旧草稿拟合响应不能污染新草稿报告', async ({ page, catalogs, testOwner }) => {
  921  |   // 观测点：两个相同 revision 的私有草稿切换时，A 的迟到响应不能落到 B 的弹窗。
  922  |   const backend = process.env.E2E_BACKEND_URL
  923  |   if (!backend) throw new Error('E2E_BACKEND_URL is required')
  924  |   const stamp = Date.now()
  925  |   const csv = Buffer.from(
  926  |     'op_type,op_name,op_state,tasktype,torch_input_params,input_shapes,input_data_types,input_formats,output_shapes,output_data_types,output_formats,task_duration_us,trimmed_sample_count\n'
  927  |     + 'MatMulV3,aclnnMatmul,dynamic,AI_CORE,"{""transpose_x1"": false, ""transpose_x2"": false}","8,16;16,4",DT_BF16;DT_BF16,ND;ND,"8,4",DT_BF16,ND,"{""mean"": 12.5}",21\n',
  928  |   )
  929  |   const headers = buildTestUserHeaders(testOwner)
  930  |   async function createDraft(name: string): Promise<string> {
  931  |     const created = await page.request.post(`${backend}/api/calibrations/versions`, {
  932  |       headers,
  933  |       data: {
  934  |         name, source_kind: 'profiling', hardware_id: catalogs.train.hardwareName,
  935  |         model_id: catalogs.train.modelId, phase: 'train',
  936  |         scope: { hardware: catalogs.train.hardwareName, model: catalogs.train.modelId, phase: 'train' },
  937  |       },
  938  |     })
  939  |     expect(created.ok()).toBeTruthy()
  940  |     const id = (await created.json()).id as string
  941  |     const imported = await page.request.post(
  942  |       `${backend}/api/calibrations/versions/${id}/batches?filename=MatMulV3.csv&request_key=capture&revision=1`,
  943  |       { headers, data: csv },
  944  |     )
  945  |     expect(imported.ok()).toBeTruthy()
  946  |     return id
  947  |   }
  948  |   const nameA = `拟合-A-${stamp}`
  949  |   const nameB = `拟合-B-${stamp}`
  950  |   const idA = await createDraft(nameA)
  951  |   await createDraft(nameB)
  952  |   let releaseOld: (() => void) | undefined
  953  |   let signalIntercept: (() => void) | undefined
  954  |   const intercepted = new Promise<void>(resolve => { signalIntercept = resolve })
  955  |   await page.route('**/shape-fit-preview', async route => {
  956  |     if (!route.request().url().includes(idA)) return route.continue()
  957  |     const response = await route.fetch()
  958  |     await new Promise<void>(resolve => {
  959  |       releaseOld = resolve
  960  |       signalIntercept?.()
  961  |     })
  962  |     await route.fulfill({ response })
  963  |   })
  964  |   await page.goto('/zrt-sim/calibration')
  965  |   await page.getByTestId('calibration-nav-versions').click()
  966  |   await clickVersionAction(page, page.locator('tbody tr').filter({ hasText: nameA }), '管理草稿与批次')
  967  |   await expect(page.getByText('有效 1 / 总 1')).toBeVisible()
  968  |   await intercepted
  969  |   await page.getByRole('button', { name: '取消' }).click()
  970  |   const detail = page.getByRole('dialog', { name: '版本详情' })
  971  |   await expect(detail).toBeVisible()
  972  |   await detail.getByRole('button', { name: '关闭详情' }).click()
  973  |   await expect(detail).toBeHidden()
  974  |   await clickVersionAction(page, page.locator('tbody tr').filter({ hasText: nameB }), '管理草稿与批次')
  975  |   await expect(page.getByText('有效 1 / 总 1')).toBeVisible()
  976  |   const oldResponse = page.waitForResponse(response => response.url().includes(idA)
  977  |     && response.url().includes('shape-fit-preview'))
  978  |   releaseOld?.()
  979  |   await oldResponse
  980  |   await expect(page.getByTestId('calibration-shape-fit-report')).toBeVisible()
  981  | })
  982  | 
  983  | test('@L1 用户手工校准工作台闭环', async ({ page, catalogs }) => {
  984  |   test.setTimeout(E2E_MULTI_TASK_TIMEOUT_MS)
  985  |   const versionName = `E2E手工校准-${Date.now()}`
  986  | 
  987  |   await page.goto('/zrt-sim/calibration')
  988  |   await expect(page.getByRole('heading', { name: '用户精度校准' })).toBeVisible()
  989  | 
  990  |   await page.getByTestId('calibration-create-open').click()
  991  |   await page.getByTestId('calibration-version-name').fill(versionName)
  992  |   await page.getByTestId('calibration-version-hardware').fill(catalogs.train.hardwareName)
  993  |   await page.getByTestId('calibration-version-model').fill(catalogs.train.modelId)
  994  |   await page.getByTestId('calibration-version-phase').fill('train')
  995  |   // 观测点：默认空算子必须明确提示如何选择整体利用率，不让用户误以为已经选中。
  996  |   await page.getByTestId('calibration-entry-add').click()
  997  |   await expect(page.getByRole('alert').filter({ hasText: '点击“全部算子”' })).toBeVisible()
  998  |   await page.getByTestId('calibration-entry-operator').fill('aten.mm.default')
  999  |   await page.getByTestId('calibration-entry-unit').selectOption('Cube')
  1000 |   await page.getByTestId('calibration-entry-dtype').fill('*')
  1001 |   await page.getByTestId('calibration-entry-utilization').fill('25')
  1002 |   await page.getByTestId('calibration-entry-add').click()
  1003 |   await page.getByTestId('calibration-version-save').click()
  1004 |   await page.getByTestId('calibration-nav-versions').click()
  1005 | 
  1006 |   const versionRow = page.locator('tbody tr').filter({ hasText: versionName })
  1007 |   await expect(versionRow).toBeVisible()
  1008 |   await clickVersionAction(page, versionRow, '编辑')
  1009 |   await page.getByTestId('calibration-saved-entry-utilization').fill('30')
  1010 |   await page.getByTestId('calibration-version-save').click()
```