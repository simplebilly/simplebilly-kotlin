# StockTransferApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createStockTransfer**](StockTransferApi.md#createStockTransfer) | **POST** /api/v1/stock-transfers |  |
| [**deleteStockTransfer**](StockTransferApi.md#deleteStockTransfer) | **DELETE** /api/v1/stock-transfers/{stock_transfer_id} |  |
| [**getStockTransfer**](StockTransferApi.md#getStockTransfer) | **GET** /api/v1/stock-transfers/{stock_transfer_id} |  |
| [**listStockTransfers**](StockTransferApi.md#listStockTransfers) | **GET** /api/v1/stock-transfers/ |  |
| [**updateStockTransferStatus**](StockTransferApi.md#updateStockTransferStatus) | **PUT** /api/v1/stock-transfers/{stock_transfer_id}/status |  |


<a id="createStockTransfer"></a>
# **createStockTransfer**
> StockTransfer createStockTransfer(stockTransfer)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockTransferApi()
val stockTransfer : StockTransfer =  // StockTransfer | 
try {
    val result : StockTransfer = apiInstance.createStockTransfer(stockTransfer)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StockTransferApi#createStockTransfer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockTransferApi#createStockTransfer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stockTransfer** | [**StockTransfer**](StockTransfer.md)|  | |

### Return type

[**StockTransfer**](StockTransfer.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteStockTransfer"></a>
# **deleteStockTransfer**
> deleteStockTransfer(stockTransferId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockTransferApi()
val stockTransferId : kotlin.String = stockTransferId_example // kotlin.String | 
try {
    apiInstance.deleteStockTransfer(stockTransferId)
} catch (e: ClientException) {
    println("4xx response calling StockTransferApi#deleteStockTransfer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockTransferApi#deleteStockTransfer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stockTransferId** | **kotlin.String**|  | |

### Return type

null (empty response body)

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

<a id="getStockTransfer"></a>
# **getStockTransfer**
> StockTransfer getStockTransfer(stockTransferId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockTransferApi()
val stockTransferId : kotlin.String = stockTransferId_example // kotlin.String | 
try {
    val result : StockTransfer = apiInstance.getStockTransfer(stockTransferId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StockTransferApi#getStockTransfer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockTransferApi#getStockTransfer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stockTransferId** | **kotlin.String**|  | |

### Return type

[**StockTransfer**](StockTransfer.md)

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

<a id="listStockTransfers"></a>
# **listStockTransfers**
> kotlin.collections.List&lt;StockTransfer&gt; listStockTransfers(page, pageSize, status, warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockTransferApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<StockTransfer> = apiInstance.listStockTransfers(page, pageSize, status, warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StockTransferApi#listStockTransfers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockTransferApi#listStockTransfers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **warehouseId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;StockTransfer&gt;**](StockTransfer.md)

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

<a id="updateStockTransferStatus"></a>
# **updateStockTransferStatus**
> StockTransfer updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StockTransferApi()
val stockTransferId : kotlin.String = stockTransferId_example // kotlin.String | 
val stockTransferStatusUpdate : StockTransferStatusUpdate =  // StockTransferStatusUpdate | 
try {
    val result : StockTransfer = apiInstance.updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StockTransferApi#updateStockTransferStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StockTransferApi#updateStockTransferStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **stockTransferId** | **kotlin.String**|  | |
| **stockTransferStatusUpdate** | [**StockTransferStatusUpdate**](StockTransferStatusUpdate.md)|  | |

### Return type

[**StockTransfer**](StockTransfer.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

