# Episode 2 — ✅ passed (8 steps)

> **Goal**: 【当前账户档案】账号：demo@rlbox.ai；昵称：张小星；支付密码：无需密码，如需支付直接确认即可。请基于以上档案打开 com.xingqiushejiaowang 并完成以下任务：陶陶发的动态我都不想错过，帮我设成特别关心

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xingqiushejiaowang | 为将陶陶设为特别关心，我将先打开目标应用。目标星球社交类应用将由我直接调用工具打开。 |
| 2 | click (918, 122) | 已进入社交广场页，将搜索陶陶。点击右上角搜索按钮后，我将输入“陶陶”查找用户。 |
| 3 | input_text "陶陶" | 搜索框已激活，我将输入“陶陶”查找用户。 |
| 4 | click (1004, 161) | 已输入关键词“陶陶”，将点击搜索按钮。 |
| 5 | click (243, 545) | 已找到目标用户，将点击进入其个人主页。 |
| 6 | click (1012, 264) | 接下来我将点击主页右上角更多按钮，设置特别关心。 |
| 7 | click (265, 1704) | 点击“特别关心”选项完成设置的操作，我即将执行。 |
| 8 | answer "已成功将陶陶设为特别关心，后续你不会错过陶陶发布的动态啦。任务完成。" | 已确认陶陶设为特别关心，任务完成。全部操作已顺利完成，可提交任务。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | session 内存在 demo → tao 的 Follow 副本 | ✅ | 40 | – |
| 2 | Follow.active = true | ✅ | 20 | – |
| 3 | Follow.status = special_care | ✅ | 40 | – |
