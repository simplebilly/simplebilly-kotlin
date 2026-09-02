# CreditNoteApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCreditNote**](CreditNoteApi.md#createCreditNote) | **POST** /api/v1/credit-notes |  |
| [**downloadCreditNotePdf**](CreditNoteApi.md#downloadCreditNotePdf) | **GET** /api/v1/credit-notes/{credit_note_id}/pdf |  |
| [**getCreditNote**](CreditNoteApi.md#getCreditNote) | **GET** /api/v1/credit-notes/{credit_note_id} |  |
| [**listCreditNotes**](CreditNoteApi.md#listCreditNotes) | **GET** /api/v1/credit-notes/ |  |


<a id="createCreditNote"></a>
# **createCreditNote**
> Invoice createCreditNote(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CreditNoteApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Invoice = apiInstance.createCreditNote(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CreditNoteApi#createCreditNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CreditNoteApi#createCreditNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
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

<a id="downloadCreditNotePdf"></a>
# **downloadCreditNotePdf**
> downloadCreditNotePdf(creditNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CreditNoteApi()
val creditNoteId : kotlin.String = creditNoteId_example // kotlin.String | 
try {
    apiInstance.downloadCreditNotePdf(creditNoteId)
} catch (e: ClientException) {
    println("4xx response calling CreditNoteApi#downloadCreditNotePdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CreditNoteApi#downloadCreditNotePdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **creditNoteId** | **kotlin.String**|  | |

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

<a id="getCreditNote"></a>
# **getCreditNote**
> Invoice getCreditNote(creditNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CreditNoteApi()
val creditNoteId : kotlin.String = creditNoteId_example // kotlin.String | 
try {
    val result : Invoice = apiInstance.getCreditNote(creditNoteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CreditNoteApi#getCreditNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CreditNoteApi#getCreditNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **creditNoteId** | **kotlin.String**|  | |

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

<a id="listCreditNotes"></a>
# **listCreditNotes**
> kotlin.collections.List&lt;Invoice&gt; listCreditNotes(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CreditNoteApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Invoice> = apiInstance.listCreditNotes(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CreditNoteApi#listCreditNotes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CreditNoteApi#listCreditNotes")
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

