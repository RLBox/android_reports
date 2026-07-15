# matching_v012_voice_dual_card  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangMatchingV012VoiceDualCardTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 296s (~4.9 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangMatchingV012VoiceDualCardTask.log](./raw_logs/XingqiushejiaowangMatchingV012VoiceDualCardTask.log)
- **Generated**: 2026-07-15T18:18:26+08:00

## Task Goal

> 帮我去签到商店买一张音色卡和一张加速卡，然后发起双卡语音匹配，接通后在通话里聊至少 3 句暖场

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV012VoiceD... | 2026-07-15 17:26:32 → 2026-07-15 17:28:14 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV012VoiceD... | 2026-07-15 17:28:14 → 2026-07-15 17:29:50 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV012VoiceD... | 2026-07-15 17:29:50 → 2026-07-15 17:31:28 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangMatchingV012VoiceDualCardTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV012VoiceDualCardTask') failed: Task 'XingqiushejiaowangMatchingV012VoiceDualCardTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV012VoiceDualCardTask') failed: Task 'XingqiushejiaowangMatchingV012VoiceDualCardTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV012VoiceDualCardTask') failed: Task 'XingqiushejiaowangMatchingV012VoiceDualCardTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
