# common_v027_budget_max_snack_variety  ❌

- **Brand**: `wogoumarket`
- **Class**: `WogoumarketCommonV027BudgetMaxSnackVarietyTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 181s (~3.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/WogoumarketCommonV027BudgetMaxSnackVarietyTask.log](./raw_logs/WogoumarketCommonV027BudgetMaxSnackVarietyTask.log)
- **Generated**: 2026-06-08T17:01:53+08:00

## Task Goal

> 我只有50块预算，帮我在零食区尽量多买几种不同的，每种一份，别超预算

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketCommonV027BudgetMaxSnackV... | 2026-06-08 11:22:55 → 2026-06-08 11:23:55 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketCommonV027BudgetMaxSnackV... | 2026-06-08 11:23:55 → 2026-06-08 11:24:56 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketCommonV027BudgetMaxSnackV... | 2026-06-08 11:24:56 → 2026-06-08 11:25:56 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'WogoumarketCommonV027BudgetMaxSnackVarietyTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketCommonV027BudgetMaxSnackVarietyTask') failed: Task 'WogoumarketCommonV027BudgetMaxSnackVarietyTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketCommonV027BudgetMaxSnackVarietyTask') failed: Task 'WogoumarketCommonV027BudgetMaxSnackVarietyTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketCommonV027BudgetMaxSnackVarietyTask') failed: Task 'WogoumarketCommonV027BudgetMaxSnackVarietyTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
