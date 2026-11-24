# Instructions

- Following Playwright test failed.
- Explain why, be concise, respect Playwright best practices.
- Provide a snippet of code with the fix, if possible.

# Test info

- Name: l1/assets/asset-lifecycle.spec.ts >> @L1 operators 真实接口按 ID 维护并保留原始规格
- Location: e2e/specs/l1/assets/asset-lifecycle.spec.ts:141:3

# Error details

```
TimeoutError: locator.click: Timeout 15000ms exceeded.
Call log:
  - waiting for getByRole('row').filter({ has: getByText('e2e_asset_operators_1795477198781', { exact: true }) }).getByRole('button', { name: '设为内置', exact: true })

```

# Page snapshot

```yaml
- generic [ref=e3]:
  - banner [ref=e4]:
    - generic [ref=e5]: ZRT
    - generic [ref=e6]: AI负载建模仿真平台
    - navigation "主要导航" [ref=e7]:
      - link "返回主页" [ref=e8] [cursor=pointer]:
        - /url: /zrt-sim/
      - link "任务管理" [ref=e9] [cursor=pointer]:
        - /url: /zrt-sim/tasks
      - link "资产管理" [ref=e10] [cursor=pointer]:
        - /url: /zrt-sim/assets
      - link "信息统计" [ref=e11] [cursor=pointer]:
        - /url: /zrt-sim/statistics
      - link "用户手册" [ref=e12] [cursor=pointer]:
        - /url: /zrt-sim/user-manual
    - generic [ref=e13]:
      - group [ref=e14]:
        - generic "工具与管理" [ref=e15] [cursor=pointer]:
          - text: 工具与管理
          - generic [ref=e16]: ⌄
      - button "切换至深色模式" [ref=e17] [cursor=pointer]:
        - img [ref=e18]
      - group [ref=e20]:
        - generic "个人菜单" [ref=e21] [cursor=pointer]:
          - generic [ref=e22]: E
          - generic [ref=e23]: E2E Admin
          - generic [ref=e24]: ⌄
      - generic [ref=e27]: Idle
  - main [ref=e28]:
    - generic [ref=e29]:
      - link "ZRT" [ref=e30] [cursor=pointer]:
        - /url: /zrt-sim/
      - generic [ref=e31]: /
      - link "资产管理" [ref=e32] [cursor=pointer]:
        - /url: /zrt-sim/assets
      - generic [ref=e33]: /
      - generic [ref=e34]: 算子管理
    - generic [ref=e36]:
      - heading "资产管理" [level=1] [ref=e37]
      - paragraph [ref=e38]: 模型 · 算子 · Module · 硬件资产的全生命周期管理
    - generic [ref=e39]:
      - complementary [ref=e40]:
        - button "模型管理" [ref=e41] [cursor=pointer]
        - button "算子管理" [ref=e42] [cursor=pointer]
        - button "Module管理" [ref=e43] [cursor=pointer]
        - button "硬件管理" [ref=e44] [cursor=pointer]
      - generic [ref=e47]:
        - generic [ref=e48]:
          - generic [ref=e49]:
            - generic [ref=e50]: Operator Assets
            - heading "算子管理" [level=1] [ref=e51]
          - generic [ref=e53]:
            - generic [ref=e54]:
              - strong [ref=e55]: "106"
              - text: 全部算子
            - generic [ref=e56]:
              - strong [ref=e57]: "1"
              - text: 自定义
            - generic [ref=e58]:
              - strong [ref=e59]: "105"
              - text: 内置资产
        - generic [ref=e61]:
          - generic [ref=e62]:
            - strong [ref=e64]: 算子列表
            - button "新增算子" [ref=e65] [cursor=pointer]
            - button "批量删除" [disabled] [ref=e66]
          - search "表格搜索" [ref=e67]:
            - generic [ref=e68]:
              - generic [ref=e69]:
                - generic [ref=e70]: 场景
                - combobox "场景" [ref=e71] [cursor=pointer]:
                  - option "全部" [selected]
                  - option "推理"
                  - option "训练"
                  - option "推荐"
              - generic [ref=e73]:
                - generic [ref=e74]: 来源
                - combobox "来源" [ref=e75] [cursor=pointer]:
                  - option "全部" [selected]
                  - option "内置算子"
                  - option "自定义算子"
              - generic [ref=e77]:
                - generic [ref=e78]: 分类
                - combobox "分类" [ref=e79] [cursor=pointer]:
                  - option "全部" [selected]
                  - option "Activation"
                  - option "Attention"
                  - option "Communication"
                  - option "Elementwise"
                  - option "Embedding"
                  - option "Flow"
                  - option "Linear"
                  - option "LinearAttention"
                  - option "MHC"
                  - option "MLA"
                  - option "MoE"
                  - option "Normalization"
                  - option "Position"
                  - option "Quantization"
                  - option "Torch"
                  - option "custom"
                  - option "vision"
              - generic [ref=e80]:
                - searchbox "搜索全部表格字段" [active] [ref=e81]: e2e_asset_operators_1795477198781
                - button "更多筛选" [ref=e82] [cursor=pointer]:
                  - text: 更多筛选
                  - img [ref=e83]
                - button "重置条件" [ref=e85] [cursor=pointer]
                - button "刷新列表" [ref=e86] [cursor=pointer]:
                  - generic [ref=e87]: ↻
            - generic "已选查询条件" [ref=e88]:
              - generic [ref=e89]: 已选条件
              - button "移除关键词条件" [ref=e90] [cursor=pointer]:
                - generic [ref=e91]: 关键词：e2e_asset_operators_1795477198781
                - generic [ref=e92]: ×
          - table [ref=e94]:
            - rowgroup [ref=e104]:
              - row "算子名称 分类 场景 来源 创建人 创建时间 操作" [ref=e105]:
                - columnheader [ref=e106]:
                  - checkbox [ref=e107]
                - columnheader "算子名称" [ref=e109]: 算子名称
                - columnheader "分类" [ref=e111]: 分类
                - columnheader "场景" [ref=e113]: 场景
                - columnheader "来源" [ref=e115]: 来源
                - columnheader "创建人" [ref=e117]: 创建人
                - columnheader "创建时间" [ref=e119]: 创建时间
                - columnheader "操作" [ref=e121]
            - rowgroup [ref=e122]:
              - row "e2e_asset_operators_1795477198781 custom 推理 自定义算子 e2e-admin(E2E Admin) 2026-11-24 07:39 编辑 拷贝 详情 删除" [ref=e123]:
                - cell [ref=e124]:
                  - checkbox [ref=e125]
                - cell "e2e_asset_operators_1795477198781" [ref=e126]:
                  - generic "e2e_asset_operators_1795477198781" [ref=e127]
                - cell "custom" [ref=e128]
                - cell "推理" [ref=e129]:
                  - generic [ref=e130]: 推理
                - cell "自定义算子" [ref=e131]:
                  - generic [ref=e132]: 自定义算子
                - cell "e2e-admin(E2E Admin)" [ref=e133]
                - cell "2026-11-24 07:39" [ref=e134]
                - cell "编辑 拷贝 详情 删除" [ref=e135]:
                  - generic [ref=e136]:
                    - button "编辑" [ref=e137] [cursor=pointer]
                    - button "拷贝" [ref=e138] [cursor=pointer]
                    - button "详情" [ref=e139] [cursor=pointer]
                    - button "删除" [ref=e140] [cursor=pointer]
          - generic [ref=e141]:
            - generic [ref=e142]: 共 1 条
            - combobox [ref=e143] [cursor=pointer]:
              - option "10条/页" [selected]
              - option "20条/页"
              - option "50条/页"
            - button "上一页" [disabled] [ref=e144]
            - button "1" [ref=e145] [cursor=pointer]
            - button "下一页" [disabled] [ref=e146]
```

