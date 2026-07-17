# matching_v005_buy_card_adventure_match  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangMatchingV005BuyCardAdventureMatchTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 68s (~1.1 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangMatchingV005BuyCardAdventureMatchTask.log](./raw_logs/XingqiushejiaowangMatchingV005BuyCardAdventureMatchTask.log)
- **Generated**: 2026-07-17T07:44:23+08:00

## Task Goal

> 晚上没事干，买张奇遇铃在线卡（匹配此刻在线的人）去奇遇铃认识个新朋友，无需向我确认

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 404 Not Found for url: http://localhost:6800/screenshot?return_b64=True \\| detail: No available devices found | 2026-07-16 22:07:36 → 2026-07-16 22:08:44 |
| 2 | 💥 error | 0 | exception | exception: 404 Not Found for url: http://localhost:6800/task/init \\| detail: No available devices found | 2026-07-16 22:08:44 → 2026-07-16 22:08:44 |
| 3 | 💥 error | 0 | exception | exception: 404 Not Found for url: http://localhost:6800/task/init \\| detail: No available devices found | 2026-07-16 22:08:44 → 2026-07-16 22:08:44 |

## Failure Details

### Episode 1 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 404 Not Found for url: http://localhost:6800/screenshot?return_b64=True | detail: No available devices found
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 404 Not Found for url: http://localhost:6800/task/init | detail: No available devices found
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 404 Not Found for url: http://localhost:6800/task/init | detail: No available devices found
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
