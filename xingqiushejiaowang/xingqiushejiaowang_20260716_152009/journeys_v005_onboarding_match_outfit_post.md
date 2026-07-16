# journeys_v005_onboarding_match_outfit_post  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 321s (~5.3 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask.log](./raw_logs/XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask.log)
- **Generated**: 2026-07-16T19:10:00+08:00
- **Note**: backfilled from /tmp/pass_at_3_full_<ts>/ on 2026-05-02

## Task Goal

> 新人流程走完后，先去灵魂匹配认识一个人，然后去个性商城买个装扮，买完记得去背包里把它戴上，最后到广场发一条带图片的动态

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV005Onboar... | 2026-07-16 19:02:19 → 2026-07-16 19:05:02 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV005Onboar... | 2026-07-16 19:05:02 → 2026-07-16 19:07:40 |
| 3 | 💥 error | 0 | exception | exception: 404 Not Found for url: http://localhost:6800/task/init \\| detail: No available devices found | 2026-07-16 19:07:40 → 2026-07-16 19:07:40 |

## Failure Details

### Episode 1 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask') failed: Task 'XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask') failed: Task 'XingqiushejiaowangJourneysV005OnboardingMatchOutfitPostTask' failed during initialize_task()
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
