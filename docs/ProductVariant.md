
# ProductVariant

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The parent product this variant belongs to. References the product entity. |  |
| **sku** | **kotlin.String** | Variant-specific SKU (must be unique per tenant). |  |
| **barcode** | **kotlin.String** |  |  [optional] |
| **imageLink** | **kotlin.String** |  |  [optional] |
| **isActive** | **kotlin.Boolean** |  |  [optional] |
| **name** | **kotlin.String** | Human-readable variant label, e.g. \&quot;Red / M\&quot;. |  [optional] |
| **optionValues** | [**kotlin.Any**](.md) | Option name → value map, e.g. &#x60;{\&quot;Color\&quot;: \&quot;Red\&quot;, \&quot;Size\&quot;: \&quot;M\&quot;}&#x60;. |  [optional] |
| **price** | **kotlin.String** | Explicit override price for this variant (takes precedence over parent price + delta). |  [optional] |
| **priceDelta** | **kotlin.String** | Price adjustment relative to the parent product&#39;s &#x60;default_price&#x60;. |  [optional] |
| **stockQuantity** | **kotlin.Long** | Variant-level stock (optional — may be tracked on the parent only). |  [optional] |



