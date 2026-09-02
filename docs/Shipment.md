
# Shipment

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **orderId** | **kotlin.String** | References the order entity. |  |
| **shipmentDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **shippingCarrier** | **kotlin.String** |  |  |
| **status** | **kotlin.String** |  |  |
| **deliveredAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **labelUrl** | **kotlin.String** |  |  [optional] |
| **lineItemsShipment** | [**kotlin.Any**](.md) |  |  [optional] |
| **recipientAddress** | [**kotlin.Any**](.md) |  |  [optional] |
| **shippingCost** | **kotlin.String** |  |  [optional] |
| **shippingMethod** | **kotlin.String** |  |  [optional] |
| **signedBy** | **kotlin.String** |  |  [optional] |
| **trackingEvents** | [**kotlin.Any**](.md) | Latest carrier tracking events (from the live tracking API). |  [optional] |
| **trackingNumber** | **kotlin.String** |  |  [optional] |
| **trackingUrl** | **kotlin.String** |  |  [optional] |
| **weightKg** | **kotlin.Double** |  |  [optional] |



