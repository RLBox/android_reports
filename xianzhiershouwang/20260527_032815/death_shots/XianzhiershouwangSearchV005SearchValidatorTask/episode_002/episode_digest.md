# Episode 2 — ✅ passed (7 steps)

> **Goal**: 【当前账户档案】账号：zhangsan@example.com；昵称：张三；默认收货地址（JSON）：{"recipient": "张三", "phone": "13800138000", "address": "上海市 上海市 浦东新区 陆家嘴环路1000号"}。请基于以上档案打开 com.xianzhiershouwang 并完成以下任务：搜一下羽毛球拍，找到那个YONEX天斧88D的帮我收藏

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xianzhiershouwang | 当前桌面未找到指定应用，我将按要求打开它。接下来我将直接调用应用启动工具，打开对应包名的目标应用。 |
| 2 | click (378, 146) | 闲鱼已打开，将搜索YONEX天斧88D并收藏。接下来将点击顶部搜索框，准备输入羽毛球拍。 |
| 3 | input_text "羽毛球拍" | 搜索框已激活，我将输入羽毛球拍搜索。输入羽毛球拍。 |
| 4 | keyboard_enter | 已输入“羽毛球拍”，将按回车搜索查找指定商品。提交搜索。 |
| 5 | click (279, 900) | 目标羽毛球拍商品已经找到，接下来将进入详情页收藏。进入详情页。 |
| 6 | click (233, 2234) | 商品详情页已打开，底部有收藏按钮，点击星星图标完成收藏。点击收藏按钮。 |
| 7 | answer "已在闲鱼（com.xianzhiershouwang）中搜索羽毛球拍，并找..." | 闲鱼收藏任务已全部完成，可提交确认。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | 有「羽毛球拍」搜索记录 | ✅ | 20 | – |
| 2 | 搜索词包含羽毛球 | ✅ | 10 | – |
| 3 | 张三收藏了「尤尼克斯羽毛球拍 天斧88D」 | ✅ | 35 | – |
| 4 | 收藏的是尤尼克斯帖子 | ✅ | 35 | – |
