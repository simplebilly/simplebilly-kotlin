
# ProductAttributeCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Attribute name, e.g. &#x60;Material&#x60;, &#x60;Farbe&#x60;, &#x60;Gewicht&#x60;. |  |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The product this attribute belongs to. References the product entity. |  |
| **&#x60;value&#x60;** | **kotlin.String** | Attribute value, e.g. &#x60;Baumwolle&#x60;, &#x60;Rot&#x60;, &#x60;180g&#x60;. |  |
| **isFilterable** | **kotlin.Boolean** | Whether this attribute participates in the shop&#39;s faceted filters. |  [optional] |
| **position** | **kotlin.Int** | Ordering position within the product&#39;s attribute list. |  [optional] |
| **unit** | **kotlin.String** | Optional unit of measure for numeric attributes, e.g. &#x60;g&#x60;, &#x60;cm&#x60;. |  [optional] |



