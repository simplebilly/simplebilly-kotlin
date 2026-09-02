
# SupplierInvoiceUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** |  |  [optional] |
| **goodsReceiptId** | **kotlin.String** | References the goods receipt entity. |  [optional] |
| **invoiceDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **invoiceNumber** | **kotlin.String** |  |  [optional] |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, unitPriceNet, taxRate}&#x60;. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **purchaseOrderId** | **kotlin.String** | References the purchase order entity. |  [optional] |
| **status** | [**SupplierInvoiceStatus**](SupplierInvoiceStatus.md) | One of: draft | matched | has_variances | posted | cancelled |  [optional] |
| **supplierContactId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **supplierName** | **kotlin.String** |  |  [optional] |
| **totalGrossAmount** | **kotlin.String** |  |  [optional] |
| **totalNetAmount** | **kotlin.String** |  |  [optional] |



