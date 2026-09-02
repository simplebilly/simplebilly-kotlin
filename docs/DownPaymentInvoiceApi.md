# DownPaymentInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**downloadDownPaymentInvoicePdf**](DownPaymentInvoiceApi.md#downloadDownPaymentInvoicePdf) | **GET** /api/v1/down-payment-invoices/{id}/pdf |  |
| [**getDownPaymentInvoice**](DownPaymentInvoiceApi.md#getDownPaymentInvoice) | **GET** /api/v1/down-payment-invoices/{id} |  |
| [**listDownPaymentInvoices**](DownPaymentInvoiceApi.md#listDownPaymentInvoices) | **GET** /api/v1/down-payment-invoices/ |  |


<a id="downloadDownPaymentInvoicePdf"></a>
# **downloadDownPaymentInvoicePdf**
> downloadDownPaymentInvoicePdf(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DownPaymentInvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.downloadDownPaymentInvoicePdf(id)
} catch (e: ClientException) {
    println("4xx response calling DownPaymentInvoiceApi#downloadDownPaymentInvoicePdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DownPaymentInvoiceApi#downloadDownPaymentInvoicePdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="getDownPaymentInvoice"></a>
# **getDownPaymentInvoice**
> DownPaymentInvoice getDownPaymentInvoice(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DownPaymentInvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : DownPaymentInvoice = apiInstance.getDownPaymentInvoice(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DownPaymentInvoiceApi#getDownPaymentInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DownPaymentInvoiceApi#getDownPaymentInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**DownPaymentInvoice**](DownPaymentInvoice.md)

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

<a id="listDownPaymentInvoices"></a>
# **listDownPaymentInvoices**
> kotlin.collections.List&lt;DownPaymentInvoice&gt; listDownPaymentInvoices(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DownPaymentInvoiceApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<DownPaymentInvoice> = apiInstance.listDownPaymentInvoices(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DownPaymentInvoiceApi#listDownPaymentInvoices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DownPaymentInvoiceApi#listDownPaymentInvoices")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;DownPaymentInvoice&gt;**](DownPaymentInvoice.md)

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

