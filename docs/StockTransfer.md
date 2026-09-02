
# StockTransfer

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, batch_number?}&#x60;. |  |
| **sourceWarehouseId** | **kotlin.String** | References the warehouse entity. |  |
| **status** | [**StockTransferStatus**](StockTransferStatus.md) | One of: draft | completed | cancelled |  |
| **targetWarehouseId** | **kotlin.String** | References the warehouse entity. |  |
| **transferDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **transferNumber** | **kotlin.String** |  |  |
| **notes** | **kotlin.String** |  |  [optional] |



