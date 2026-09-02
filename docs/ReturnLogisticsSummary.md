
# ReturnLogisticsSummary

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **byStatus** | [**kotlin.Any**](.md) | Number of return orders per status. |  |
| **byWarehouse** | [**kotlin.collections.List&lt;ReturnWarehouseSummary&gt;**](ReturnWarehouseSummary.md) | Per-warehouse aggregation. |  |
| **itemsRestocked** | **kotlin.Long** | Sum of &#x60;restock: true&#x60; line-item quantities. |  |
| **itemsScrapped** | **kotlin.Long** | Sum of &#x60;restock: false&#x60; line-item quantities (scrapped/disposed). |  |
| **totalItems** | **kotlin.Long** | Sum of all line-item quantities across returns. |  |
| **totalReturns** | **kotlin.Long** | Total number of return orders (excluding soft-deleted). |  |



