# QuotationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createQuotation**](QuotationApi.md#createQuotation) | **POST** /api/v1/quotations |  |
| [**deleteQuotation**](QuotationApi.md#deleteQuotation) | **DELETE** /api/v1/quotations/{quotation_id} |  |
| [**downloadQuotationPdf**](QuotationApi.md#downloadQuotationPdf) | **GET** /api/v1/quotations/{quotation_id}/pdf |  |
| [**getQuotation**](QuotationApi.md#getQuotation) | **GET** /api/v1/quotations/{quotation_id} |  |
| [**listQuotations**](QuotationApi.md#listQuotations) | **GET** /api/v1/quotations/ |  |
| [**pursueQuotation**](QuotationApi.md#pursueQuotation) | **POST** /api/v1/quotations/{quotation_id}/pursue |  |
| [**quotationRestore**](QuotationApi.md#quotationRestore) | **POST** /api/v1/quotations/{quotation_id}/restore |  |
| [**updateQuotation**](QuotationApi.md#updateQuotation) | **PUT** /api/v1/quotations/{quotation_id} |  |


<a id="createQuotation"></a>
# **createQuotation**
> Quotation createQuotation(quotationCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationCreate : QuotationCreate =  // QuotationCreate | 
try {
    val result : Quotation = apiInstance.createQuotation(quotationCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#createQuotation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#createQuotation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationCreate** | [**QuotationCreate**](QuotationCreate.md)|  | |

### Return type

[**Quotation**](Quotation.md)

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

<a id="deleteQuotation"></a>
# **deleteQuotation**
> deleteQuotation(quotationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationId : kotlin.String = quotationId_example // kotlin.String | 
try {
    apiInstance.deleteQuotation(quotationId)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#deleteQuotation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#deleteQuotation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationId** | **kotlin.String**|  | |

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

<a id="downloadQuotationPdf"></a>
# **downloadQuotationPdf**
> downloadQuotationPdf(quotationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationId : kotlin.String = quotationId_example // kotlin.String | 
try {
    apiInstance.downloadQuotationPdf(quotationId)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#downloadQuotationPdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#downloadQuotationPdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationId** | **kotlin.String**|  | |

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

<a id="getQuotation"></a>
# **getQuotation**
> Quotation getQuotation(quotationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationId : kotlin.String = quotationId_example // kotlin.String | 
try {
    val result : Quotation = apiInstance.getQuotation(quotationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#getQuotation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#getQuotation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationId** | **kotlin.String**|  | |

### Return type

[**Quotation**](Quotation.md)

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

<a id="listQuotations"></a>
# **listQuotations**
> kotlin.collections.List&lt;Quotation&gt; listQuotations(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Quotation> = apiInstance.listQuotations(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#listQuotations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#listQuotations")
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

[**kotlin.collections.List&lt;Quotation&gt;**](Quotation.md)

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

<a id="pursueQuotation"></a>
# **pursueQuotation**
> OrderConfirmation pursueQuotation(quotationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationId : kotlin.String = quotationId_example // kotlin.String | 
try {
    val result : OrderConfirmation = apiInstance.pursueQuotation(quotationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#pursueQuotation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#pursueQuotation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationId** | **kotlin.String**|  | |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

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

<a id="quotationRestore"></a>
# **quotationRestore**
> Quotation quotationRestore(quotationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationId : kotlin.String = quotationId_example // kotlin.String | 
try {
    val result : Quotation = apiInstance.quotationRestore(quotationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#quotationRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#quotationRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationId** | **kotlin.String**|  | |

### Return type

[**Quotation**](Quotation.md)

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

<a id="updateQuotation"></a>
# **updateQuotation**
> Quotation updateQuotation(quotationId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = QuotationApi()
val quotationId : kotlin.String = quotationId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Quotation = apiInstance.updateQuotation(quotationId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling QuotationApi#updateQuotation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling QuotationApi#updateQuotation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotationId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Quotation**](Quotation.md)

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

