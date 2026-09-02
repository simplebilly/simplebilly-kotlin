# StilleApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**stilleExportApi**](StilleApi.md#stilleExportApi) | **GET** /api/v1/bookkeeping/stille/export |  |
| [**stilleReportApi**](StilleApi.md#stilleReportApi) | **GET** /api/v1/bookkeeping/stille/report |  |


<a id="stilleExportApi"></a>
# **stilleExportApi**
> StilleExportResponse stilleExportApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StilleApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : StilleExportResponse = apiInstance.stilleExportApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StilleApi#stilleExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StilleApi#stilleExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**StilleExportResponse**](StilleExportResponse.md)

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

<a id="stilleReportApi"></a>
# **stilleReportApi**
> StilleReport stilleReportApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = StilleApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : StilleReport = apiInstance.stilleReportApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling StilleApi#stilleReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling StilleApi#stilleReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**StilleReport**](StilleReport.md)

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

