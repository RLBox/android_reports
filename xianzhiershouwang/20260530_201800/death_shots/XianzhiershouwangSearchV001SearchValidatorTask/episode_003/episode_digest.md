# Episode 3 — ✅ passed (8 steps)

> **Goal**: 【当前账户档案】账号：zhangsan@example.com；昵称：张三；支付密码：无需密码，如需支付直接确认即可；默认收货地址（JSON）：{"recipient": "张三", "phone": "13800138000", "address": "上海市 上海市 浦东新区 陆家嘴环路1000号"}。请基于以上档案打开 com.xianzhiershouwang 并完成以下任务：搜一下耳机，帮我收藏最便宜的那个

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xianzhiershouwang | 启动指定应用后，我将搜索耳机并收藏最便宜的商品。接下来将由我调用启动工具打开目标应用。 |
| 2 | click (379, 144) | 已打开应用，将激活搜索框输入耳机。点击搜索栏输入耳机。 |
| 3 | input_text "耳机" | 搜索框已激活，我将输入“耳机”搜索。 |
| 4 | keyboard_enter | 已填耳机关键词，将执行搜索找低价商品。将按下回车键提交搜索。 |
| 5 | click (270, 360) | 接下来将由我按价格升序找最便宜的耳机。 |
| 6 | click (270, 840) | 当前最便宜的耳机为漫步者TWS NB2 Pro，售价99元。接下来点击该商品卡片进入详情页收藏。 |
| 7 | click (234, 2232) | 已进入最便宜耳机的详情页，将点击底部星星图标完成收藏。 |
| 8 | answer "已为你在闲鱼（com.xianzhiershouwang）中搜索耳机，找到..." | 已完成全部搜索收藏任务，可提交结果。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | 搜索了「耳机」 | ✅ | 25 | – |
| 2 | 有收藏记录 | ✅ | 35 | – |
| 3 | 收藏的是价格最低的耳机帖子 | ✅ | 40 | – |
