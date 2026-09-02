
# ProformaInvoiceCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | [**CurrencyCode**](CurrencyCode.md) |  |  |
| **issueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **lineItems** | [**kotlin.Any**](.md) |  |  |
| **status** | [**ProformaInvoiceStatus**](ProformaInvoiceStatus.md) | &#x60;draft&#x60; | &#x60;sent&#x60; | &#x60;converted&#x60;. |  |
| **subtotal** | **kotlin.String** |  |  |
| **totalAmount** | **kotlin.String** |  |  |
| **totalTax** | **kotlin.String** |  |  |
| **convertedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **convertedToInvoiceId** | **kotlin.String** | Set when the proforma was converted into a real invoice. References the invoice entity. |  [optional] |
| **customerId** | **kotlin.String** | References the customer entity. |  [optional] |
| **customerSnapshot** | [**kotlin.Any**](.md) | Snapshot of the recipient at issue time (address, VAT id, …). |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **orderNumber** | **kotlin.String** | Reference to the order/quote this proforma belongs to. |  [optional] |
| **paymentDueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Optional deadline the real invoice should carry after conversion. |  [optional] |
| **quotationId** | **kotlin.String** | References the quotation entity. |  [optional] |



