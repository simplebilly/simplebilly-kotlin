# SuitabilityApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**shippingSuitabilityApi**](SuitabilityApi.md#shippingSuitabilityApi) | **POST** /api/v1/shipping/suitability |  |


<a id="shippingSuitabilityApi"></a>
# **shippingSuitabilityApi**
> SuitabilityResult shippingSuitabilityApi(suitabilityRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SuitabilityApi()
val suitabilityRequest : SuitabilityRequest =  // SuitabilityRequest | 
try {
    val result : SuitabilityResult = apiInstance.shippingSuitabilityApi(suitabilityRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SuitabilityApi#shippingSuitabilityApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SuitabilityApi#shippingSuitabilityApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **suitabilityRequest** | [**SuitabilityRequest**](SuitabilityRequest.md)|  | |

### Return type

[**SuitabilityResult**](SuitabilityResult.md)

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

