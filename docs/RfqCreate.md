
# RfqCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. |  |
| **requestedDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **rfqNumber** | **kotlin.String** |  |  |
| **status** | [**RfqStatus**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted |  |
| **currency** | **kotlin.String** |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **responseDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **supplierContactId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **supplierName** | **kotlin.String** |  |  [optional] |



