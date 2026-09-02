# InvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createInvoice**](InvoiceApi.md#createInvoice) | **POST** /api/v1/invoices |  |
| [**deleteInvoice**](InvoiceApi.md#deleteInvoice) | **DELETE** /api/v1/invoices/{id} |  |
| [**downloadInvoicePdf**](InvoiceApi.md#downloadInvoicePdf) | **GET** /api/v1/invoices/{id}/pdf |  |
| [**getInvoice**](InvoiceApi.md#getInvoice) | **GET** /api/v1/invoices/{id} |  |
| [**getInvoicePdfUrl**](InvoiceApi.md#getInvoicePdfUrl) | **GET** /api/v1/invoices/{id}/pdf-url |  |
| [**getInvoices**](InvoiceApi.md#getInvoices) | **GET** /api/v1/invoices/ |  |
| [**invoiceRestore**](InvoiceApi.md#invoiceRestore) | **POST** /api/v1/invoices/{id}/restore |  |
| [**updateInvoice**](InvoiceApi.md#updateInvoice) | **PUT** /api/v1/invoices/{id} |  |


<a id="createInvoice"></a>
# **createInvoice**
> Invoice createInvoice(invoiceCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val invoiceCreate : InvoiceCreate =  // InvoiceCreate | 
try {
    val result : Invoice = apiInstance.createInvoice(invoiceCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#createInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#createInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **invoiceCreate** | [**InvoiceCreate**](InvoiceCreate.md)|  | |

### Return type

[**Invoice**](Invoice.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteInvoice"></a>
# **deleteInvoice**
> deleteInvoice(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.deleteInvoice(id)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#deleteInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#deleteInvoice")
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

<a id="downloadInvoicePdf"></a>
# **downloadInvoicePdf**
> downloadInvoicePdf(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.downloadInvoicePdf(id)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#downloadInvoicePdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#downloadInvoicePdf")
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

<a id="getInvoice"></a>
# **getInvoice**
> Invoice getInvoice(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : Invoice = apiInstance.getInvoice(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#getInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#getInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**Invoice**](Invoice.md)

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

<a id="getInvoicePdfUrl"></a>
# **getInvoicePdfUrl**
> InvoicePdfUrlResponse getInvoicePdfUrl(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : InvoicePdfUrlResponse = apiInstance.getInvoicePdfUrl(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#getInvoicePdfUrl")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#getInvoicePdfUrl")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**InvoicePdfUrlResponse**](InvoicePdfUrlResponse.md)

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

<a id="getInvoices"></a>
# **getInvoices**
> kotlin.collections.List&lt;Invoice&gt; getInvoices(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Invoice> = apiInstance.getInvoices(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#getInvoices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#getInvoices")
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

[**kotlin.collections.List&lt;Invoice&gt;**](Invoice.md)

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

<a id="invoiceRestore"></a>
# **invoiceRestore**
> Invoice invoiceRestore(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : Invoice = apiInstance.invoiceRestore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#invoiceRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#invoiceRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

### Return type

[**Invoice**](Invoice.md)

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

<a id="updateInvoice"></a>
# **updateInvoice**
> Invoice updateInvoice(id, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InvoiceApi()
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Invoice = apiInstance.updateInvoice(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InvoiceApi#updateInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InvoiceApi#updateInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Invoice**](Invoice.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

