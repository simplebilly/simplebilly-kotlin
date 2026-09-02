# GewinnverwendungApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gewinnverwendungApi**](GewinnverwendungApi.md#gewinnverwendungApi) | **GET** /api/v1/bookkeeping/gewinnverwendung |  |
| [**gewinnverwendungExportApi**](GewinnverwendungApi.md#gewinnverwendungExportApi) | **GET** /api/v1/bookkeeping/gewinnverwendung/export |  |


<a id="gewinnverwendungApi"></a>
# **gewinnverwendungApi**
> GewinnverwendungsReport gewinnverwendungApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GewinnverwendungApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : GewinnverwendungsReport = apiInstance.gewinnverwendungApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GewinnverwendungApi#gewinnverwendungApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GewinnverwendungApi#gewinnverwendungApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**GewinnverwendungsReport**](GewinnverwendungsReport.md)

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

<a id="gewinnverwendungExportApi"></a>
# **gewinnverwendungExportApi**
> GewinnverwendungsExportResponse gewinnverwendungExportApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GewinnverwendungApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : GewinnverwendungsExportResponse = apiInstance.gewinnverwendungExportApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GewinnverwendungApi#gewinnverwendungExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GewinnverwendungApi#gewinnverwendungExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**GewinnverwendungsExportResponse**](GewinnverwendungsExportResponse.md)

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

