> ⚠️  **候选池清理建议（pipeline 预检发现 N 个 slug 在容器里没注册）**
>
> 以下 **39** 个 slug 来自 `/Users/zhangrunsheng/Documents/GitHub/box/Kangoo/db/validator_statuses.json` 但容器 vendor_android_env 里没注册对应 task class，已自动跳过（避免死循环重启 emulator）。
>
> 建议在下次跑 pipeline 前去 validator_statuses.json 把这些 key 删掉：
>
> | web_slug | 推算的 class |
> |----------|--------------|
> | `kanbing_v001_add_medicine_to_cart` | `DaishushenghuoKanbingV001AddMedicineToCartTask` |
> | `kanbing_v002_add_medicine_qty2` | `DaishushenghuoKanbingV002AddMedicineQty2Task` |
> | `kanbing_v003_add_multi_medicines` | `DaishushenghuoKanbingV003AddMultiMedicinesTask` |
> | `kanbing_v004_update_medicine_quantity` | `DaishushenghuoKanbingV004UpdateMedicineQuantityTask` |
> | `kanbing_v005_clear_medicine_cart` | `DaishushenghuoKanbingV005ClearMedicineCartTask` |
> | `kanbing_v006_buy_at_cheapest_pharmacy` | `DaishushenghuoKanbingV006BuyAtCheapestPharmacyTask` |
> | `kanbing_v007_add_via_chuncung_sheet` | `DaishushenghuoKanbingV007AddViaChuncungSheetTask` |
> | `kanbing_v008_carts_across_pharmacies` | `DaishushenghuoKanbingV008CartsAcrossPharmaciesTask` |
> | `kanbing_v009_place_order_nanbei` | `DaishushenghuoKanbingV009PlaceOrderNanbeiTask` |
> | `kanbing_v010_place_order_dashenlin` | `DaishushenghuoKanbingV010PlaceOrderDashenlinTask` |
> | `kanbing_v011_place_order_renhe` | `DaishushenghuoKanbingV011PlaceOrderRenheTask` |
> | `kanbing_v012_place_order_qty2` | `DaishushenghuoKanbingV012PlaceOrderQty2Task` |
> | `kanbing_v013_place_order_multi_items` | `DaishushenghuoKanbingV013PlaceOrderMultiItemsTask` |
> | `kanbing_v014_cancel_medicine_order` | `DaishushenghuoKanbingV014CancelMedicineOrderTask` |
> | `kanbing_v015_cancel_dashenlin_order` | `DaishushenghuoKanbingV015CancelDashenlinOrderTask` |
> | `kanbing_v016_pay_medicine_order` | `DaishushenghuoKanbingV016PayMedicineOrderTask` |
> | `kanbing_v017_pay_renhe_order` | `DaishushenghuoKanbingV017PayRenheOrderTask` |
> | `kanbing_v018_reset_and_add_medicine` | `DaishushenghuoKanbingV018ResetAndAddMedicineTask` |
> | `kanbing_v019_place_order_tainuolin` | `DaishushenghuoKanbingV019PlaceOrderTainuolinTask` |
> | `kanbing_v020_place_order_three_medicines` | `DaishushenghuoKanbingV020PlaceOrderThreeMedicinesTask` |
> | `kanbing_v021_pay_laobaixing_qty2` | `DaishushenghuoKanbingV021PayLaobaixingQty2Task` |
> | `kanbing_v022_pay_haiwang_multi` | `DaishushenghuoKanbingV022PayHaiwangMultiTask` |
> | `kanbing_v023_pay_dashenlin_pinjian` | `DaishushenghuoKanbingV023PayDashenlinPinjianTask` |
> | `kanbing_v024_pay_minghua_taino` | `DaishushenghuoKanbingV024PayMinghuaTainoTask` |
> | `kanbing_v025_pay_nanbei_three` | `DaishushenghuoKanbingV025PayNanbeiThreeTask` |
> | `kanbing_v026_buy_laobaixing_qty2` | `DaishushenghuoKanbingV026BuyLaobaixingQty2Task` |
> | `kanbing_v027_buy_haiwang_multi` | `DaishushenghuoKanbingV027BuyHaiwangMultiTask` |
> | `kanbing_v028_buy_nanbei_pinjian` | `DaishushenghuoKanbingV028BuyNanbeiPinjianTask` |
> | `kanbing_v029_buy_minghua_taino` | `DaishushenghuoKanbingV029BuyMinghuaTainoTask` |
> | `kanbing_v030_buy_dashenlin_three` | `DaishushenghuoKanbingV030BuyDashenlinThreeTask` |
> | `kanbing_v031_add_banlangen_haiwang` | `DaishushenghuoKanbingV031AddBanlangenHaiwangTask` |
> | `kanbing_v032_update_amoxi_qty4` | `DaishushenghuoKanbingV032UpdateAmoxiQty4Task` |
> | `kanbing_v033_clear_dashenlin_cart` | `DaishushenghuoKanbingV033ClearDashenlinCartTask` |
> | `kanbing_v034_cheapest_shuanghuanglian` | `DaishushenghuoKanbingV034CheapestShuanghuanglianTask` |
> | `kanbing_v035_add_via_chuncung_ganmaoling` | `DaishushenghuoKanbingV035AddViaChuncungGanmaolingTask` |
> | `kanbing_v037_place_order_xiaochaihu` | `DaishushenghuoKanbingV037PlaceOrderXiaochaihuTask` |
> | `kanbing_v038_cancel_minghua_order` | `DaishushenghuoKanbingV038CancelMinghuaOrderTask` |
> | `kanbing_v039_pay_renhe_shuanghuanglian` | `DaishushenghuoKanbingV039PayRenheShuanghuanglianTask` |
> | `kanbing_v041_buy_nanbei_three_flow` | `DaishushenghuoKanbingV041BuyNanbeiThreeFlowTask` |
>
> **快速清理命令**：
> ```bash
> cd /Users/zhangrunsheng/Documents/GitHub/box/Kangoo
> # 用 jq 删掉 UUID 形态的 key（备份再删）
> cp db/validator_statuses.json db/validator_statuses.json.bak
> jq 'with_entries(select(.key | test("^[0-9a-f]{8}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{4}-[0-9a-f]{12}$") | not))' db/validator_statuses.json.bak > db/validator_statuses.json
> ```

# Pass@3 Report — daishushenghuo — 20260513_014438

## Summary

- ❌ 预检后没有可跑 slug（候选池里 39 个全部在容器里没注册）
- 请按下方「候选池清理建议」清理 `db/validator_statuses.json` 后重跑 pipeline

