# Episode 2 — ❌ failed (5 steps)

> **Goal**: 【当前账户档案】账号：demo@rlbox.ai；昵称：张三；支付密码：123456；默认收货地址（JSON）：{"recipient": "王", "phone": "15212348132", "address": "惠恒大厦1期 3楼312室"}。请基于以上档案完成下列任务：小象超市下单时切到地址「李/世纪花园 3栋2单元502」（验 address_id 关联与 delivery_address/phone/name 三字段全部一致）

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.daishushenghuo | Got it, let's tackle this task. First, the user wants to order from小象超市 (Xiaoxiang Supermarket, which is part of Meituan… |
| 2 | click (172, 780) | Okay, now I'm on the app's main page, and I see the "小象超市" icon here, both in the top grid (the green one with a cart, l… |
| 3 | click (478, 134) | Got it, now I'm in the 小象超市 (Meituan Self-operated) page. At the top, next to the title, there's the current address: "惠… |
| 4 | click (303, 1454) | Perfect, now I'm on the address selection page. I can see the target address here: "世纪花园 3栋2单元502" with recipient 李女士 (w… |
| 5 | answer "已成功将小象超市的收货地址切换为「李/世纪花园 3栋2单元502」，验证：..." | Now I can see that the top address has changed to "世纪花园", which means the address switch was successful. Let me verify: … |

## Result

- **Terminated**: answer
