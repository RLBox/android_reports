# matching_v006_dual_card_soul_match  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangMatchingV006DualCardSoulMatchTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 295s (~4.9 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangMatchingV006DualCardSoulMatchTask.log](./raw_logs/XingqiushejiaowangMatchingV006DualCardSoulMatchTask.log)
- **Generated**: 2026-07-15T18:18:25+08:00

## Task Goal

> 我是上海的 INFJ，想认识两种新朋友：帮我去签到商店分别买一张同城卡和一张 MBTI 卡，各发起一次匹配，匹配到的都关注并打声招呼

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV006DualCa... | 2026-07-15 16:23:39 → 2026-07-15 16:25:21 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV006DualCa... | 2026-07-15 16:25:21 → 2026-07-15 16:26:58 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangMatchingV006DualCa... | 2026-07-15 16:26:58 → 2026-07-15 16:28:34 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangMatchingV006DualCardSoulMatchTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV006DualCardSoulMatchTask') failed: Task 'XingqiushejiaowangMatchingV006DualCardSoulMatchTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV006DualCardSoulMatchTask') failed: Task 'XingqiushejiaowangMatchingV006DualCardSoulMatchTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangMatchingV006DualCardSoulMatchTask') failed: Task 'XingqiushejiaowangMatchingV006DualCardSoulMatchTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
