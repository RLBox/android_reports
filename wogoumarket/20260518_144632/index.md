> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **1** 个 slug 来自 `/Users/zhangrunsheng/Documents/GitHub/box/Goomart/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `cart_v006_cart_validator` | `WogoumarketCartV006CartValidatorTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/zhangrunsheng/Documents/GitHub/box/Goomart
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — wogoumarket — 20260518_144632

## Summary

- ❌ 预检后没有可跑 slug（候选池里 1 个全部在容器里没注册）
- 请按下方「候选池清理建议」清理 `db/validator_statuses.json` 后重跑 pipeline

