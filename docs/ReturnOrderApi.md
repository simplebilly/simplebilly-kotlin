# ReturnOrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createReturnOrder**](ReturnOrderApi.md#createReturnOrder) | **POST** /api/v1/returns |  |
| [**deleteReturnOrder**](ReturnOrderApi.md#deleteReturnOrder) | **DELETE** /api/v1/returns/{return_order_id} |  |
| [**getReturnOrder**](ReturnOrderApi.md#getReturnOrder) | **GET** /api/v1/returns/{return_order_id} |  |
| [**listReturnOrders**](ReturnOrderApi.md#listReturnOrders) | **GET** /api/v1/returns/ |  |
| [**returnLogisticsQueue**](ReturnOrderApi.md#returnLogisticsQueue) | **GET** /api/v1/returns/logistics-queue |  |
| [**returnLogisticsSummary**](ReturnOrderApi.md#returnLogisticsSummary) | **GET** /api/v1/returns/logistics-summary | Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse. |
| [**updateReturnOrder**](ReturnOrderApi.md#updateReturnOrder) | **PUT** /api/v1/returns/{return_order_id} |  |
| [**updateReturnOrderStatus**](ReturnOrderApi.md#updateReturnOrderStatus) | **PUT** /api/v1/returns/{return_order_id}/status |  |


<a id="createReturnOrder"></a>
# **createReturnOrder**
> ReturnOrder createReturnOrder(returnOrder)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
val returnOrder : ReturnOrder =  // ReturnOrder | 
try {
    val result : ReturnOrder = apiInstance.createReturnOrder(returnOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#createReturnOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#createReturnOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **returnOrder** | [**ReturnOrder**](ReturnOrder.md)|  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

<a id="deleteReturnOrder"></a>
# **deleteReturnOrder**
> deleteReturnOrder(returnOrderId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
val returnOrderId : kotlin.String = returnOrderId_example // kotlin.String | 
try {
    apiInstance.deleteReturnOrder(returnOrderId)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#deleteReturnOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#deleteReturnOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **returnOrderId** | **kotlin.String**|  | |

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

<a id="getReturnOrder"></a>
# **getReturnOrder**
> ReturnOrder getReturnOrder(returnOrderId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
val returnOrderId : kotlin.String = returnOrderId_example // kotlin.String | 
try {
    val result : ReturnOrder = apiInstance.getReturnOrder(returnOrderId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#getReturnOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#getReturnOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **returnOrderId** | **kotlin.String**|  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

<a id="listReturnOrders"></a>
# **listReturnOrders**
> kotlin.collections.List&lt;ReturnOrder&gt; listReturnOrders(page, pageSize, status, customerName, orderNumber)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val customerName : kotlin.String = customerName_example // kotlin.String | 
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ReturnOrder> = apiInstance.listReturnOrders(page, pageSize, status, customerName, orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#listReturnOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#listReturnOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **customerName** | **kotlin.String**|  | [optional] |
| **orderNumber** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ReturnOrder&gt;**](ReturnOrder.md)

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

<a id="returnLogisticsQueue"></a>
# **returnLogisticsQueue**
> kotlin.collections.List&lt;ReturnLogisticsQueueItem&gt; returnLogisticsQueue()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
try {
    val result : kotlin.collections.List<ReturnLogisticsQueueItem> = apiInstance.returnLogisticsQueue()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#returnLogisticsQueue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#returnLogisticsQueue")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ReturnLogisticsQueueItem&gt;**](ReturnLogisticsQueueItem.md)

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

<a id="returnLogisticsSummary"></a>
# **returnLogisticsSummary**
> ReturnLogisticsSummary returnLogisticsSummary()

Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
try {
    val result : ReturnLogisticsSummary = apiInstance.returnLogisticsSummary()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#returnLogisticsSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#returnLogisticsSummary")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ReturnLogisticsSummary**](ReturnLogisticsSummary.md)

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

<a id="updateReturnOrder"></a>
# **updateReturnOrder**
> ReturnOrder updateReturnOrder(returnOrderId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
val returnOrderId : kotlin.String = returnOrderId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : ReturnOrder = apiInstance.updateReturnOrder(returnOrderId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#updateReturnOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#updateReturnOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **returnOrderId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

<a id="updateReturnOrderStatus"></a>
# **updateReturnOrderStatus**
> ReturnOrder updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReturnOrderApi()
val returnOrderId : kotlin.String = returnOrderId_example // kotlin.String | 
val returnOrderStatusUpdate : ReturnOrderStatusUpdate =  // ReturnOrderStatusUpdate | 
try {
    val result : ReturnOrder = apiInstance.updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReturnOrderApi#updateReturnOrderStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReturnOrderApi#updateReturnOrderStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **returnOrderId** | **kotlin.String**|  | |
| **returnOrderStatusUpdate** | [**ReturnOrderStatusUpdate**](ReturnOrderStatusUpdate.md)|  | |

### Return type

[**ReturnOrder**](ReturnOrder.md)

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

