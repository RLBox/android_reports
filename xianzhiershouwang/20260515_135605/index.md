> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **15** 个 slug 来自 `/Users/zhangrunsheng/Documents/GitHub/box/IdleSwap/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `comment/v004_comment_validator` | `XianzhiershouwangCommentV004CommentValidatorTask` |
> | `comment/v005_comment_validator` | `XianzhiershouwangCommentV005CommentValidatorTask` |
> | `favorite/v001_favorite_validator` | `XianzhiershouwangFavoriteV001FavoriteValidatorTask` |
> | `favorite/v002_favorite_validator` | `XianzhiershouwangFavoriteV002FavoriteValidatorTask` |
> | `like/v002_like_validator` | `XianzhiershouwangLikeV002LikeValidatorTask` |
> | `message/v001_message_validator` | `XianzhiershouwangMessageV001MessageValidatorTask` |
> | `message/v004_message_validator` | `XianzhiershouwangMessageV004MessageValidatorTask` |
> | `message/v006_message_validator` | `XianzhiershouwangMessageV006MessageValidatorTask` |
> | `message/v007_message_validator` | `XianzhiershouwangMessageV007MessageValidatorTask` |
> | `message/v008_message_validator` | `XianzhiershouwangMessageV008MessageValidatorTask` |
> | `order/v001_order_validator` | `XianzhiershouwangOrderV001OrderValidatorTask` |
> | `order/v004_order_validator` | `XianzhiershouwangOrderV004OrderValidatorTask` |
> | `post/v009_post_validator` | `XianzhiershouwangPostV009PostValidatorTask` |
> | `post/v016_post_validator` | `XianzhiershouwangPostV016PostValidatorTask` |
> | `post/v020_post_validator` | `XianzhiershouwangPostV020PostValidatorTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/zhangrunsheng/Documents/GitHub/box/IdleSwap
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — xianzhiershouwang — 20260515_135605

## Summary

- ❌ 预检后没有可跑 slug（候选池里 15 个全部在容器里没注册）
- 请按下方「候选池清理建议」清理 `db/validator_statuses.json` 后重跑 pipeline

