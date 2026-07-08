# party_v001_join_first_recommended  ❌

- **Brand**: `xingqiushejiaowang`
- **Class**: `XingqiushejiaowangPartyV001JoinFirstRecommendedTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 13s (~0.2 min)
- **Model**: `doubao-seed-evolving`
- **Raw log**: [./raw_logs/XingqiushejiaowangPartyV001JoinFirstRecommendedTask.log](./raw_logs/XingqiushejiaowangPartyV001JoinFirstRecommendedTask.log)
- **Generated**: 2026-07-08T13:19:37+08:00

## Task Goal

> 使用星球社交网（com.xingqiushejiaowang）应用完成以下任务：随便加入一个推荐的派对看看有什么好玩的

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangPartyV001JoinFirst... | 2026-07-08 13:17:42 → 2026-07-08 13:17:50 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangPartyV001JoinFirst... | 2026-07-08 13:17:50 → 2026-07-08 13:17:52 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XingqiushejiaowangPartyV001JoinFirst... | 2026-07-08 13:17:52 → 2026-07-08 13:17:55 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Connection refused\n\tIs the server running on that host and accepting TCP/IP connections?\nconnection to server a`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangPartyV001JoinFirstRecommendedTask') failed: Task 'XingqiushejiaowangPartyV001JoinFirstRecommendedTask' failed during initialize_task(): Xingqiushejiaowang POST /api/tasks/{self.app_task_id}/start failed: Xingqiushejiaowang POST /api/tasks/party_v001_join_first_recommended/start → HTTP 500: {"error":"Failed to start session: connection to server at \"::1\", port 5432 failed: Connection refused\n\tIs the server running on that host and accepting TCP/IP connections?\nconnection to server a
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangPartyV001JoinFirstRecommendedTask') failed: Task 'XingqiushejiaowangPartyV001JoinFirstRecommendedTask' failed during initialize_task(): Xingqiushejiaowang POST /api/tasks/{self.app_task_id}/start failed: Xingqiushejiaowang POST /api/tasks/party_v001_join_first_recommended/start → HTTP 500: {"error":"Failed to start session: connection to server at \"::1\", port 5432 failed: Connection refused\n\tIs the server running on that host and accepting TCP/IP connections?\nconnection to server a
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XingqiushejiaowangPartyV001JoinFirstRecommendedTask') failed: Task 'XingqiushejiaowangPartyV001JoinFirstRecommendedTask' failed during initialize_task(): Xingqiushejiaowang POST /api/tasks/{self.app_task_id}/start failed: Xingqiushejiaowang POST /api/tasks/party_v001_join_first_recommended/start → HTTP 500: {"error":"Failed to start session: connection to server at \"::1\", port 5432 failed: Connection refused\n\tIs the server running on that host and accepting TCP/IP connections?\nconnection to server a
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
