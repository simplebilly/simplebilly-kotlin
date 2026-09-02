
# ProductionOrder

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String** |  |  |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | The finished product to manufacture. References the product entity. |  |
| **quantity** | **kotlin.Long** | Quantity of finished product to produce. |  |
| **bomId** | [**java.util.UUID**](java.util.UUID.md) | References the BOM entity. |  [optional] |
| **components** | [**kotlin.Any**](.md) | JSON snapshot of the BOM components at creation time. |  [optional] |
| **endDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **sourceWarehouseId** | **kotlin.String** | Warehouse components are consumed from. References the warehouse entity. |  [optional] |
| **startDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **status** | [**ProductionOrderStatus**](ProductionOrderStatus.md) | One of: planned | in_production | completed | cancelled |  [optional] |
| **targetWarehouseId** | **kotlin.String** | Warehouse the finished product is added to. References the warehouse entity. |  [optional] |



