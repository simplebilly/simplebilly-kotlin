
# InventoryCount

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **countDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **countNumber** | **kotlin.String** |  |  |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, sku, expected_quantity, counted_quantity, bin_location?, batch_number?, variance}&#x60;. |  |
| **status** | [**InventoryCountStatus**](InventoryCountStatus.md) | One of: draft | counting | reviewed | posted |  |
| **warehouseId** | **kotlin.String** | References the warehouse entity. |  |
| **notes** | **kotlin.String** |  |  [optional] |



