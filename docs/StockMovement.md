
# StockMovement

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **delta** | **kotlin.Long** | Signed movement: positive &#x3D; into stock, negative &#x3D; out of stock. |  |
| **movementType** | [**MovementType**](MovementType.md) | One of the &#x60;MOVEMENT_*&#x60; constants. |  |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | References the product entity. |  |
| **quantity** | **kotlin.Long** | Absolute quantity moved (always &gt;&#x3D; 0). |  |
| **warehouseId** | **kotlin.String** | References the warehouse entity. |  |
| **reason** | **kotlin.String** |  |  [optional] |
| **referenceId** | **kotlin.String** | Primary-key of the referencing entity. |  [optional] |
| **referenceType** | [**ReferenceType**](ReferenceType.md) | Entity that caused the movement, e.g. &#x60;goods_receipt&#x60;, &#x60;stock_transfer&#x60;. |  [optional] |



