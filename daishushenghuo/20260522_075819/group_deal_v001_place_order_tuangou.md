# group_deal_v001_place_order_tuangou  ❌

- **Brand**: `daishushenghuo`
- **Class**: `DaishushenghuoGroupDealV001PlaceOrderTuangouTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 8s (~0.1 min)
- **Model**: `doubao-seed-2-0-pro-260215`
- **Raw log**: [./raw_logs/DaishushenghuoGroupDealV001PlaceOrderTuangouTask.log](./raw_logs/DaishushenghuoGroupDealV001PlaceOrderTuangouTask.log)
- **Generated**: 2026-05-22T12:03:59+08:00

## Task Goal

> 当前App：【袋鼠生活】。

> 🔴 **基建重试记录**：本 task 发生 1 次基建重试（原因：ep1: /task/init + vendor_restart），重试后仍全部失败，**建议排查 infra 而非 Agent 能力**。

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Server Error: Internal Server Error for url: http://localhost:6800/task/init | 2026-05-22 08:04:04 → 2026-05-22 08:04:11 |
| 2 | 💥 error | 0 | exception | exception: 404 Client Error: Not Found for url: http://localhost:6800/task/init | 2026-05-22 08:04:11 → 2026-05-22 08:04:11 |
| 3 | 💥 error | 0 | exception | exception: 404 Client Error: Not Found for url: http://localhost:6800/task/init | 2026-05-22 08:04:11 → 2026-05-22 08:04:11 |

## Failure Details

### Episode 1 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Server Error: Internal Server Error for url: http://localhost:6800/task/init
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 404 Client Error: Not Found for url: http://localhost:6800/task/init
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 404 Client Error: Not Found for url: http://localhost:6800/task/init
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
