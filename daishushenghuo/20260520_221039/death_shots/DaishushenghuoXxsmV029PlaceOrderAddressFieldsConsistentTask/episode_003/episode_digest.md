# Episode 3 — ❌ failed (5 steps)

> **Goal**: 【当前账户档案】账号：demo@rlbox.ai；昵称：张三；支付密码：123456；默认收货地址（JSON）：{"recipient": "王", "phone": "15212348132", "address": "惠恒大厦1期 3楼312室"}。请基于以上档案完成下列任务：小象超市下单时切到地址「李/世纪花园 3栋2单元502」（验 address_id 关联与 delivery_address/phone/name 三字段全部一致）

## Step Timeline

| # | Action | Think |
|---|--------|-------|
| 1 | open_app com.daishushenghuo | Got it, let's see. The task is about ordering on 小象超市 (Xiaoxiang Supermarket) and switching the address to 李/世纪花园 3栋2单元5… |
| 2 | click (172, 785) | Got it, now I'm on the home page of the app. The task is to go to 小象超市 to order, and switch the address to "李/世纪花园 3栋2单元… |
| 3 | click (477, 132) | 现在我在小象超市的页面，顶部显示当前地址是惠恒大厦1期，这是默认的地址。任务需要切换到「李/世纪花园 3栋2单元502」这个地址。首先我得点击顶部的地址区域，就是显示“惠恒大厦1期”旁边的箭头，进入地址选择页面，这样才能切换到目标地址。所以… |
| 4 | click (300, 1452) | 现在我在地址选择页面，看到收货地址列表里有“世纪花园 3栋2单元502”，联系人是李女士，正好是我要切换的目标地址。那我现在只需要点击这个地址选项，就能把配送地址切换成这个了，对吧？这样之后下单的时候就会用这个地址了。那我就点这个地址条目，… |
| 5 | answer "已成功将小象超市的配送地址切换为「李/世纪花园 3栋2单元502」，当前页..." | 现在顶部的地址已经变成世纪花园了，对应的就是我们选择的「李/世纪花园 3栋2单元502」地址对吧？首先确认一下，之前选的地址是李女士的世纪花园3栋2单元502，现在页面顶部显示地址是世纪花园，说明切换成功了。那任务是下单时切到这个地址，现在… |

## Result

- **Terminated**: answer
