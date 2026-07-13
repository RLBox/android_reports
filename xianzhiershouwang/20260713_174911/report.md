# Android Sandbox Pass@3 测试报告（增量更新中）

> **run_id**：`xianzhiershouwang_20260713_174911`  
> **started_at**：2026-07-13T17:49:11  
> **model**：`unknown`  
> **server**：http://localhost:6800  
> **k**：3  |  **max_steps**：80  
> **report_dir**：`/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911`

## 进度总览

- ✅ 已完成 task：**10 / 10**
- 🟢 Pass@3 = 1.0 的 task：**8 / 10**（命中率 80.0%）
- 🎯 episode 总成功率：**22 / 30**（73.3%）

## 品牌汇总

| 品牌 | 已测 task | Pass@3=1.0 | Episode 成功 | 备注 |
|---|---|---|---|---|
| 🟡 Other | 10 | 8/10 | 22/30 | |

## 每个 Task 详细结果

| # | Task | Pass@3 | Success/K | Steps | Terminated | Elapsed | Artifact |
|---|---|---|---|---|---|---|---|
| 1 | `XianzhiershouwangAddressV001AddressValidatorTask` | 🟢 1.0 | 3/3 | 26/32/22 | answer:3 | 490s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangAddressV001AddressValidatorTask` |
| 2 | `XianzhiershouwangAddressV002AddressValidatorTask` | 🟢 1.0 | 3/3 | 23/30/25 | answer:3 | 469s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangAddressV002AddressValidatorTask` |
| 3 | `XianzhiershouwangAddressV003AddressValidatorTask` | 🟢 1.0 | 3/3 | 28/80/31 | answer:3 | 1632s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangAddressV003AddressValidatorTask` |
| 4 | `XianzhiershouwangCommentV001CommentValidatorTask` | 🟢 1.0 | 3/3 | 27/25/24 | answer:3 | 562s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangCommentV001CommentValidatorTask` |
| 5 | `XianzhiershouwangCommentV002CommentValidatorTask` | 🔴 0.0 | 0/3 | 0/0/0 | exception:3 | 298s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangCommentV002CommentValidatorTask` |
| 6 | `XianzhiershouwangCommentV003CommentValidatorTask` | 🔴 0.0 | 0/3 | 0/0/0 | exception:3 | 298s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangCommentV003CommentValidatorTask` |
| 7 | `XianzhiershouwangFavoriteV001FavoriteValidatorTask` | 🟢 1.0 | 1/3 | 14/0/0 | answer:1, exception:2 | 353s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangFavoriteV001FavoriteValidatorTask` |
| 8 | `XianzhiershouwangFavoriteV002FavoriteValidatorTask` | 🟢 1.0 | 3/3 | 32/13/14 | answer:3 | 484s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangFavoriteV002FavoriteValidatorTask` |
| 9 | `XianzhiershouwangFavoriteV003FavoriteValidatorTask` | 🟢 1.0 | 3/3 | 29/9/37 | answer:3 | 552s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangFavoriteV003FavoriteValidatorTask` |
| 10 | `XianzhiershouwangLikeV001LikeValidatorTask` | 🟢 1.0 | 3/3 | 14/14/14 | answer:3 | 384s | `/tmp/pass_at_3_reports/xianzhiershouwang_20260713_174911/artifacts/XianzhiershouwangLikeV001LikeValidatorTask` |

## ❌ 失败案例（Pass@3 < 1.0）

### `XianzhiershouwangCommentV002CommentValidatorTask`
- success: 0/3
- terminated_breakdown: `{'exception': 3}`
  - ep1: score=0.00 steps=0 reason=exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangCommentV002CommentValidatorTask') failed: Ta
  - ep2: score=0.00 steps=0 reason=exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangCommentV002CommentValidatorTask') failed: Ta
  - ep3: score=0.00 steps=0 reason=exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangCommentV002CommentValidatorTask') failed: Ta

### `XianzhiershouwangCommentV003CommentValidatorTask`
- success: 0/3
- terminated_breakdown: `{'exception': 3}`
  - ep1: score=0.00 steps=0 reason=exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangCommentV003CommentValidatorTask') failed: Ta
  - ep2: score=0.00 steps=0 reason=exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangCommentV003CommentValidatorTask') failed: Ta
  - ep3: score=0.00 steps=0 reason=exception: 500 Internal Server Error for url: http://localhost:6800/task/init | detail: init_task('XianzhiershouwangCommentV003CommentValidatorTask') failed: Ta

---
> 最后更新：2026-07-13T19:28:51
