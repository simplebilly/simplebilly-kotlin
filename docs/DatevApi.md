# DatevApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**datevExportApi**](DatevApi.md#datevExportApi) | **GET** /api/v1/bookkeeping/datev/export | Export bookkeeping data as DATEV CSV |
| [**datevPreviewApi**](DatevApi.md#datevPreviewApi) | **GET** /api/v1/bookkeeping/datev/preview | Exported_datev_bookings: returns formed bookings for review |


<a id="datevExportApi"></a>
# **datevExportApi**
> DatevExportResponse datevExportApi(accountSchema, dateFrom, dateTo, page, pageSize)

Export bookkeeping data as DATEV CSV

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DatevApi()
val accountSchema : kotlin.String = accountSchema_example // kotlin.String | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : DatevExportResponse = apiInstance.datevExportApi(accountSchema, dateFrom, dateTo, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatevApi#datevExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatevApi#datevExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **accountSchema** | **kotlin.String**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**DatevExportResponse**](DatevExportResponse.md)

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

<a id="datevPreviewApi"></a>
# **datevPreviewApi**
> kotlin.collections.List&lt;DatevBookingPreview&gt; datevPreviewApi(accountSchema, dateFrom, dateTo, page, pageSize)

Exported_datev_bookings: returns formed bookings for review

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DatevApi()
val accountSchema : kotlin.String = accountSchema_example // kotlin.String | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<DatevBookingPreview> = apiInstance.datevPreviewApi(accountSchema, dateFrom, dateTo, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DatevApi#datevPreviewApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DatevApi#datevPreviewApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **accountSchema** | **kotlin.String**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;DatevBookingPreview&gt;**](DatevBookingPreview.md)

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

