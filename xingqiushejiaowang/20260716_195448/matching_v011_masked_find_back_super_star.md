# matching_v011_masked_find_back_super_star  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 838s (~14.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask.log](./raw_logs/XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask.log)
- **Generated**: 2026-07-17T08:24:35+08:00

## Task Goal

> 超级星人已开通 → 我的遇见找回蒙面酒馆「小羊咩咩」→ 关注并私聊含「酒馆」

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV011Masked... | 2026-07-16 22:48:03 → 2026-07-16 22:52:42 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV011Masked... | 2026-07-16 22:52:42 → 2026-07-16 22:57:22 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV011Masked... | 2026-07-16 22:57:22 → 2026-07-16 23:02:01 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask') failed: Task 'XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask') failed: Task 'XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask') failed: Task 'XingqiushejiaowangMatchingV011MaskedFindBackSuperStarTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
