# cart_v013_add_pork_jerky_from_recommend  ❌

- **Brand**: `wogoumarket`
- **Class**: `WogoumarketCartV013AddPorkJerkyFromRecommendTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 182s (~3.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/WogoumarketCartV013AddPorkJerkyFromRecommendTask.log](./raw_logs/WogoumarketCartV013AddPorkJerkyFromRecommendTask.log)
- **Generated**: 2026-06-08T17:01:53+08:00

## Task Goal

> 看看购物车有啥东西了，下面好物推荐里的东西挺感兴趣的，把澳洲牛排加购1份

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketCartV013AddPorkJerkyFromR... | 2026-06-08 08:51:37 → 2026-06-08 08:52:37 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketCartV013AddPorkJerkyFromR... | 2026-06-08 08:52:37 → 2026-06-08 08:53:37 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketCartV013AddPorkJerkyFromR... | 2026-06-08 08:53:37 → 2026-06-08 08:54:38 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'WogoumarketCartV013AddPorkJerkyFromRecommendTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketCartV013AddPorkJerkyFromRecommendTask') failed: Task 'WogoumarketCartV013AddPorkJerkyFromRecommendTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketCartV013AddPorkJerkyFromRecommendTask') failed: Task 'WogoumarketCartV013AddPorkJerkyFromRecommendTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketCartV013AddPorkJerkyFromRecommendTask') failed: Task 'WogoumarketCartV013AddPorkJerkyFromRecommendTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
