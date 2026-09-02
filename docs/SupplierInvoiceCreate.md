
# SupplierInvoiceCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **invoiceDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **invoiceNumber** | **kotlin.String** |  |  |
| **lineItems** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, unitPriceNet, taxRate}&#x60;. |  |
| **status** | [**SupplierInvoiceStatus**](SupplierInvoiceStatus.md) | One of: draft | matched | has_variances | posted | cancelled |  |
| **currency** | **kotlin.String** |  |  [optional] |
| **goodsReceiptId** | **kotlin.String** | References the goods receipt entity. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **purchaseOrderId** | **kotlin.String** | References the purchase order entity. |  [optional] |
| **supplierContactId** | **kotlin.String** | References the supplier entity. |  [optional] |
| **supplierName** | **kotlin.String** |  |  [optional] |
| **totalGrossAmount** | **kotlin.String** |  |  [optional] |
| **totalNetAmount** | **kotlin.String** |  |  [optional] |



