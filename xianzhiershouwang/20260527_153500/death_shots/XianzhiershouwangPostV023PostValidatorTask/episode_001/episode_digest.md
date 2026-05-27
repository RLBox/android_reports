# Episode 1 — ✅ passed (8 steps)

> **Goal**: 【当前账户档案】账号：zhangsan@example.com；昵称：张三；支付密码：无需密码，直接完成支付；默认收货地址（JSON）：{"recipient": "张三", "phone": "13800138000", "address": "上海市 上海市 浦东新区 陆家嘴环路1000号"}。请基于以上档案打开 com.xianzhiershouwang 并完成以下任务：我发的Switch OLED帖子开个10%折扣优惠吧

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xianzhiershouwang | 需要我先打开指定的闲至二手网应用，之后再处理Switch OLED帖子的折扣事宜。 |
| 2 | click (961, 2237) | 已进入闲至二手网主界面，下一步点击右下角「我的」进入个人中心。 |
| 3 | click (162, 1068) | 点击“我发布的”选项后，我将找到对应帖子设置10%折扣。点击对应按钮。 |
| 4 | drag | 已找到Switch OLED的相关帖子，接下来将滑动页面调出完整操作栏查找折扣设置入口。 |
| 5 | click (567, 1375) | Switch OLED帖子有折扣入口。接下来我将点击该按钮进入界面设置10%折扣。 |
| 6 | click (529, 948) | 当前已选中10%折扣，下一步将开启折扣。点击10%选项。 |
| 7 | click (842, 1092) | 已选10%折扣比例，折后价1305元，点击按钮即可完成设置。点击右侧黄色按钮开启折扣。 |
| 8 | answer "已为你在闲至二手网中给你发布的Switch OLED帖子设置了10%的折扣..." | 任务完成，Switch OLED帖子设10%折扣，折后1305元。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | 帖子折扣已设置（不再是0%） | ✅ | 40 | – |
| 2 | 折扣比例为10% | ✅ | 35 | – |
| 3 | 帖子仍为已发布状态 | ✅ | 25 | – |
