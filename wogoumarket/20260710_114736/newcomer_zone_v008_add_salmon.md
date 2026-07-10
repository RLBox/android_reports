# newcomer_zone_v008_add_salmon  ❌

- **Brand**: `wogoumarket`
- **Class**: `WogoumarketNewcomerZoneV008AddSalmonTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 295s (~4.9 min)
- **Model**: `doubao-seed-2-0-pro-260215`
- **Raw log**: [./raw_logs/WogoumarketNewcomerZoneV008AddSalmonTask.log](./raw_logs/WogoumarketNewcomerZoneV008AddSalmonTask.log)
- **Generated**: 2026-07-10T14:16:41+08:00

## Task Goal

> 在新人专区生鲜专区"大家都在买"频道加购挪威三文鱼1份，切换到"肉禽蛋品"频道加购猪后腿肉1斤，再到首页搜索青椒加购一份双丰青椒（500g），最后结算下单

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketNewcomerZoneV008AddSalmon... | 2026-07-10 13:48:51 → 2026-07-10 13:50:28 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketNewcomerZoneV008AddSalmon... | 2026-07-10 13:50:28 → 2026-07-10 13:52:08 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('WogoumarketNewcomerZoneV008AddSalmon... | 2026-07-10 13:52:09 → 2026-07-10 13:53:46 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'WogoumarketNewcomerZoneV008AddSalmonTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketNewcomerZoneV008AddSalmonTask') failed: Task 'WogoumarketNewcomerZoneV008AddSalmonTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketNewcomerZoneV008AddSalmonTask') failed: Task 'WogoumarketNewcomerZoneV008AddSalmonTask' failed during initialize_task(): Command 'adb -s emulator-5554 shell settings put global wogoumarket_api_endpoint http://10.0.2.2:11601' timed out after 5 seconds
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('WogoumarketNewcomerZoneV008AddSalmonTask') failed: Task 'WogoumarketNewcomerZoneV008AddSalmonTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
