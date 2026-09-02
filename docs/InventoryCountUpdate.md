
# InventoryCountUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **countDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **countNumber** | **kotlin.String** |  |  [optional] |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, sku, expected_quantity, counted_quantity, bin_location?, batch_number?, variance}&#x60;. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **status** | [**InventoryCountStatus**](InventoryCountStatus.md) | One of: draft | counting | reviewed | posted |  [optional] |
| **warehouseId** | **kotlin.String** | References the warehouse entity. |  [optional] |



