# ReportsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**bilanzReportApi**](ReportsApi.md#bilanzReportApi) | **GET** /api/v1/bookkeeping/reports/bilanz | Bilanz (Balance Sheet) |
| [**guvReportApi**](ReportsApi.md#guvReportApi) | **GET** /api/v1/bookkeeping/reports/guv | Gewinn- und Verlustrechnung (P&amp;L statement) |
| [**kontenansichtReportApi**](ReportsApi.md#kontenansichtReportApi) | **GET** /api/v1/bookkeeping/reports/kontenansicht | Kontenansicht (Account Overview) |
| [**umsatzsteuerReportApi**](ReportsApi.md#umsatzsteuerReportApi) | **GET** /api/v1/bookkeeping/reports/umsatzsteuer | Umsatzsteuer-Voranmeldung (VAT report) |


<a id="bilanzReportApi"></a>
# **bilanzReportApi**
> BilanzReport bilanzReportApi(year, month, dateFrom, dateTo, page, pageSize)

Bilanz (Balance Sheet)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReportsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BilanzReport = apiInstance.bilanzReportApi(year, month, dateFrom, dateTo, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#bilanzReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#bilanzReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **month** | **kotlin.Int**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**BilanzReport**](BilanzReport.md)

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

<a id="guvReportApi"></a>
# **guvReportApi**
> GuVReport guvReportApi(year, month, dateFrom, dateTo, page, pageSize)

Gewinn- und Verlustrechnung (P&amp;L statement)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReportsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : GuVReport = apiInstance.guvReportApi(year, month, dateFrom, dateTo, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#guvReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#guvReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **month** | **kotlin.Int**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**GuVReport**](GuVReport.md)

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

<a id="kontenansichtReportApi"></a>
# **kontenansichtReportApi**
> KontoReport kontenansichtReportApi(year, month, dateFrom, dateTo, page, pageSize)

Kontenansicht (Account Overview)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReportsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KontoReport = apiInstance.kontenansichtReportApi(year, month, dateFrom, dateTo, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#kontenansichtReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#kontenansichtReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **month** | **kotlin.Int**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**KontoReport**](KontoReport.md)

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

<a id="umsatzsteuerReportApi"></a>
# **umsatzsteuerReportApi**
> UmsatzsteuerReport umsatzsteuerReportApi(year, month, dateFrom, dateTo, page, pageSize)

Umsatzsteuer-Voranmeldung (VAT report)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ReportsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
val dateFrom : kotlin.String = dateFrom_example // kotlin.String | 
val dateTo : kotlin.String = dateTo_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : UmsatzsteuerReport = apiInstance.umsatzsteuerReportApi(year, month, dateFrom, dateTo, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ReportsApi#umsatzsteuerReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ReportsApi#umsatzsteuerReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **month** | **kotlin.Int**|  | [optional] |
| **dateFrom** | **kotlin.String**|  | [optional] |
| **dateTo** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**UmsatzsteuerReport**](UmsatzsteuerReport.md)

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

