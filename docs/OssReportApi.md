# OssReportApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**ossReportApi**](OssReportApi.md#ossReportApi) | **GET** /api/v1/bookkeeping/oss |  |


<a id="ossReportApi"></a>
# **ossReportApi**
> OssReport ossReportApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OssReportApi()
try {
    val result : OssReport = apiInstance.ossReportApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OssReportApi#ossReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OssReportApi#ossReportApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**OssReport**](OssReport.md)

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

