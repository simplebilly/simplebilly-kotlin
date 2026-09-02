
# SupplierConditionCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** | Currency for the minimum order value. |  |
| **supplierContactId** | **kotlin.String** | The supplier this condition applies to (&#x60;contact_id&#x60;). References the supplier entity. |  |
| **deliveryTerms** | **kotlin.String** | Incoterms, e.g. \&quot;EXW\&quot;, \&quot;DAP\&quot;. |  [optional] |
| **earlyPaymentDiscountPercent** | **kotlin.String** | Early-payment discount percentage (Skonto), e.g. 2.0. |  [optional] |
| **isDefault** | **kotlin.Boolean** | Is this the default condition for the supplier? |  [optional] |
| **minimumOrderValue** | **kotlin.String** | Minimum order value required for this supplier. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **paymentDueDays** | **kotlin.Int** | Number of days within which payment is due. |  [optional] |
| **paymentTerms** | **kotlin.String** | Payment terms, e.g. \&quot;14 Tage, 2% Skonto\&quot;. |  [optional] |
| **supplierName** | **kotlin.String** | The name of the supplier, denormalized for easy listing. |  [optional] |
| **volumeDiscountTiers** | [**kotlin.Any**](.md) | Tiered discounts: JSON array of &#x60;{min_quantity, discount_percent}&#x60;. |  [optional] |



