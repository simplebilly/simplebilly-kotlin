# KonzernApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**konzernExportApi**](KonzernApi.md#konzernExportApi) | **GET** /api/v1/bookkeeping/konzern/status/export |  |
| [**konzernStatusApi**](KonzernApi.md#konzernStatusApi) | **GET** /api/v1/bookkeeping/konzern/status |  |


<a id="konzernExportApi"></a>
# **konzernExportApi**
> KonzernExportResponse konzernExportApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KonzernApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KonzernExportResponse = apiInstance.konzernExportApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KonzernApi#konzernExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KonzernApi#konzernExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**KonzernExportResponse**](KonzernExportResponse.md)

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

<a id="konzernStatusApi"></a>
# **konzernStatusApi**
> KonzernStatus konzernStatusApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KonzernApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KonzernStatus = apiInstance.konzernStatusApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KonzernApi#konzernStatusApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KonzernApi#konzernStatusApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**KonzernStatus**](KonzernStatus.md)

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

