# search_v006_search_egg_view_and_checkout  ❌

- **Brand**: `wogoumarket`
- **Class**: `WogoumarketSearchV006SearchEggViewAndCheckoutTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 295s (~4.9 min)
- **Model**: `doubao-seed-2-0-pro-260215`
- **Raw log**: [./raw_logs/WogoumarketSearchV006SearchEggViewAndCheckoutTask.log](./raw_logs/WogoumarketSearchV006SearchEggViewAndCheckoutTask.log)
- **Generated**: 2026-07-10T17:40:15+08:00

## Task Goal

> 想买鸡蛋，帮我在搜索页点击热门搜索，然后找到鲜鸡蛋，看下详情后买一盒

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketSearchV006SearchEggViewAn... | 2026-07-10 16:48:14 → 2026-07-10 16:49:52 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketSearchV006SearchEggViewAn... | 2026-07-10 16:49:52 → 2026-07-10 16:51:31 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketSearchV006SearchEggViewAn... | 2026-07-10 16:51:31 → 2026-07-10 16:53:09 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'WogoumarketSearchV006SearchEggViewAndCheckoutTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketSearchV006SearchEggViewAndCheckoutTask') failed: Task 'WogoumarketSearchV006SearchEggViewAndCheckoutTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketSearchV006SearchEggViewAndCheckoutTask') failed: Task 'WogoumarketSearchV006SearchEggViewAndCheckoutTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketSearchV006SearchEggViewAndCheckoutTask') failed: Task 'WogoumarketSearchV006SearchEggViewAndCheckoutTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
