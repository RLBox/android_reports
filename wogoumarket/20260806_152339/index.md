> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **3** 个 slug 来自 `/Users/zhangrunsheng/Documents/GitHub/box/Goomart/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `checkout_v023_addon_to_use_coupon` | `WogoumarketCheckoutV023AddonToUseCouponTask` |
> | `checkout_v026_recommendation_refresh_then_pay` | `WogoumarketCheckoutV026RecommendationRefreshThenPayTask` |
> | `order_v029_use_coupon_checkout` | `WogoumarketOrderV029UseCouponCheckoutTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/zhangrunsheng/Documents/GitHub/box/Goomart
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — wogoumarket — 20260806_152339

## Summary

- Total tasks: **6**
- ✅ All passed (3/3): **0**
- ⚠️  Partial (1-2 / 3): **6**
- ❌ Failed (0/3): **0**
- Total elapsed: 1914s (31.9 min)

## Tasks

| Status | Task | Pass@3 | Steps (ep1/ep2/ep3) | Elapsed |
|--------|------|--------|---------------------|---------|
| ⚠️ | [`WogoumarketCheckoutV032Fresh29FreeDeliveryTask`](./checkout_v032_fresh_29_free_delivery.md) | 1/3 | 40/?/? | 843s |
| ⚠️ | [`WogoumarketNotificationV015PaySavingCardFromExpiryNotificationTask`](./notification_v015_pay_saving_card_from_expiry_notification.md) | 1/3 | 14/?/? | 122s |
| ⚠️ | [`WogoumarketOrderV047CancelAndRebuyZongziTask`](./order_v047_cancel_and_rebuy_zongzi.md) | 1/3 | 25/?/? | 258s |
| ⚠️ | [`WogoumarketSearchV006SearchEggViewAndCheckoutTask`](./search_v006_search_egg_view_and_checkout.md) | 1/3 | 18/?/? | 211s |
| ⚠️ | [`WogoumarketSearchV007SearchGrapeMostExpensiveCheckoutTask`](./search_v007_search_grape_most_expensive_checkout.md) | 1/3 | 20/?/? | 265s |
| ⚠️ | [`WogoumarketSearchV008SearchZongziCheapestCheckoutTask`](./search_v008_search_zongzi_cheapest_checkout.md) | 1/3 | 19/?/? | 215s |
