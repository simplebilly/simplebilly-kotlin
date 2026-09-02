
# PurchaseOrderUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** |  |  [optional] |
| **deliveryAddress** | [**kotlin.Any**](.md) |  |  [optional] |
| **expectedDeliveryDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, unit_price_net, tax_rate, delivery_date}&#x60;. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **orderDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **poNumber** | **kotlin.String** |  |  [optional] |
| **status** | [**PurchaseOrderStatus**](PurchaseOrderStatus.md) | One of: draft | ordered | partially_received | received | cancelled |  [optional] |
| **supplierContactId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **supplierName** | **kotlin.String** |  |  [optional] |
| **totalGrossAmount** | **kotlin.String** |  |  [optional] |
| **totalNetAmount** | **kotlin.String** |  |  [optional] |



