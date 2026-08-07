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

# Pass@3 Report — wogoumarket — 20260804_183409

## Summary

- Total tasks: **10**
- ✅ All passed (3/3): **0**
- ⚠️  Partial (1-2 / 3): **0**
- ❌ Failed (0/3): **10**
- Total elapsed: 5762s (96.0 min)

## Tasks

| Status | Task | Pass@3 | Steps (ep1/ep2/ep3) | Elapsed |
|--------|------|--------|---------------------|---------|
| ❌ | [`WogoumarketCheckoutV032Fresh29FreeDeliveryTask`](./checkout_v032_fresh_29_free_delivery.md) | 0/3 | 80/8/80 | 1525s |
| ❌ | [`WogoumarketNotificationV011ReorderFromPaymentTimeoutNotificationTask`](./notification_v011_reorder_from_payment_timeout_notification.md) | 0/3 | 61/52/47 | 1358s |
| ❌ | [`WogoumarketNotificationV015PaySavingCardFromExpiryNotificationTask`](./notification_v015_pay_saving_card_from_expiry_notification.md) | 0/3 | 9/15/38 | 479s |
| ❌ | [`WogoumarketOrderV004CancelAndReorderZongziTask`](./order_v004_cancel_and_reorder_zongzi.md) | 0/3 | 4/20/40 | 478s |
| ❌ | [`WogoumarketOrderV005PendingOrderChangeAddressTask`](./order_v005_pending_order_change_address.md) | 0/3 | 28/25/20 | 479s |
| ❌ | [`WogoumarketOrderV039RenewSavingCardTask`](./order_v039_renew_saving_card.md) | 0/3 | 10/6/4 | 140s |
| ❌ | [`WogoumarketOrderV047CancelAndRebuyZongziTask`](./order_v047_cancel_and_rebuy_zongzi.md) | 0/3 | 5/5/5 | 113s |
| ❌ | [`WogoumarketSearchV006SearchEggViewAndCheckoutTask`](./search_v006_search_egg_view_and_checkout.md) | 0/3 | 6/6/6 | 131s |
| ❌ | [`WogoumarketSearchV007SearchGrapeMostExpensiveCheckoutTask`](./search_v007_search_grape_most_expensive_checkout.md) | 0/3 | 19/9/80 | 804s |
| ❌ | [`WogoumarketSearchV008SearchZongziCheapestCheckoutTask`](./search_v008_search_zongzi_cheapest_checkout.md) | 0/3 | 6/9/20 | 255s |
