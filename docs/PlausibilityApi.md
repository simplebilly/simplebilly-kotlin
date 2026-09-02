# PlausibilityApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**plausibilityCheckApi**](PlausibilityApi.md#plausibilityCheckApi) | **GET** /api/v1/bookkeeping/plausibility |  |


<a id="plausibilityCheckApi"></a>
# **plausibilityCheckApi**
> PlausibilityReport plausibilityCheckApi(dateFrom, dateTo)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PlausibilityApi()
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
try {
    val result : PlausibilityReport = apiInstance.plausibilityCheckApi(dateFrom, dateTo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PlausibilityApi#plausibilityCheckApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PlausibilityApi#plausibilityCheckApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |

### Return type

[**PlausibilityReport**](PlausibilityReport.md)

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

