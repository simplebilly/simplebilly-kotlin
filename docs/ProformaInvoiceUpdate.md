
# ProformaInvoiceUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **convertedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **convertedToInvoiceId** | **kotlin.String** | Set when the proforma was converted into a real invoice. References the invoice entity. |  [optional] |
| **currency** | [**CurrencyCode**](CurrencyCode.md) |  |  [optional] |
| **customerId** | **kotlin.String** | References the customer entity. |  [optional] |
| **customerSnapshot** | [**kotlin.Any**](.md) | Snapshot of the recipient at issue time (address, VAT id, …). |  [optional] |
| **issueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **lineItems** | [**kotlin.Any**](.md) |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **orderNumber** | **kotlin.String** | Reference to the order/quote this proforma belongs to. |  [optional] |
| **paymentDueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Optional deadline the real invoice should carry after conversion. |  [optional] |
| **quotationId** | **kotlin.String** | References the quotation entity. |  [optional] |
| **status** | [**ProformaInvoiceStatus**](ProformaInvoiceStatus.md) | &#x60;draft&#x60; | &#x60;sent&#x60; | &#x60;converted&#x60;. |  [optional] |
| **subtotal** | **kotlin.String** |  |  [optional] |
| **totalAmount** | **kotlin.String** |  |  [optional] |
| **totalTax** | **kotlin.String** |  |  [optional] |



