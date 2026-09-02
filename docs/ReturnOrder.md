
# ReturnOrder

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **returnNumber** | **kotlin.String** |  |  |
| **status** | [**ReturnOrderStatus**](ReturnOrderStatus.md) | One of: requested | received | inspected | restocked | closed |  |
| **customerContactId** | **kotlin.String** | References the contact entity. |  [optional] |
| **customerName** | **kotlin.String** |  |  [optional] |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, condition, restock, batch_number?}&#x60;. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **orderId** | **kotlin.String** | References the order entity. |  [optional] |
| **orderNumber** | **kotlin.String** |  |  [optional] |
| **returnReason** | **kotlin.String** |  |  [optional] |
| **warehouseId** | **kotlin.String** | Warehouse into which restockable items are returned. References the warehouse entity. |  [optional] |



