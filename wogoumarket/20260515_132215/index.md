> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **12** 个 slug 来自 `/Users/zhangrunsheng/Documents/GitHub/box/Goomart/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `account_v002_view_rules_then_purchase_saving_card` | `WogoumarketAccountV002ViewRulesThenPurchaseSavingCardTask` |
> | `catalog_v012_durian_and_melon_add_cart` | `WogoumarketCatalogV012DurianAndMelonAddCartTask` |
> | `checkout_v005_checkout_with_saving_card` | `WogoumarketCheckoutV005CheckoutWithSavingCardTask` |
> | `common_v001_search_add_edit_checkout` | `WogoumarketCommonV001SearchAddEditCheckoutTask` |
> | `common_v002_express_filter_price_sort_checkout` | `WogoumarketCommonV002ExpressFilterPriceSortCheckoutTask` |
> | `notification_v001_mark_all_read` | `WogoumarketNotificationV001MarkAllReadTask` |
> | `search_v001_search_milk_price_range` | `WogoumarketSearchV001SearchMilkPriceRangeTask` |
> | `search_v002_search_milk_sort_by_sales` | `WogoumarketSearchV002SearchMilkSortBySalesTask` |
> | `search_v003_search_no_result_fallback` | `WogoumarketSearchV003SearchNoResultFallbackTask` |
> | `search_v004_search_flower_from_home` | `WogoumarketSearchV004SearchFlowerFromHomeTask` |
> | `search_v005_search_beef_add_braised` | `WogoumarketSearchV005SearchBeefAddBraisedTask` |
> | `search_v006_search_egg_view_and_checkout` | `WogoumarketSearchV006SearchEggViewAndCheckoutTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/zhangrunsheng/Documents/GitHub/box/Goomart
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — wogoumarket — 20260515_132215

## Summary

- ❌ 预检后没有可跑 slug（候选池里 12 个全部在容器里没注册）
- 请按下方「候选池清理建议」清理 `db/validator_statuses.json` 后重跑 pipeline

