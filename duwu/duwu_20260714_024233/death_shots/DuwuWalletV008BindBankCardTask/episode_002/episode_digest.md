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
| 4 | wait | ?ms |
| 5 | click | (73, 127) |
| 6 | drag | start_x=522, start_y=2112, end_x=522, end_y=840 |
| 7 | click | (1002, 125) |
| 8 | click | (819, 1284) |
| 9 | click | (170, 1056) |
| 10 | ask_user | text=进入Du有钱模块需要先勾选同意《佳物消费金融服务协议及信息授权协议》，该操作涉及你的隐私授权，且后续还需要进行实名信息核验、人脸信息核验等敏感操作，以 |
| 11 | answer | text=由于进入Du有钱模块需要你自行勾选同意相关金融服务协议，且后续还涉及实名信息核验、人脸信息核验以及银行卡绑定的验证等敏感操作，你当前不在场无法完成这些 |

---

> Generated from `episode_summary.json`