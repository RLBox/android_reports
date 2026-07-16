# journeys_v023_status_party_gift_post  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangJourneysV023StatusPartyGiftPostTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 479s (~8.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangJourneysV023StatusPartyGiftPostTask.log](./raw_logs/XingqiushejiaowangJourneysV023StatusPartyGiftPostTask.log)
- **Generated**: 2026-07-16T14:40:36+08:00
- **Note**: backfilled from /tmp/pass_at_3_full_<ts>/ on 2026-05-02

## Task Goal

> 切换为「想要聊天」状态 → 进「音乐分享会」发言 → 给主持人送「甜甜圈」(8星币) → 发帖含「夜聊」

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV023Status... | 2026-07-16 11:05:18 → 2026-07-16 11:08:01 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV023Status... | 2026-07-16 11:08:01 → 2026-07-16 11:10:39 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV023Status... | 2026-07-16 11:10:39 → 2026-07-16 11:13:17 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangJourneysV023StatusPartyGiftPostTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV023StatusPartyGiftPostTask') failed: Task 'XingqiushejiaowangJourneysV023StatusPartyGiftPostTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV023StatusPartyGiftPostTask') failed: Task 'XingqiushejiaowangJourneysV023StatusPartyGiftPostTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV023StatusPartyGiftPostTask') failed: Task 'XingqiushejiaowangJourneysV023StatusPartyGiftPostTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
