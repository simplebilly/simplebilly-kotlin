# PaygapApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**paygapAuskunftApi**](PaygapApi.md#paygapAuskunftApi) | **GET** /api/v1/bookkeeping/paygap/auskunft/{employee_id} |  |
| [**paygapExportApi**](PaygapApi.md#paygapExportApi) | **GET** /api/v1/bookkeeping/paygap/export |  |
| [**paygapReportApi**](PaygapApi.md#paygapReportApi) | **GET** /api/v1/bookkeeping/paygap/report |  |


<a id="paygapAuskunftApi"></a>
# **paygapAuskunftApi**
> PayGapInfoResponse paygapAuskunftApi(employeeId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaygapApi()
val employeeId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : PayGapInfoResponse = apiInstance.paygapAuskunftApi(employeeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaygapApi#paygapAuskunftApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaygapApi#paygapAuskunftApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **employeeId** | **java.util.UUID**|  | |

### Return type

[**PayGapInfoResponse**](PayGapInfoResponse.md)

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

<a id="paygapExportApi"></a>
# **paygapExportApi**
> PayGapExportResponse paygapExportApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaygapApi()
try {
    val result : PayGapExportResponse = apiInstance.paygapExportApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaygapApi#paygapExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaygapApi#paygapExportApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PayGapExportResponse**](PayGapExportResponse.md)

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

<a id="paygapReportApi"></a>
# **paygapReportApi**
> PayGapReport paygapReportApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaygapApi()
try {
    val result : PayGapReport = apiInstance.paygapReportApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaygapApi#paygapReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaygapApi#paygapReportApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**PayGapReport**](PayGapReport.md)

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

