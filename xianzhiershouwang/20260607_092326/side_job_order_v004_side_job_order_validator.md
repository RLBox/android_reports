# side_job_order/v004_side_job_order_validator  ❌

- **Brand**: `xianzhiershouwang`
- **Class**: `XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 182s (~3.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask.log](./raw_logs/XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask.log)
- **Generated**: 2026-06-07T16:06:03+08:00

## Task Goal

> 帮妈妈在神奇副业找广州三甲医院全程陪诊服务，微信下单

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XianzhiershouwangSideJobOrderV004Sid... | 2026-06-07 16:03:02 → 2026-06-07 16:04:02 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XianzhiershouwangSideJobOrderV004Sid... | 2026-06-07 16:04:02 → 2026-06-07 16:05:02 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('XianzhiershouwangSideJobOrderV004Sid... | 2026-06-07 16:05:02 → 2026-06-07 16:06:03 |

> 🔴 **品牌后端异常**：所有 episode 均在 `initialize_task()` 阶段失败（HTTP 500），非 Agent 能力问题。
> **后端报错**：`Task 'XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask' failed during initialize_task()`
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
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask') failed: Task 'XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask') failed: Task 'XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask') failed: Task 'XianzhiershouwangSideJobOrderV004SideJobOrderValidatorTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
