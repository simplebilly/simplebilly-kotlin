# PeppolApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**peppolApi**](PeppolApi.md#peppolApi) | **GET** /api/v1/invoices/{id}/peppol |  |


<a id="peppolApi"></a>
# **peppolApi**
> PeppolResponse peppolApi(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PeppolApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : PeppolResponse = apiInstance.peppolApi(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PeppolApi#peppolApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PeppolApi#peppolApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**PeppolResponse**](PeppolResponse.md)

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

