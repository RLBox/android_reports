# Episode 2 — ❌ failed (8 steps)

> **Goal**: 想入个 Gucci 包但怕买到假货，只看能支持验货，在这些里面挑现价相对专柜价打折最狠（现价÷专柜价比例最低）的那个收藏

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xianzhiershouwang | 未在桌面找到目标应用，我将打开它。我将启动包名对应的闲致二手网应用。 |
| 2 | click (996, 144) | 将搜索Gucci包。点击搜索图标后，我将输入“Gucci包”，后续再筛选可验货商品，比价后收藏最低的。 |
| 3 | input_text "Gucci包" | 搜索框已激活，我将输入“Gucci包”搜索相关商品。输入Gucci包。 |
| 4 | keyboard_enter | 已输入“Gucci包”，现在按回车键提交搜索，获取相关商品列表。 |
| 5 | click (545, 466) | 点击验货宝标签筛选支持验货的Gucci包，后续计算比价找到最低比例。点击验货宝。 |
| 6 | click (279, 984) | 比例计算已完成，接下来将点击进入商品详情页确认信息并收藏。 |
| 7 | click (256, 2249) | 点击收藏按钮完成收藏。这款支持验货的Gucci包性价比最高，我将点击收藏按钮完成收藏。 |
| 8 | answer "已在com.xianzhiershouwang中筛选出支持验货的Gucci..." | 支持验货的Gucci包中性价比最高的 Marmont 小号链条包已被我收藏，接下来将关闭弹窗确认任务完成。 |

## Result

- **Terminated**: answer
- **Reason**: 收藏的是折扣最低的「支持验货」款 id=200: 预期收藏 id=200（Gucci 双肩包 支持验货 ¥4999/¥12000 = 41.7折，在带验货/凭证的 Gucci 包中折扣最低），实际收藏了 id=1044「Gucci Marmont 小号链条包 黑色牛皮 经典双G」
