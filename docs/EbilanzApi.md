# EbilanzApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**ebilanzReportApi**](EbilanzApi.md#ebilanzReportApi) | **GET** /api/v1/bookkeeping/ebilanz |  |
| [**ebilanzXbrlExportApi**](EbilanzApi.md#ebilanzXbrlExportApi) | **GET** /api/v1/bookkeeping/ebilanz/xbrl |  |


<a id="ebilanzReportApi"></a>
# **ebilanzReportApi**
> EBilanzReport ebilanzReportApi(year, dateFrom, dateTo)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EbilanzApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
try {
    val result : EBilanzReport = apiInstance.ebilanzReportApi(year, dateFrom, dateTo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EbilanzApi#ebilanzReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EbilanzApi#ebilanzReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |

### Return type

[**EBilanzReport**](EBilanzReport.md)

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

<a id="ebilanzXbrlExportApi"></a>
# **ebilanzXbrlExportApi**
> ebilanzXbrlExportApi(year, dateFrom, dateTo)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EbilanzApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
try {
    apiInstance.ebilanzXbrlExportApi(year, dateFrom, dateTo)
} catch (e: ClientException) {
    println("4xx response calling EbilanzApi#ebilanzXbrlExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EbilanzApi#ebilanzXbrlExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

