# address_v004_add_school_address  ❌

- **Brand**: `daishushenghuo`
- **Class**: `DaishushenghuoAddressV004AddSchoolAddressTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 181s (~3.0 min)
- **Model**: `doubao-seed-2-0-lite-260428`
- **Raw log**: [./raw_logs/DaishushenghuoAddressV004AddSchoolAddressTask.log](./raw_logs/DaishushenghuoAddressV004AddSchoolAddressTask.log)
- **Generated**: 2026-05-24T09:55:20+08:00

## Task Goal

> 【当前账户档案】账号：demo@rlbox.ai；昵称：张三；支付密码：123456；默认收货地址（JSON）：{"recipient": "王", "phone": "15212348132", "address": "惠恒大厦1期 3楼312室"}。请基于以上档案使用袋鼠生活应用完成以下任务：新增学校收货地址（联系人：赵同学 15088889999，北京市海淀区北京大学燕园28号楼，类型：学校）

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('DaishushenghuoAddressV004AddSchoolAd... | 2026-05-24 09:52:19 → 2026-05-24 09:53:19 |
| 2 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('DaishushenghuoAddressV004AddSchoolAd... | 2026-05-24 09:53:19 → 2026-05-24 09:54:19 |
| 3 | 💥 error | 0 | exception | exception: 500 Internal Server Error for url: http://localhost:6800/task/init \\| detail: init_task('DaishushenghuoAddressV004AddSchoolAd... | 2026-05-24 09:54:19 → 2026-05-24 09:55:20 |

## Failure Details

### Episode 1 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('DaishushenghuoAddressV004AddSchoolAddressTask') failed: Task 'DaishushenghuoAddressV004AddSchoolAddressTask' failed during initialize_task()
  ```

### Episode 2 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('DaishushenghuoAddressV004AddSchoolAddressTask') failed: Task 'DaishushenghuoAddressV004AddSchoolAddressTask' failed during initialize_task()
  ```

### Episode 3 — 💥 error

- steps_used: `0`
- terminated_reason: `exception`
- reason:

  ```
  exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('DaishushenghuoAddressV004AddSchoolAddressTask') failed: Task 'DaishushenghuoAddressV004AddSchoolAddressTask' failed during initialize_task()
  ```

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