# Test source

```ts
  71  |     const row = page.getByRole('row').filter({ hasText: asset.name })
  72  |     const confirmation = page.getByRole('alertdialog')
  73  |     await expect(row.locator('.source-builtin')).toBeVisible()
  74  |     await row.getByRole('button', { name: '编辑', exact: true }).click()
  75  |     const editor = page.getByRole('dialog')
  76  |     const input = editor.getByLabel('原始规格')
  77  |     await expect(input).toBeVisible()
  78  |     expect(parse(await input.inputValue())).toEqual(spec)
  79  |     await expect(editor).toContainText('下次启动同步会按配置文件更新规格')
  80  |     if (asset.collection === 'models') await expect(editor).toContainText('保存时保留原规格中未提交的顶层字段')
  81  |     await expect(page.locator('html')).toHaveAttribute('data-theme', 'dark')
  82  |     await expect(input).not.toHaveCSS('background-color', 'rgb(255, 255, 255)')
  83  | 
  84  |     await input.fill(JSON.stringify({ ...spec, name: 'unexpected-rename' }))
  85  |     await editor.getByRole('button', { name: '保存', exact: true }).click()
  86  |     await expect(editor.getByRole('alert')).toHaveText(/资产名称为只读/)
  87  |     expect(changes).toHaveLength(0)
  88  | 
  89  |     const edited = { ...spec, user_added_key: { keep: true } }
  90  |     await input.fill(JSON.stringify(edited))
  91  |     await editor.getByRole('button', { name: '保存', exact: true }).click()
  92  |     await confirmation.getByRole('button', { name: '取消', exact: true }).click()
  93  |     await expect(input).toHaveValue(JSON.stringify(edited))
  94  |     expect(changes).toHaveLength(0)
  95  |     await editor.getByRole('button', { name: '保存', exact: true }).click()
  96  |     await confirmation.getByRole('button', { name: '确认保存', exact: true }).click()
  97  |     await expect(confirmation).toHaveCount(0)
  98  |     expect(changes[0]).toEqual({ method: 'POST', path: `${base}/811/versions`, body: { name: asset.name, spec_json: edited } })
  99  | 
  100 |     await row.getByRole('button', { name: '转为非内置', exact: true }).click()
  101 |     await expect(confirmation).toContainText('下次启动同步会恢复为内置资产')
  102 |     await confirmation.getByRole('button', { name: '转为非内置', exact: true }).click()
  103 |     await expect(row.locator('.source-custom')).toBeVisible()
  104 |     await row.getByRole('button', { name: '设为内置', exact: true }).click()
  105 |     await confirmation.getByRole('button', { name: '设为内置', exact: true }).click()
  106 |     await expect(row.locator('.source-builtin')).toBeVisible()
  107 | 
  108 |     await row.getByRole('button', { name: '删除', exact: true }).click()
  109 |     await expect(confirmation).toContainText('下次启动同步会恢复为内置资产')
  110 |     await confirmation.getByRole('button', { name: '删除', exact: true }).click()
  111 |     await expect(row).toHaveCount(0)
  112 |     expect(changes.map(({ method, path }) => [method, path])).toEqual([
  113 |       ['POST', `${base}/811/versions`], ['POST', `${base}/811/demote-from-builtin`],
  114 |       ['POST', `${base}/811/promote-to-builtin`], ['DELETE', `${base}/811`],
  115 |     ])
  116 |   })
  117 | }
  118 | 
  119 | test('@L1 普通用户无内置资产生命周期入口，仍可创建模型副本', async ({ page }) => {
  120 |   for (const asset of assets) {
  121 |     const { changes, reads } = await mockLifecycle(page, asset, false)
  122 |     await page.goto(`/zrt-sim/assets?section=${asset.section}`)
  123 |     const row = page.getByRole('row').filter({ hasText: asset.name })
  124 |     await expect(row.getByRole('button', { name: /^(设为内置|转为非内置)$/ })).toHaveCount(0)
  125 |     await expect(row.getByRole('button', { name: '删除', exact: true })).toBeDisabled()
  126 |     const edit = row.getByRole('button', { name: '编辑', exact: true })
  127 |     if (asset.collection === 'models') {
  128 |       await expect(edit).toHaveAttribute('title', '编辑副本')
  129 |       await edit.click()
  130 |       await page.waitForURL(url => url.pathname.endsWith('manual-model.html') && url.searchParams.get('mode') === 'copy')
  131 |     } else {
  132 |       await expect(edit).toBeDisabled()
  133 |     }
  134 |     expect(changes).toHaveLength(0)
  135 |     expect(reads()).toBe(0)
  136 |     await page.unroute('**/zrt-sim-server/api/**')
  137 |   }
  138 | })
  139 | 
  140 | for (const asset of assets) {
  141 |   adminTest(`@L1 ${asset.collection} 真实接口按 ID 维护并保留原始规格`, async ({ page, testOwner }) => {
  142 |     const name = `e2e_asset_${asset.collection}_${Date.now()}`
  143 |     const initial = { name, custom_extension: { units: 'GiB', values: [1, null, 'literal'] } }
  144 |     const storedSpec = asset.collection === 'modules' ? [initial] : initial
  145 |     const modified = { ...initial, added_extension: { retained: true } }
  146 |     const nextSpec = asset.collection === 'modules' ? [modified] : modified
  147 |     const endpoint = `/zrt-sim-server/api/assets/${asset.collection}`
  148 |     const headers = buildTestUserHeaders(testOwner)
  149 |     const created = await page.request.post(endpoint, {
  150 |       headers,
  151 |       data: {
  152 |         name, domain: asset.domain, spec_format: asset.format, spec_json: initial,
  153 |         ...(asset.collection === 'modules' ? { module_kind: 'custom' } : {}),
  154 |       },
  155 |     })
  156 |     expect(created.status(), await created.text()).toBe(200)
  157 |     const persisted = await created.json()
  158 |     const assetPath = `${endpoint}/${persisted.id}`
  159 |     let archived = false
  160 |     try {
  161 |       if (asset.collection === 'modules') {
  162 |         const legacy = await page.request.post(`${assetPath}/versions`, { headers, data: { name, spec_json: storedSpec } })
  163 |         expect(legacy.status(), await legacy.text()).toBe(200)
  164 |       }
  165 |       await page.goto(`/zrt-sim/assets?section=${asset.section}`)
  166 |       const search = page.getByTestId('table-search')
  167 |       await search.fill(name)
  168 |       await search.press('Enter')
  169 |       const row = page.getByRole('row').filter({ has: page.getByText(name, { exact: true }) })
  170 |       const confirmation = page.getByRole('alertdialog')
> 171 |       await row.getByRole('button', { name: '设为内置', exact: true }).click()
      |                                                                    ^ TimeoutError: locator.click: Timeout 15000ms exceeded.
  172 |       await confirmation.getByRole('button', { name: '设为内置', exact: true }).click()
  173 |       await expect(row.locator('.source-builtin')).toBeVisible()
  174 | 
  175 |       await row.getByRole('button', { name: '编辑', exact: true }).click()
  176 |       const editor = page.getByRole('dialog')
  177 |       const input = editor.getByLabel('原始规格')
  178 |       expect(parse(await input.inputValue())).toEqual(storedSpec)
  179 |       const submitted = asset.collection === 'models' ? { name, added_extension: modified.added_extension } : nextSpec
  180 |       await input.fill(JSON.stringify(submitted))
  181 |       await editor.getByRole('button', { name: '保存', exact: true }).click()
  182 |       const saving = page.waitForResponse(response => response.url().endsWith(`${assetPath}/versions`) && response.request().method() === 'POST')
  183 |       await confirmation.getByRole('button', { name: '确认保存', exact: true }).click()
  184 |       const saved = await saving
  185 |       expect(saved.status(), await saved.text()).toBe(200)
  186 |       const updated = await saved.json()
  187 |       expect(updated).toMatchObject({
  188 |         id: persisted.id, owner: testOwner.account, builtin: 1, visibility: 'public', spec_format: asset.format, spec_json: nextSpec,
  189 |       })
  190 |       if (asset.collection === 'operators') {
  191 |         expect(updated).toMatchObject({ op_type: persisted.op_type, category: persisted.category })
  192 |       }
  193 |       if (asset.collection === 'modules') expect(updated.module_kind).toBe('custom')
  194 |       await expect(confirmation).toHaveCount(0)
  195 | 
  196 |       await row.getByRole('button', { name: '转为非内置', exact: true }).click()
  197 |       await confirmation.getByRole('button', { name: '转为非内置', exact: true }).click()
  198 |       await expect(row.locator('.source-custom')).toBeVisible()
  199 |       const read = await page.request.get(`${assetPath}/edit-spec`, { headers })
  200 |       expect(await read.json()).toMatchObject({ id: persisted.id, owner: testOwner.account, builtin: 0, spec_json: nextSpec })
  201 | 
  202 |       await row.getByRole('button', { name: '删除', exact: true }).click()
  203 |       const deleting = page.waitForResponse(response => response.url().endsWith(assetPath) && response.request().method() === 'DELETE')
  204 |       await confirmation.getByRole('button', { name: '删除', exact: true }).click()
  205 |       const deleted = await deleting
  206 |       expect(deleted.status(), await deleted.text()).toBe(200)
  207 |       expect((await deleted.json()).archived_at).toBeTruthy()
  208 |       await expect(row).toHaveCount(0)
  209 |       archived = true
  210 |     } finally {
  211 |       if (!archived) await page.request.delete(assetPath, { headers })
  212 |     }
  213 |   })
  214 | }
  215 | 
```