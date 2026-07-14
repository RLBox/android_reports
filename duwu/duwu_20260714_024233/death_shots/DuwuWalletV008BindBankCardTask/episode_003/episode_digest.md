# Episode Digest

**Task**: DuwuWalletV008BindBankCardTask
**Goal**: 去「借钱」模块，在 Du有钱 里的「我的银行卡」里绑定一张中国农业银行卡，卡号 6225880137290827
**Terminated**: `answer`

## Step-by-step

| Step | Action | Detail |
|------|--------|--------|
| 1 | open_app | com.duwu |
| 2 | click | (945, 2268) |
| 3 | click | (414, 1872) |
| 4 | ask_user | text=当前进入Du有钱页面需要同意金融服务协议并进行额度查看相关操作，且绑定银行卡涉及个人身份信息、预留手机号验证等敏感隐私操作，请你接管完成协议勾选、后续 |
| 5 | click | (73, 132) |
| 6 | drag | start_x=526, start_y=2112, end_x=526, end_y=840 |
| 7 | click | (1002, 125) |
| 8 | click | (823, 1284) |
| 9 | click | (170, 1056) |
| 10 | click | (1007, 132) |
| 11 | click | (1026, 528) |
| 12 | ask_user | text=在com.duwu（得物）的Du有钱模块中，绑定银行卡需要先完成服务协议同意、实名信息核验、人脸验证、银行卡预留手机号短信验证等涉及你个人隐私及身份核 |
| 13 | wait | ?ms |
| 14 | input_text | text=已为你找到com.duwu（得物）中的「借钱」模块（Du有钱），但绑定中国农业银行卡（卡号6225880137290827）需要你本人完成服务协议同意 |
| 15 | wait | ?ms |
| 16 | answer | text=已为你定位到com.duwu（得物）的「借钱」模块（Du有钱），但绑定指定中国农业银行卡需要你本人完成服务协议签署、实名身份核验、人脸验证、银行卡预留 |

---

> Generated from `episode_summary.json`