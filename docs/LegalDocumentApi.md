# LegalDocumentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getLegalDocuments**](LegalDocumentApi.md#getLegalDocuments) | **GET** /api/v1/legal/documents | List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access. |
| [**resetLegalDocuments**](LegalDocumentApi.md#resetLegalDocuments) | **POST** /api/v1/legal/documents/reset | Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list. |
| [**upsertLegalDocuments**](LegalDocumentApi.md#upsertLegalDocuments) | **PUT** /api/v1/legal/documents | Upsert legal documents per (doc_type, lang). Returns the full tenant list. |


<a id="getLegalDocuments"></a>
# **getLegalDocuments**
> kotlin.collections.List&lt;LegalDocument&gt; getLegalDocuments()

List all legal documents of the tenant. Missing documents are seeded from the default texts (with tenant placeholders replaced) on first access.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LegalDocumentApi()
try {
    val result : kotlin.collections.List<LegalDocument> = apiInstance.getLegalDocuments()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LegalDocumentApi#getLegalDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LegalDocumentApi#getLegalDocuments")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;LegalDocument&gt;**](LegalDocument.md)

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

<a id="resetLegalDocuments"></a>
# **resetLegalDocuments**
> kotlin.collections.List&lt;LegalDocument&gt; resetLegalDocuments(legalDocumentReset)

Restore default texts for all documents (or a single doc_type/lang when the optional filter is given). Returns the full tenant list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LegalDocumentApi()
val legalDocumentReset : LegalDocumentReset =  // LegalDocumentReset | 
try {
    val result : kotlin.collections.List<LegalDocument> = apiInstance.resetLegalDocuments(legalDocumentReset)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LegalDocumentApi#resetLegalDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LegalDocumentApi#resetLegalDocuments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **legalDocumentReset** | [**LegalDocumentReset**](LegalDocumentReset.md)|  | |

### Return type

[**kotlin.collections.List&lt;LegalDocument&gt;**](LegalDocument.md)

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

<a id="upsertLegalDocuments"></a>
# **upsertLegalDocuments**
> kotlin.collections.List&lt;LegalDocument&gt; upsertLegalDocuments(legalDocumentUpsert)

Upsert legal documents per (doc_type, lang). Returns the full tenant list.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LegalDocumentApi()
val legalDocumentUpsert : kotlin.collections.List<LegalDocumentUpsert> =  // kotlin.collections.List<LegalDocumentUpsert> | 
try {
    val result : kotlin.collections.List<LegalDocument> = apiInstance.upsertLegalDocuments(legalDocumentUpsert)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LegalDocumentApi#upsertLegalDocuments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LegalDocumentApi#upsertLegalDocuments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **legalDocumentUpsert** | [**kotlin.collections.List&lt;LegalDocumentUpsert&gt;**](LegalDocumentUpsert.md)|  | |

### Return type

[**kotlin.collections.List&lt;LegalDocument&gt;**](LegalDocument.md)

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

