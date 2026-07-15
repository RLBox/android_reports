# journeys_v014_stealth_follow_gift_quiet_off_dm  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 295s (~4.9 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask.log](./raw_logs/XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask.log)
- **Generated**: 2026-07-15T18:47:42+08:00
- **Note**: backfilled from /tmp/pass_at_3_full_<ts>/ on 2026-05-02

## Task Goal

> 隐身经济学：悄悄关注海风拾贝 → 收到 ta 送的礼物 → 关掉自闭模式切回想要聊天 → 私聊海风拾贝致谢

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV014Stealt... | 2026-07-15 14:31:59 → 2026-07-15 14:33:41 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV014Stealt... | 2026-07-15 14:33:41 → 2026-07-15 14:35:17 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangJourneysV014Stealt... | 2026-07-15 14:35:18 → 2026-07-15 14:36:54 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask') failed: Task 'XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask') failed: Task 'XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask') failed: Task 'XingqiushejiaowangJourneysV014StealthFollowGiftQuietOffDmTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
