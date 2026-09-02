# ProductionOrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProductionOrder**](ProductionOrderApi.md#createProductionOrder) | **POST** /api/v1/production-orders |  |
| [**deleteProductionOrder**](ProductionOrderApi.md#deleteProductionOrder) | **DELETE** /api/v1/production-orders/{production_order_id} |  |
| [**getProductionOrder**](ProductionOrderApi.md#getProductionOrder) | **GET** /api/v1/production-orders/{production_order_id} |  |
| [**listProductionOrders**](ProductionOrderApi.md#listProductionOrders) | **GET** /api/v1/production-orders/ |  |
| [**productionOrderCosting**](ProductionOrderApi.md#productionOrderCosting) | **GET** /api/v1/production-orders/{production_order_id}/costing | Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price. |
| [**updateProductionOrder**](ProductionOrderApi.md#updateProductionOrder) | **PUT** /api/v1/production-orders/{production_order_id} |  |
| [**updateProductionOrderStatus**](ProductionOrderApi.md#updateProductionOrderStatus) | **PUT** /api/v1/production-orders/{production_order_id}/status |  |


<a id="createProductionOrder"></a>
# **createProductionOrder**
> ProductionOrder createProductionOrder(productionOrder)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val productionOrder : ProductionOrder =  // ProductionOrder | 
try {
    val result : ProductionOrder = apiInstance.createProductionOrder(productionOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#createProductionOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#createProductionOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productionOrder** | [**ProductionOrder**](ProductionOrder.md)|  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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

<a id="deleteProductionOrder"></a>
# **deleteProductionOrder**
> deleteProductionOrder(productionOrderId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val productionOrderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteProductionOrder(productionOrderId)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#deleteProductionOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#deleteProductionOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productionOrderId** | **java.util.UUID**|  | |

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

<a id="getProductionOrder"></a>
# **getProductionOrder**
> ProductionOrder getProductionOrder(productionOrderId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val productionOrderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : ProductionOrder = apiInstance.getProductionOrder(productionOrderId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#getProductionOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#getProductionOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productionOrderId** | **java.util.UUID**|  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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

<a id="listProductionOrders"></a>
# **listProductionOrders**
> kotlin.collections.List&lt;ProductionOrder&gt; listProductionOrders(page, pageSize, search, status)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | Filter by status.
try {
    val result : kotlin.collections.List<ProductionOrder> = apiInstance.listProductionOrders(page, pageSize, search, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#listProductionOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#listProductionOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **status** | **kotlin.String**| Filter by status. | [optional] |

### Return type

[**kotlin.collections.List&lt;ProductionOrder&gt;**](ProductionOrder.md)

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

<a id="productionOrderCosting"></a>
# **productionOrderCosting**
> ProductionOrderCosting productionOrderCosting(productionOrderId)

Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val productionOrderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : ProductionOrderCosting = apiInstance.productionOrderCosting(productionOrderId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#productionOrderCosting")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#productionOrderCosting")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productionOrderId** | **java.util.UUID**|  | |

### Return type

[**ProductionOrderCosting**](ProductionOrderCosting.md)

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

<a id="updateProductionOrder"></a>
# **updateProductionOrder**
> ProductionOrder updateProductionOrder(productionOrderId, productionOrder)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val productionOrderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val productionOrder : ProductionOrder =  // ProductionOrder | 
try {
    val result : ProductionOrder = apiInstance.updateProductionOrder(productionOrderId, productionOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#updateProductionOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#updateProductionOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productionOrderId** | **java.util.UUID**|  | |
| **productionOrder** | [**ProductionOrder**](ProductionOrder.md)|  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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

<a id="updateProductionOrderStatus"></a>
# **updateProductionOrderStatus**
> ProductionOrder updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductionOrderApi()
val productionOrderId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val productionOrderStatusUpdate : ProductionOrderStatusUpdate =  // ProductionOrderStatusUpdate | 
try {
    val result : ProductionOrder = apiInstance.updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductionOrderApi#updateProductionOrderStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductionOrderApi#updateProductionOrderStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productionOrderId** | **java.util.UUID**|  | |
| **productionOrderStatusUpdate** | [**ProductionOrderStatusUpdate**](ProductionOrderStatusUpdate.md)|  | |

### Return type

[**ProductionOrder**](ProductionOrder.md)

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

