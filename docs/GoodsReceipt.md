
# GoodsReceipt

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **grNumber** | **kotlin.String** |  |  |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, batch_number?, expiry_date?, bin_location?}&#x60;. |  |
| **receiptDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **warehouseId** | **kotlin.String** | References the warehouse entity. |  |
| **notes** | **kotlin.String** |  |  [optional] |
| **purchaseOrderId** | **kotlin.String** | References the purchase order entity. |  [optional] |
| **supplierContactId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **supplierName** | **kotlin.String** |  |  [optional] |



