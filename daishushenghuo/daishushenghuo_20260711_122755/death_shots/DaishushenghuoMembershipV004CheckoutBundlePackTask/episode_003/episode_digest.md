# Episode Digest

**Task**: DaishushenghuoMembershipV004CheckoutBundlePackTask
**Goal**: 在好利来下单时同时购买神券包，自动用刚发的券抵扣 5 元（结算页勾选「同时购买神券包¥2.99」→ 提交订单 → 支付）
**Terminated**: `answer`

## Step-by-step

| Step | Action | Detail |
|------|--------|--------|
| 1 | open_app | com.daishushenghuo |
| 2 | click | (171, 545) |
| 3 | click | (251, 396) |
| 4 | input_text | text=好利来 |
| 5 | click | (1007, 168) |
| 6 | click | (945, 698) |
| 7 | ask_user | text=请你指定在好利来店铺中需要选购的商品，以便继续完成下单流程。 |
| 8 | drag | start_x=540, start_y=2040, end_x=540, end_y=1080 |
| 9 | click | (1015, 1169) |
| 10 | click | (1015, 2119) |
| 11 | click | (900, 2256) |
| 12 | drag | start_x=540, start_y=1920, end_x=540, end_y=960 |
| 13 | drag | start_x=540, start_y=1920, end_x=540, end_y=720 |
| 14 | ask_user | text=在当前好利来店铺的结算页面中，未找到“同时购买神券包¥2.99”的相关勾选选项，无法完成对应操作，请你确认相关设置或给出后续指示。 |
| 15 | click | (869, 2232) |
| 16 | answer | text=当前已提交订单，进入支付密码输入页面，支付操作涉及你的隐私和资金安全，请你自行输入支付密码完成支付步骤，后续相关操作由你自主完成。 |

---

> Generated from `episode_summary.json`