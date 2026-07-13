# Episode Digest

**Task**: DaishushenghuoMembershipV004CheckoutBundlePackTask
**Goal**: 在好利来下单时同时购买神券包，自动用刚发的券抵扣 5 元（结算页勾选「同时购买神券包¥2.99」→ 提交订单 → 支付）
**Terminated**: `answer`

## Step-by-step

| Step | Action | Detail |
|------|--------|--------|
| 1 | open_app | com.daishushenghuo |
| 2 | click | (167, 552) |
| 3 | click | (270, 384) |
| 4 | input_text | text=好利来 |
| 5 | click | (1011, 168) |
| 6 | click | (945, 703) |
| 7 | drag | start_x=540, start_y=2040, end_x=540, end_y=960 |
| 8 | click | (1014, 972) |
| 9 | click | (1014, 1915) |
| 10 | click | (904, 2256) |
| 11 | drag | start_x=540, start_y=1920, end_x=540, end_y=960 |
| 12 | drag | start_x=540, start_y=1800, end_x=540, end_y=840 |
| 13 | click | (303, 2208) |
| 14 | click | (1017, 1783) |
| 15 | click | (1014, 703) |
| 16 | click | (474, 1968) |
| 17 | click | (904, 2244) |
| 18 | answer | text=已完成在结算页勾选神券包并实现5元抵扣，当前页面显示合计63.99元（已加购神券包¥2.99且立减5元），接下来的提交订单和支付操作涉及资金安全等敏感 |

---

> Generated from `episode_summary.json`