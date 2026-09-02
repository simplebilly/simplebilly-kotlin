# ReplenishmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**applyReplenishments**](ReplenishmentApi.md#applyReplenishments) | **POST** /api/v1/replenishments/apply | Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair. |
| [**getReplenishments**](ReplenishmentApi.md#getReplenishments) | **GET** /api/v1/replenishments |  |


<a id="applyReplenishments"></a>
# **applyReplenishments**
> kotlin.Any applyReplenishments(targetWarehouseId, sourceWarehouseId)

Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReplenishmentApi()
val targetWarehouseId : kotlin.String = targetWarehouseId_example // kotlin.String | Warehouse to be replenished. Defaults to the tenant's default warehouse.
val sourceWarehouseId : kotlin.String = sourceWarehouseId_example // kotlin.String | Restrict source warehouses to this id.
try {
    val result : kotlin.Any = apiInstance.applyReplenishments(targetWarehouseId, sourceWarehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReplenishmentApi#applyReplenishments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReplenishmentApi#applyReplenishments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **targetWarehouseId** | **kotlin.String**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] |
| **sourceWarehouseId** | **kotlin.String**| Restrict source warehouses to this id. | [optional] |

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

<a id="getReplenishments"></a>
# **getReplenishments**
> ReplenishmentResponse getReplenishments(targetWarehouseId, sourceWarehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReplenishmentApi()
val targetWarehouseId : kotlin.String = targetWarehouseId_example // kotlin.String | Warehouse to be replenished. Defaults to the tenant's default warehouse.
val sourceWarehouseId : kotlin.String = sourceWarehouseId_example // kotlin.String | Restrict source warehouses to this id.
try {
    val result : ReplenishmentResponse = apiInstance.getReplenishments(targetWarehouseId, sourceWarehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReplenishmentApi#getReplenishments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReplenishmentApi#getReplenishments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **targetWarehouseId** | **kotlin.String**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] |
| **sourceWarehouseId** | **kotlin.String**| Restrict source warehouses to this id. | [optional] |

### Return type

[**ReplenishmentResponse**](ReplenishmentResponse.md)

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

