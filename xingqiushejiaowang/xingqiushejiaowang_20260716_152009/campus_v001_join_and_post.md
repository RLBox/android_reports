# campus_v001_join_and_post  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangCampusV001JoinAndPostTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 479s (~8.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XingqiushejiaowangCampusV001JoinAndPostTask.log](./raw_logs/XingqiushejiaowangCampusV001JoinAndPostTask.log)
- **Generated**: 2026-07-16T19:10:00+08:00
- **Note**: backfilled from /tmp/pass_at_3_full_<ts>/ on 2026-05-02

## Task Goal

> ⚠️禁搜！星球Tab(nav-home) → 右下角星球实验室卡片直接点(entry-lab) → 校园吧(entry-campus) → 立即加入 → 选江苏大学(campus-school-option-江苏大学) → 发帖(campus-compose-btn) → 发布(campus-post-submit)

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangCampusV001JoinAndP... | 2026-07-16 15:20:54 → 2026-07-16 15:23:37 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangCampusV001JoinAndP... | 2026-07-16 15:23:37 → 2026-07-16 15:26:15 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangCampusV001JoinAndP... | 2026-07-16 15:26:15 → 2026-07-16 15:28:51 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XingqiushejiaowangCampusV001JoinAndPostTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangCampusV001JoinAndPostTask') failed: Task 'XingqiushejiaowangCampusV001JoinAndPostTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangCampusV001JoinAndPostTask') failed: Task 'XingqiushejiaowangCampusV001JoinAndPostTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangCampusV001JoinAndPostTask') failed: Task 'XingqiushejiaowangCampusV001JoinAndPostTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
