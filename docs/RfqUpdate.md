
# RfqUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** |  |  [optional] |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **requestedDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **responseDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **rfqNumber** | **kotlin.String** |  |  [optional] |
| **status** | [**RfqStatus**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted |  [optional] |
| **supplierContactId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **supplierName** | **kotlin.String** |  |  [optional] |



