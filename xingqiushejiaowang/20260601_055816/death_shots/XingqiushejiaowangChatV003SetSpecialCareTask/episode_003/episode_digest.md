# Episode 3 — ✅ passed (8 steps)

> **Goal**: 【当前账户档案】账号：demo@rlbox.ai；昵称：张小星；支付密码：无需密码，如需支付直接确认即可。请基于以上档案打开 com.xingqiushejiaowang 并完成以下任务：陶陶发的动态我都不想错过，帮我设成特别关心

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xingqiushejiaowang | 我将先打开目标应用，设置陶陶为特别关心。我将打开对应包名的星球社交网应用。 |
| 2 | click (929, 122) | 已进入星球社交网广场页，将点击搜索查找陶陶账号。点击搜索按钮。 |
| 3 | input_text "陶陶" | 在搜索框输入“陶陶”。 |
| 4 | click (1005, 161) | 已输入“陶陶”，将点击搜索查找用户。 |
| 5 | click (239, 545) | 已找到目标用户，将点击进入其主页。 |
| 6 | click (1005, 264) | 在陶陶个人主页，我将点击右上角更多按钮设置特别关心。 |
| 7 | click (261, 1704) | 点击特别关心完成设置，关注陶陶动态。 |
| 8 | answer "已成功将陶陶设置为特别关心，你不会错过陶陶发的任何动态啦。" | 已将陶陶设为特别关心，操作成功。  全流程操作顺利，我将提交任务结果。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | session 内存在 demo → tao 的 Follow 副本 | ✅ | 40 | – |
| 2 | Follow.active = true | ✅ | 20 | – |
| 3 | Follow.status = special_care | ✅ | 40 | – |
