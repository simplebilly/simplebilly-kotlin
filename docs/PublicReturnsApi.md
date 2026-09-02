# PublicReturnsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getPublicReturnStatus**](PublicReturnsApi.md#getPublicReturnStatus) | **GET** /api/v1/public/returns/status | Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches. |
| [**listPublicReturns**](PublicReturnsApi.md#listPublicReturns) | **GET** /api/v1/public/returns/list | List all returns for an order (public, no auth). |
| [**requestPublicReturn**](PublicReturnsApi.md#requestPublicReturn) | **POST** /api/v1/public/returns/request | Customer requests a return for an order (public, no auth). |


<a id="getPublicReturnStatus"></a>
# **getPublicReturnStatus**
> PublicReturnStatusResponse getPublicReturnStatus(email, returnNumber, returnOrderId, orderNumber)

Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PublicReturnsApi()
val email : kotlin.String = email_example // kotlin.String | 
val returnNumber : kotlin.String = returnNumber_example // kotlin.String | Either return_number or return_order_id must be provided.
val returnOrderId : kotlin.String = returnOrderId_example // kotlin.String | 
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : PublicReturnStatusResponse = apiInstance.getPublicReturnStatus(email, returnNumber, returnOrderId, orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PublicReturnsApi#getPublicReturnStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PublicReturnsApi#getPublicReturnStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **email** | **kotlin.String**|  | |
| **returnNumber** | **kotlin.String**| Either return_number or return_order_id must be provided. | [optional] |
| **returnOrderId** | **kotlin.String**|  | [optional] |
| **orderNumber** | **kotlin.String**|  | [optional] |

### Return type

[**PublicReturnStatusResponse**](PublicReturnStatusResponse.md)

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

<a id="listPublicReturns"></a>
# **listPublicReturns**
> kotlin.collections.List&lt;PublicReturnStatusResponse&gt; listPublicReturns(orderNumber, email)

List all returns for an order (public, no auth).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PublicReturnsApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val email : kotlin.String = email_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PublicReturnStatusResponse> = apiInstance.listPublicReturns(orderNumber, email)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PublicReturnsApi#listPublicReturns")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PublicReturnsApi#listPublicReturns")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |
| **email** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;PublicReturnStatusResponse&gt;**](PublicReturnStatusResponse.md)

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

<a id="requestPublicReturn"></a>
# **requestPublicReturn**
> PublicReturnResponse requestPublicReturn(publicReturnRequest)

Customer requests a return for an order (public, no auth).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PublicReturnsApi()
val publicReturnRequest : PublicReturnRequest =  // PublicReturnRequest | 
try {
    val result : PublicReturnResponse = apiInstance.requestPublicReturn(publicReturnRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PublicReturnsApi#requestPublicReturn")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PublicReturnsApi#requestPublicReturn")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **publicReturnRequest** | [**PublicReturnRequest**](PublicReturnRequest.md)|  | |

### Return type

[**PublicReturnResponse**](PublicReturnResponse.md)

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

