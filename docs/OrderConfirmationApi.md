# OrderConfirmationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createConfirmation**](OrderConfirmationApi.md#createConfirmation) | **POST** /api/v1/order-confirmations |  |
| [**deleteConfirmation**](OrderConfirmationApi.md#deleteConfirmation) | **DELETE** /api/v1/order-confirmations/{confirmation_id} |  |
| [**downloadConfirmationPdf**](OrderConfirmationApi.md#downloadConfirmationPdf) | **GET** /api/v1/order-confirmations/{confirmation_id}/pdf |  |
| [**getConfirmation**](OrderConfirmationApi.md#getConfirmation) | **GET** /api/v1/order-confirmations/{confirmation_id} |  |
| [**listConfirmations**](OrderConfirmationApi.md#listConfirmations) | **GET** /api/v1/order-confirmations/ |  |
| [**orderconfirmationRestore**](OrderConfirmationApi.md#orderconfirmationRestore) | **POST** /api/v1/order-confirmations/{confirmation_id}/restore |  |
| [**pursueConfirmation**](OrderConfirmationApi.md#pursueConfirmation) | **POST** /api/v1/order-confirmations/{confirmation_id}/pursue |  |


<a id="createConfirmation"></a>
# **createConfirmation**
> OrderConfirmation createConfirmation(orderConfirmationCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val orderConfirmationCreate : OrderConfirmationCreate =  // OrderConfirmationCreate | 
try {
    val result : OrderConfirmation = apiInstance.createConfirmation(orderConfirmationCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#createConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#createConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderConfirmationCreate** | [**OrderConfirmationCreate**](OrderConfirmationCreate.md)|  | |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

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

<a id="deleteConfirmation"></a>
# **deleteConfirmation**
> deleteConfirmation(confirmationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val confirmationId : kotlin.String = confirmationId_example // kotlin.String | 
try {
    apiInstance.deleteConfirmation(confirmationId)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#deleteConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#deleteConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmationId** | **kotlin.String**|  | |

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

<a id="downloadConfirmationPdf"></a>
# **downloadConfirmationPdf**
> downloadConfirmationPdf(confirmationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val confirmationId : kotlin.String = confirmationId_example // kotlin.String | 
try {
    apiInstance.downloadConfirmationPdf(confirmationId)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#downloadConfirmationPdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#downloadConfirmationPdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmationId** | **kotlin.String**|  | |

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

<a id="getConfirmation"></a>
# **getConfirmation**
> OrderConfirmation getConfirmation(confirmationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val confirmationId : kotlin.String = confirmationId_example // kotlin.String | 
try {
    val result : OrderConfirmation = apiInstance.getConfirmation(confirmationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#getConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#getConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmationId** | **kotlin.String**|  | |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

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

<a id="listConfirmations"></a>
# **listConfirmations**
> kotlin.collections.List&lt;OrderConfirmation&gt; listConfirmations(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<OrderConfirmation> = apiInstance.listConfirmations(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#listConfirmations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#listConfirmations")
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

[**kotlin.collections.List&lt;OrderConfirmation&gt;**](OrderConfirmation.md)

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

<a id="orderconfirmationRestore"></a>
# **orderconfirmationRestore**
> OrderConfirmation orderconfirmationRestore(confirmationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val confirmationId : kotlin.String = confirmationId_example // kotlin.String | 
try {
    val result : OrderConfirmation = apiInstance.orderconfirmationRestore(confirmationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#orderconfirmationRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#orderconfirmationRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmationId** | **kotlin.String**|  | |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

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

<a id="pursueConfirmation"></a>
# **pursueConfirmation**
> DeliveryNote pursueConfirmation(confirmationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OrderConfirmationApi()
val confirmationId : kotlin.String = confirmationId_example // kotlin.String | 
try {
    val result : DeliveryNote = apiInstance.pursueConfirmation(confirmationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OrderConfirmationApi#pursueConfirmation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OrderConfirmationApi#pursueConfirmation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **confirmationId** | **kotlin.String**|  | |

### Return type

[**DeliveryNote**](DeliveryNote.md)

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

