# DatevImportApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**datevImportApi**](DatevImportApi.md#datevImportApi) | **POST** /api/v1/bookkeeping/datev/import |  |


<a id="datevImportApi"></a>
# **datevImportApi**
> DatevImportResponse datevImportApi(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DatevImportApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : DatevImportResponse = apiInstance.datevImportApi(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatevImportApi#datevImportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatevImportApi#datevImportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**DatevImportResponse**](DatevImportResponse.md)

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

