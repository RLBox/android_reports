# group_v001_invite_friend  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangGroupV001InviteFriendTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 1730s (~28.8 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangGroupV001InviteFriendTask.log](./raw_logs/XingqiushejiaowangGroupV001InviteFriendTask.log)
- **Generated**: 2026-06-05T00:38:18+08:00

## Task Goal

> 【当前账户档案】账号：demo@rlbox.ai；昵称：张小星；支付密码：123456，如需支付请使用此密码完成支付。请基于以上档案打开 com.xingqiushejiaowang 并完成以下任务：关注柚子汽水很久了，先打个招呼，再拉她进我的「周末桌游搭子」群

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | ⏰ timeout | 80 | max_steps | task 'XingqiushejiaowangGroupV001InviteFriendTask' was not initialized; current initialized task is 'XianzhiershouwangOrderV020OrderValid... | 2026-06-04 19:29:37 → 2026-06-04 19:41:52 |
| 2 | 💥 error | 0 | exception | exception: 404 Not Found for url: http://localhost:6800/step \\| detail: No available devices found | 2026-06-04 19:41:52 → 2026-06-04 19:44:04 |
| 3 | ⏰ timeout | 80 | max_steps | task 'XingqiushejiaowangGroupV001InviteFriendTask' was not initialized; current initialized task is 'XianzhiershouwangOrderV022OrderValid... | 2026-06-04 19:44:28 → 2026-06-04 19:58:27 |

## Failure Details

### Episode 1 — ⏰ timeout

- steps_used: `80`
- terminated_reason: `max_steps`
- reason:

  ```
  task 'XingqiushejiaowangGroupV001InviteFriendTask' was not initialized; current initialized task is 'XianzhiershouwangOrderV020OrderValidatorTask'
  ```
- death shot: ![last-step](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_001/step_080.png)
  - state: [`./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_001/step_080.json`](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_001/step_080.json)
  - digest: [`episode_digest.md`](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_001/episode_digest.md)

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 404 Not Found for url: http://localhost:6800/step | detail: No available devices found
  ```
- death shot: ![last-step](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_002/step_015.png)
  - state: [`./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_002/step_015.json`](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_002/step_015.json)
  - digest: [`episode_digest.md`](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_002/episode_digest.md)

### Episode 3 — ⏰ timeout

- steps_used: `80`
- terminated_reason: `max_steps`
- reason:

  ```
  task 'XingqiushejiaowangGroupV001InviteFriendTask' was not initialized; current initialized task is 'XianzhiershouwangOrderV022OrderValidatorTask'
  ```
- death shot: ![last-step](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_003/step_080.png)
  - state: [`./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_003/step_080.json`](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_003/step_080.json)
  - digest: [`episode_digest.md`](./death_shots/XingqiushejiaowangGroupV001InviteFriendTask/episode_003/episode_digest.md)

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
