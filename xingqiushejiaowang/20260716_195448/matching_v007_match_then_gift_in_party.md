# matching_v007_match_then_gift_in_party  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 838s (~14.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask.log](./raw_logs/XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask.log)
- **Generated**: 2026-07-17T08:04:29+08:00

## Task Goal

> 灵魂匹配到的小猫姐姐有派对，进派对送 50 星币以内见面礼

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV007MatchT... | 2026-07-16 22:15:59 → 2026-07-16 22:20:39 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV007MatchT... | 2026-07-16 22:20:39 → 2026-07-16 22:25:18 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV007MatchT... | 2026-07-16 22:25:18 → 2026-07-16 22:29:58 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask' failed during initialize_task()`
> 
> **排查步骤**：
> 1. 检查品牌后端是否正常运行
> 2. 查看后端 log：`docker logs vendor_android_env | grep -A5 initialize_task`
> 3. 或直接访问品牌后端 admin 页面手动触发该 task 看具体报错

## Failure Details

### Episode 1 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask') failed: Task 'XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask') failed: Task 'XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask') failed: Task 'XingqiushejiaowangMatchingV007MatchThenGiftInPartyTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
