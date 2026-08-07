> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **1** 个 slug 来自 `/Users/zhangrunsheng/Documents/GitHub/box/duvy/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `identify_v001_create_luxury_bag_order` | `DuwuIdentifyV001CreateLuxuryBagOrderTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/zhangrunsheng/Documents/GitHub/box/duvy
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — duwu — 20260807_174417

## Summary

- Total tasks: **15**
- ✅ All passed (3/3): **0**
- ⚠️  Partial (1-2 / 3): **15**
- ❌ Failed (0/3): **0**
- Total elapsed: 3707s (61.8 min)

## Tasks

| Status | Task | Pass@3 | Steps (ep1/ep2/ep3) | Elapsed |
|--------|------|--------|---------------------|---------|
| ⚠️ | [`DuwuFeedLikeV003UnlikePostTask`](./feed_like_v003_unlike_post.md) | 1/3 | 9/?/? | 82s |
| ⚠️ | [`DuwuFeedLikeV004LikeWithExclusionTask`](./feed_like_v004_like_with_exclusion.md) | 1/3 | 15/?/? | 154s |
| ⚠️ | [`DuwuIdentifyV002CreateWatchOrderTask`](./identify_v002_create_watch_order.md) | 1/3 | 24/?/? | 237s |
| ⚠️ | [`DuwuIdentifyV003CreatePhysicalOrderTask`](./identify_v003_create_physical_order.md) | 1/3 | 20/21/? | 557s |
| ⚠️ | [`DuwuIdentifyV004CreateDualOrderTask`](./identify_v004_create_dual_order.md) | 1/3 | 27/?/? | 298s |
| ⚠️ | [`DuwuOrderV001BuyProductTask`](./order_v001_buy_product.md) | 1/3 | 23/?/? | 265s |
| ⚠️ | [`DuwuOrderV008BuyCheapItemTask`](./order_v008_buy_cheap_item.md) | 1/3 | 11/?/? | 251s |
| ⚠️ | [`DuwuOrderV009BuyWithNewAddressTask`](./order_v009_buy_with_new_address.md) | 1/3 | 13/16/? | 342s |
| ⚠️ | [`DuwuPostV002CreatePostWithTopicsTask`](./post_v002_create_post_with_topics.md) | 1/3 | 39/?/? | 403s |
| ⚠️ | [`DuwuPostV006CreatePostWithImageTask`](./post_v006_create_post_with_image.md) | 1/3 | 16/?/? | 145s |
| ⚠️ | [`DuwuReviewV008MarkUntrueAndCommentMedihealReviewTask`](./review_v008_mark_untrue_and_comment_mediheal_review.md) | 1/3 | 12/?/? | 107s |
| ⚠️ | [`DuwuSkuV003ViewRestockWishlistTask`](./sku_v003_view_restock_wishlist.md) | 1/3 | 8/?/? | 99s |
| ⚠️ | [`DuwuSkuV010BuyJacketWishPantsBuyBackpackTask`](./sku_v010_buy_jacket_wish_pants_buy_backpack.md) | 1/3 | 54/?/? | 604s |
| ⚠️ | [`DuwuWalletV010RepayOneTask`](./wallet_v010_repay_one.md) | 1/3 | 8/?/? | 88s |
| ⚠️ | [`DuwuWalletV012UnbindIcbcTask`](./wallet_v012_unbind_icbc.md) | 1/3 | 8/?/? | 75s |
