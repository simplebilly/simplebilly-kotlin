
# InvoiceCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | [**CurrencyCode**](CurrencyCode.md) |  |  |
| **invoiceType** | [**InvoiceType**](InvoiceType.md) |  |  |
| **issueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **lineItems** | [**kotlin.Any**](.md) |  |  |
| **status** | [**InvoiceStatus**](InvoiceStatus.md) |  |  |
| **subtotal** | **kotlin.String** |  |  |
| **totalAmount** | **kotlin.String** |  |  |
| **totalTax** | **kotlin.String** |  |  |
| **attachments** | [**kotlin.Any**](.md) |  |  [optional] |
| **billingPeriodEnd** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **billingPeriodStart** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **cancellationDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **cancellationInvoiceId** | **kotlin.String** | References the invoice entity. |  [optional] |
| **cancellationReason** | **kotlin.String** |  |  [optional] |
| **contractId** | [**java.util.UUID**](java.util.UUID.md) | References the contract entity. |  [optional] |
| **customerId** | **kotlin.String** | References the customer entity. |  [optional] |
| **discountAmount** | **kotlin.String** |  |  [optional] |
| **discountDays** | **kotlin.Int** |  |  [optional] |
| **discountPercentage** | **kotlin.String** |  |  [optional] |
| **documentType** | [**DocumentType**](DocumentType.md) |  |  [optional] |
| **dunningLevel** | **kotlin.Int** |  |  [optional] |
| **inputVatAmount** | **kotlin.String** |  |  [optional] |
| **inputVatDeductible** | **kotlin.Boolean** |  |  [optional] |
| **inputVatPercentage** | **kotlin.String** |  |  [optional] |
| **introductionText** | **kotlin.String** |  |  [optional] |
| **isCancelled** | **kotlin.Boolean** |  |  [optional] |
| **isDraft** | **kotlin.Boolean** |  |  [optional] |
| **isEuAcquisition** | **kotlin.Boolean** |  |  [optional] |
| **isEuDelivery** | **kotlin.Boolean** |  |  [optional] |
| **isIntraCommunityAcquisition** | **kotlin.Boolean** |  |  [optional] |
| **isReverseCharge** | **kotlin.Boolean** |  |  [optional] |
| **ledgerAccount** | **kotlin.String** |  |  [optional] |
| **margin25a** | **kotlin.Boolean** |  |  [optional] |
| **margin25aGross** | **kotlin.String** |  |  [optional] |
| **margin25aPurchasePrice** | **kotlin.String** |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **orderNumber** | **kotlin.String** |  |  [optional] |
| **originalPdfPath** | **kotlin.String** |  |  [optional] |
| **paidAmount** | **kotlin.String** |  |  [optional] |
| **paymentDueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **paymentStatus** | [**PaymentStatus**](PaymentStatus.md) |  |  [optional] |
| **paymentTermsText** | **kotlin.String** |  |  [optional] |
| **precedingSalesVoucherId** | **kotlin.String** | References the preceding sales voucher entity. |  [optional] |
| **precedingSalesVoucherType** | [**PrecedingSalesVoucherType**](PrecedingSalesVoucherType.md) |  |  [optional] |
| **receiptConfirmationAvailable** | **kotlin.Boolean** |  |  [optional] |
| **relatedInvoiceId** | [**java.util.UUID**](java.util.UUID.md) | References the invoice entity. |  [optional] |
| **relationshipType** | **kotlin.String** |  |  [optional] |
| **senderSnapshot** | [**kotlin.Any**](.md) |  |  [optional] |
| **sentAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **servicePeriodEnd** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **servicePeriodStart** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **supplierId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **taxExemptionReason** | **kotlin.String** |  |  [optional] |
| **vatCountry** | [**CountryCode**](CountryCode.md) |  |  [optional] |
| **vatSpecialCase** | **kotlin.String** |  |  [optional] |



