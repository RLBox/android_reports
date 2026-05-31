# Episode 1 — ✅ passed (8 steps)

> **Goal**: 【当前账户档案】账号：demo@rlbox.ai；昵称：张小星；支付密码：无需密码，如需支付直接确认即可。请基于以上档案打开 com.xingqiushejiaowang 并完成以下任务：陶陶发的动态我都不想错过，帮我设成特别关心

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xingqiushejiaowang | 我将启动指定的目标应用。我将调用打开应用的操作，启动目标应用，后续找到陶陶设置特别关心。 |
| 2 | click (923, 122) | 已进入星球社交广场，将搜索陶陶。点击右上角搜索按钮后，我将输入“陶陶”查找用户。 |
| 3 | input_text "陶陶" | 在已激活的搜索框中，我将输入“陶陶”查找用户。 |
| 4 | click (1001, 161) | 已输入关键词“陶陶”，将点击搜索按钮执行搜索。 |
| 5 | click (239, 545) | 已找到目标用户，将点击进入其主页。 |
| 6 | click (1005, 264) | 在陶陶个人主页，我将点击右上角更多按钮设特别关心。接下来点击右上角图标。 |
| 7 | click (261, 1704) | 用户设置弹窗里有“特别关心”选项，点击该选项即可完成设置。接下来点击“特别关心”选项。 |
| 8 | answer "已成功将陶陶设置为特别关心，你不会错过陶陶发的动态啦。任务完成。" | 已完成特别关心设置，可提交任务。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | session 内存在 demo → tao 的 Follow 副本 | ✅ | 40 | – |
| 2 | Follow.active = true | ✅ | 20 | – |
| 3 | Follow.status = special_care | ✅ | 40 | – |
