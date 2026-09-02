# GobdExportApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**buchhalterCsvApi**](GobdExportApi.md#buchhalterCsvApi) | **GET** /api/v1/bookkeeping/buchhalter-csv |  |
| [**gobdExportApi**](GobdExportApi.md#gobdExportApi) | **GET** /api/v1/bookkeeping/gobd | GoBD/GDPdU export. Default: ZIP archive (&#x60;index.xml&#x60; + CSV tables, IDEA format). &#x60;?format&#x3D;csv&#x60; returns the legacy single-journal CSV as JSON. |


<a id="buchhalterCsvApi"></a>
# **buchhalterCsvApi**
> GoBDExportResponse buchhalterCsvApi(dateFrom, dateTo)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GobdExportApi()
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
try {
    val result : GoBDExportResponse = apiInstance.buchhalterCsvApi(dateFrom, dateTo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GobdExportApi#buchhalterCsvApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GobdExportApi#buchhalterCsvApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dateFrom** | **kotlin.String**|  | |
| **dateTo** | **kotlin.String**|  | |

### Return type

[**GoBDExportResponse**](GoBDExportResponse.md)

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

<a id="gobdExportApi"></a>
# **gobdExportApi**
> gobdExportApi(year, format)

GoBD/GDPdU export. Default: ZIP archive (&#x60;index.xml&#x60; + CSV tables, IDEA format). &#x60;?format&#x3D;csv&#x60; returns the legacy single-journal CSV as JSON.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GobdExportApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val format : kotlin.String = zip // kotlin.String | Export format: `zip` (default, full GDPdU/IDEA export) or `csv` (legacy single-journal CSV as JSON).
try {
    apiInstance.gobdExportApi(year, format)
} catch (e: ClientException) {
    println("4xx response calling GobdExportApi#gobdExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GobdExportApi#gobdExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |
| **format** | **kotlin.String**| Export format: &#x60;zip&#x60; (default, full GDPdU/IDEA export) or &#x60;csv&#x60; (legacy single-journal CSV as JSON). | [optional] |

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
 - **Accept**: application/json

