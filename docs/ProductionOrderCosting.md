
# ProductionOrderCosting

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **costPerUnit** | **kotlin.String** | material_cost_total ÷ quantity. |  |
| **costSource** | **kotlin.String** | \&quot;actual\&quot; when costed from stock-movement consumption, else \&quot;planned\&quot;. |  |
| **lines** | [**kotlin.collections.List&lt;CostingLine&gt;**](CostingLine.md) |  |  |
| **materialCostTotal** | **kotlin.String** | Total material cost for the whole order. |  |
| **orderNumber** | **kotlin.String** |  |  |
| **productionOrderId** | [**java.util.UUID**](java.util.UUID.md) |  |  |
| **quantity** | **kotlin.Long** |  |  |
| **status** | **kotlin.String** |  |  |
| **marginPerUnit** | **kotlin.String** | sale_price − cost_per_unit. |  [optional] |
| **marginPercent** | **kotlin.String** | margin_per_unit ÷ cost_per_unit as a percentage. |  [optional] |
| **salePrice** | **kotlin.String** | Finished product&#39;s sale price per unit (used to compute margin). |  [optional] |



