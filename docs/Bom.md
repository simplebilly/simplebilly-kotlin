
# Bom

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** |  |  |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The finished product this BOM produces. References the product entity. |  |
| **components** | [**kotlin.Any**](.md) | JSON array of &#x60;{product_id, name, quantity, unit, scrap_rate}&#x60;. |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **outputQuantity** | **kotlin.Long** | Output quantity per production run (defaults to 1). |  [optional] |
| **status** | [**BomStatus**](BomStatus.md) | One of: draft | active | archived |  [optional] |



