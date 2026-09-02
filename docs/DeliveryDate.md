
# DeliveryDate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String** | Sales order number (&#x60;order.order_number&#x60;). |  |
| **promisedDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Date promised to the customer. |  |
| **status** | [**DeliveryDateStatus**](DeliveryDateStatus.md) | One of: promised | confirmed | rescheduled | fulfilled | late | cancelled |  |
| **customerId** | **kotlin.String** | References the customer entity. |  [optional] |
| **fulfilledDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Date actually delivered (set on fulfillment). |  [optional] |
| **note** | **kotlin.String** |  |  [optional] |
| **originalDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Original date promised before rescheduling. |  [optional] |
| **productId** | **kotlin.String** | Product line item this date applies to, if per-item. References the product entity. |  [optional] |



