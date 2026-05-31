# Episode 1 — ✅ passed (6 steps)

> **Goal**: 【当前账户档案】账号：demo@rlbox.ai；昵称：张小星；支付密码：无需密码，如需支付直接确认即可。请基于以上档案打开 com.xingqiushejiaowang 并完成以下任务：看到 yuzi_soda 的主页挺有趣，想关注一下

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.xingqiushejiaowang | 我需要打开指定的星球社交类应用，接下来将执行启动操作。 |
| 2 | click (929, 122) | 已经进入社交应用广场页，接下来将点击搜索图标查找目标用户。点击搜索按钮。 |
| 3 | click (297, 857) | 点击热搜上的yuzi_soda条目，即可快速找到对应主页。点击该选项。 |
| 4 | click (324, 552) | 已找到目标用户，有关注按钮。结合用户反馈的情况，我将先点击目标用户的用户名进入其主页，再完成关注操作。 |
| 5 | click (157, 2244) | 已进入目标主页，接下来将点击关注按钮完成关注。 |
| 6 | answer "已成功在com.xingqiushejiaowang应用中关注用户yuzi..." | 已成功关注目标用户主页。关注操作已完成，任务可提交。 |

## Result

- **Terminated**: answer

## Validator Response

| # | Check | Passed | Weight | Detail |
|---|-------|--------|--------|--------|
| 1 | session 内存在 demo → yuzi 的 Follow 记录 | ✅ | 60 | – |
| 2 | Follow.active = true | ✅ | 20 | – |
| 3 | baseline 中不存在该关注（这是新关注） | ✅ | 20 | – |
