# ReorderProposalApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**applyReorderProposal**](ReorderProposalApi.md#applyReorderProposal) | **POST** /api/v1/reorder-proposals/apply | Convert a reorder proposal into a draft purchase order. |
| [**getReorderProposal**](ReorderProposalApi.md#getReorderProposal) | **GET** /api/v1/reorder-proposals |  |


<a id="applyReorderProposal"></a>
# **applyReorderProposal**
> kotlin.Any applyReorderProposal(configuredOnly, warehouseId)

Convert a reorder proposal into a draft purchase order.

Returns the created purchase order id. Suggested line items are generated with the current reorder quantity per product.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReorderProposalApi()
val configuredOnly : kotlin.Boolean = true // kotlin.Boolean | Only include products with a reorder point configured (`min_stock`).
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | Limit to a single warehouse id.
try {
    val result : kotlin.Any = apiInstance.applyReorderProposal(configuredOnly, warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReorderProposalApi#applyReorderProposal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReorderProposalApi#applyReorderProposal")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **configuredOnly** | **kotlin.Boolean**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] |
| **warehouseId** | **kotlin.String**| Limit to a single warehouse id. | [optional] |

### Return type

[**kotlin.Any**](kotlin.Any.md)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="getReorderProposal"></a>
# **getReorderProposal**
> ReorderProposalResponse getReorderProposal(configuredOnly, warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReorderProposalApi()
val configuredOnly : kotlin.Boolean = true // kotlin.Boolean | Only include products with a reorder point configured (`min_stock`).
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | Limit to a single warehouse id.
try {
    val result : ReorderProposalResponse = apiInstance.getReorderProposal(configuredOnly, warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReorderProposalApi#getReorderProposal")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReorderProposalApi#getReorderProposal")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **configuredOnly** | **kotlin.Boolean**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] |
| **warehouseId** | **kotlin.String**| Limit to a single warehouse id. | [optional] |

### Return type

[**ReorderProposalResponse**](ReorderProposalResponse.md)

### Authorization


Configure bearer_token statically:
```kotlin
ApiClient.accessToken = ""
```
Configure bearer_token dynamically:
```kotlin
apiInstance.accessTokenProvider = { "" }
```

### HTTP request headers

 - **Content-Type**: Not defined
 - **Accept**: application/json

