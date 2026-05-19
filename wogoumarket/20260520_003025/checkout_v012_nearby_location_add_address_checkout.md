# checkout_v012_nearby_location_add_address_checkout  ❌

- **Brand**: `wogoumarket`
- **Class**: `WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask`
- **Pass@3**: **0/3**  (score = 0.00)
- **Elapsed**: 1330s (~22.2 min)
- **Model**: `doubao-seed-2-0-pro-260215`
- **Raw log**: [./raw_logs/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask.log](./raw_logs/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask.log)
- **Generated**: 2026-05-20T00:54:05+08:00

## Task Goal

> 【当前账户档案】账号：demo@rlbox.ai；昵称：张三；支付密码：123456；默认收货地址（JSON）：{"recipient": "科憨憨", "phone": "13100002345", "address": "腾讯滨海大厦 广东省 深圳市 南山区 1楼东门外卖柜"}。请基于以上档案完成下列任务：从附近地址找到南山科技园服务点，新增该地点收货地址并下单

## Attempts

| # | Outcome | Steps | Terminated | Reason | Start → End |
|---|---------|-------|------------|--------|-------------|
| 1 | ⏰ timeout | 50 | max_steps | – | – |
| 2 | ❌ failed | 44 | answer | – | – |
| 3 | ❌ failed | 46 | answer | – | – |

## Failure Details

### Episode 1 — ⏰ timeout

- steps_used: `50`
- terminated_reason: `max_steps`
- death shot: ![last-step](./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_001/step_050.png)
  - state: [`./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_001/step_050.json`](./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_001/step_050.json)

### Episode 2 — ❌ failed

- steps_used: `44`
- terminated_reason: `answer`
- death shot: ![last-step](./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_002/step_044.png)
  - state: [`./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_002/step_044.json`](./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_002/step_044.json)

### Episode 3 — ❌ failed

- steps_used: `46`
- terminated_reason: `answer`
- death shot: ![last-step](./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_003/step_046.png)
  - state: [`./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_003/step_046.json`](./death_shots/WogoumarketCheckoutV012NearbyLocationAddAddressCheckoutTask/episode_003/step_046.json)

---

> 本摘要由 `sengclaw/scripts/pipeline/log_summarizer.py` 自动生成。 原始完整 log 见上方 Raw log 链接（含每 step 的 messages / tool_call / screenshot 引用）。
