> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **8** 个 slug 来自 `/Users/kehan/Documents/GitHub/box/Goomart/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `account_v002_view_rules_then_purchase_saving_card` | `WogoumarketAccountV002ViewRulesThenPurchaseSavingCardTask` |
> | `checkout_v005_checkout_with_saving_card` | `WogoumarketCheckoutV005CheckoutWithSavingCardTask` |
> | `checkout_v006_remark_pick_fresh` | `WogoumarketCheckoutV006RemarkPickFreshTask` |
> | `checkout_v007_drop_off_door_current_order` | `WogoumarketCheckoutV007DropOffDoorCurrentOrderTask` |
> | `checkout_v009_shortage_policy_call_me` | `WogoumarketCheckoutV009ShortagePolicyCallMeTask` |
> | `common_v001_search_add_edit_checkout` | `WogoumarketCommonV001SearchAddEditCheckoutTask` |
> | `common_v002_express_filter_price_sort_checkout` | `WogoumarketCommonV002ExpressFilterPriceSortCheckoutTask` |
> | `search_v002_search_milk_sort_by_sales` | `WogoumarketSearchV002SearchMilkSortBySalesTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/kehan/Documents/GitHub/box/Goomart
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — wogoumarket — 20260712_183610

## Summary

- ❌ 预检后没有可跑 slug（候选池里 8 个全部在容器里没注册）
- 请按下方「候选池清理建议」清理 `db/validator_statuses.json` 后重跑 pipeline

