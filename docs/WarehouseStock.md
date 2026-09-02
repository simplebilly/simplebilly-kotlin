
# WarehouseStock

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **productId** | [**java.util.UUID**](java.util.UUID.md) |  |  |
| **quantity** | **kotlin.Long** |  |  |
| **warehouseId** | **kotlin.String** |  |  |
| **batchNumber** | **kotlin.String** | Batch/lot number (Chargennummer) — &#x60;None&#x60; for non-batched goods. |  [optional] |
| **binLocation** | **kotlin.String** |  |  [optional] |
| **expiryDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Expiry date for batch-tracked goods. |  [optional] |
| **serialNumbers** | [**kotlin.Any**](.md) | JSON array of serial numbers (Seriennummern) in this stock row. |  [optional] |



