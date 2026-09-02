# StockMovementApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getStockMovement**](StockMovementApi.md#getStockMovement) | **GET** /api/v1/stock-movements/{movement_id} |  |
| [**listStockMovements**](StockMovementApi.md#listStockMovements) | **GET** /api/v1/stock-movements/ |  |


<a id="getStockMovement"></a>
# **getStockMovement**
> StockMovement getStockMovement(movementId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockMovementApi()
val movementId : kotlin.String = movementId_example // kotlin.String | 
try {
    val result : StockMovement = apiInstance.getStockMovement(movementId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StockMovementApi#getStockMovement")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockMovementApi#getStockMovement")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **movementId** | **kotlin.String**|  | |

### Return type

[**StockMovement**](StockMovement.md)

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

<a id="listStockMovements"></a>
# **listStockMovements**
> kotlin.collections.List&lt;StockMovement&gt; listStockMovements(page, pageSize, productId, warehouseId, movementType, from, to)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockMovementApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val movementType : kotlin.String = movementType_example // kotlin.String | 
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only movements on or after this date (inclusive).
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only movements on or before this date (inclusive).
try {
    val result : kotlin.collections.List<StockMovement> = apiInstance.listStockMovements(page, pageSize, productId, warehouseId, movementType, from, to)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StockMovementApi#listStockMovements")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockMovementApi#listStockMovements")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **productId** | **java.util.UUID**|  | [optional] |
| **warehouseId** | **kotlin.String**|  | [optional] |
| **movementType** | **kotlin.String**|  | [optional] |
| **from** | **java.time.LocalDate**| Only movements on or after this date (inclusive). | [optional] |
| **to** | **java.time.LocalDate**| Only movements on or before this date (inclusive). | [optional] |

### Return type

[**kotlin.collections.List&lt;StockMovement&gt;**](StockMovement.md)

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

