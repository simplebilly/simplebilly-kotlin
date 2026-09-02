# OrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**addOrderTags**](OrderApi.md#addOrderTags) | **POST** /api/v1/orders/{order_id}/tags |  |
| [**findOrderByExternalRef**](OrderApi.md#findOrderByExternalRef) | **GET** /api/v1/orders/by-ext-ref/{ext_ref} |  |
| [**getOrder**](OrderApi.md#getOrder) | **GET** /api/v1/order/{order_number} |  |
| [**getOrders**](OrderApi.md#getOrders) | **GET** /api/v1/orders |  |
| [**patchOrder**](OrderApi.md#patchOrder) | **PATCH** /api/v1/orders/{order_id} |  |
| [**replaceOrderTags**](OrderApi.md#replaceOrderTags) | **PUT** /api/v1/orders/{order_id}/tags |  |
| [**updateOrderState**](OrderApi.md#updateOrderState) | **PUT** /api/v1/orders/{order_id}/state |  |


<a id="addOrderTags"></a>
# **addOrderTags**
> Order addOrderTags(orderId, orderTagsRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val orderId : kotlin.String = orderId_example // kotlin.String | 
val orderTagsRequest : OrderTagsRequest =  // OrderTagsRequest | 
try {
    val result : Order = apiInstance.addOrderTags(orderId, orderTagsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#addOrderTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#addOrderTags")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderId** | **kotlin.String**|  | |
| **orderTagsRequest** | [**OrderTagsRequest**](OrderTagsRequest.md)|  | |

### Return type

[**Order**](Order.md)

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

<a id="findOrderByExternalRef"></a>
# **findOrderByExternalRef**
> Order findOrderByExternalRef(extRef)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val extRef : kotlin.String = extRef_example // kotlin.String | 
try {
    val result : Order = apiInstance.findOrderByExternalRef(extRef)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#findOrderByExternalRef")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#findOrderByExternalRef")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **extRef** | **kotlin.String**|  | |

### Return type

[**Order**](Order.md)

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

<a id="getOrder"></a>
# **getOrder**
> Order getOrder(orderNumber)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : Order = apiInstance.getOrder(orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#getOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#getOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |

### Return type

[**Order**](Order.md)

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

<a id="getOrders"></a>
# **getOrders**
> kotlin.collections.List&lt;Order&gt; getOrders(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Order> = apiInstance.getOrders(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#getOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#getOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;Order&gt;**](Order.md)

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

<a id="patchOrder"></a>
# **patchOrder**
> Order patchOrder(orderId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val orderId : kotlin.String = orderId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Order = apiInstance.patchOrder(orderId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#patchOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#patchOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Order**](Order.md)

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

<a id="replaceOrderTags"></a>
# **replaceOrderTags**
> Order replaceOrderTags(orderId, orderTagsRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val orderId : kotlin.String = orderId_example // kotlin.String | 
val orderTagsRequest : OrderTagsRequest =  // OrderTagsRequest | 
try {
    val result : Order = apiInstance.replaceOrderTags(orderId, orderTagsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#replaceOrderTags")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#replaceOrderTags")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderId** | **kotlin.String**|  | |
| **orderTagsRequest** | [**OrderTagsRequest**](OrderTagsRequest.md)|  | |

### Return type

[**Order**](Order.md)

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

<a id="updateOrderState"></a>
# **updateOrderState**
> Order updateOrderState(orderId, orderStateUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderApi()
val orderId : kotlin.String = orderId_example // kotlin.String | 
val orderStateUpdate : OrderStateUpdate =  // OrderStateUpdate | 
try {
    val result : Order = apiInstance.updateOrderState(orderId, orderStateUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderApi#updateOrderState")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderApi#updateOrderState")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderId** | **kotlin.String**|  | |
| **orderStateUpdate** | [**OrderStateUpdate**](OrderStateUpdate.md)|  | |

### Return type

[**Order**](Order.md)

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

