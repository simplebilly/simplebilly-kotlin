# DeliveryNoteApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createDeliveryNote**](DeliveryNoteApi.md#createDeliveryNote) | **POST** /api/v1/delivery-notes |  |
| [**deleteDeliveryNote**](DeliveryNoteApi.md#deleteDeliveryNote) | **DELETE** /api/v1/delivery-notes/{delivery_note_id} |  |
| [**deliverynoteRestore**](DeliveryNoteApi.md#deliverynoteRestore) | **POST** /api/v1/delivery-notes/{delivery_note_id}/restore |  |
| [**downloadDeliveryNotePdf**](DeliveryNoteApi.md#downloadDeliveryNotePdf) | **GET** /api/v1/delivery-notes/{delivery_note_id}/pdf |  |
| [**getDeliveryNote**](DeliveryNoteApi.md#getDeliveryNote) | **GET** /api/v1/delivery-notes/{delivery_note_id} |  |
| [**listDeliveryNotes**](DeliveryNoteApi.md#listDeliveryNotes) | **GET** /api/v1/delivery-notes/ |  |
| [**pursueDeliveryNote**](DeliveryNoteApi.md#pursueDeliveryNote) | **POST** /api/v1/delivery-notes/{delivery_note_id}/pursue |  |


<a id="createDeliveryNote"></a>
# **createDeliveryNote**
> DeliveryNote createDeliveryNote(deliveryNoteCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val deliveryNoteCreate : DeliveryNoteCreate =  // DeliveryNoteCreate | 
try {
    val result : DeliveryNote = apiInstance.createDeliveryNote(deliveryNoteCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#createDeliveryNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#createDeliveryNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryNoteCreate** | [**DeliveryNoteCreate**](DeliveryNoteCreate.md)|  | |

### Return type

[**DeliveryNote**](DeliveryNote.md)

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

<a id="deleteDeliveryNote"></a>
# **deleteDeliveryNote**
> deleteDeliveryNote(deliveryNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val deliveryNoteId : kotlin.String = deliveryNoteId_example // kotlin.String | 
try {
    apiInstance.deleteDeliveryNote(deliveryNoteId)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#deleteDeliveryNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#deleteDeliveryNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryNoteId** | **kotlin.String**|  | |

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

<a id="deliverynoteRestore"></a>
# **deliverynoteRestore**
> DeliveryNote deliverynoteRestore(deliveryNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val deliveryNoteId : kotlin.String = deliveryNoteId_example // kotlin.String | 
try {
    val result : DeliveryNote = apiInstance.deliverynoteRestore(deliveryNoteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#deliverynoteRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#deliverynoteRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryNoteId** | **kotlin.String**|  | |

### Return type

[**DeliveryNote**](DeliveryNote.md)

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

<a id="downloadDeliveryNotePdf"></a>
# **downloadDeliveryNotePdf**
> downloadDeliveryNotePdf(deliveryNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val deliveryNoteId : kotlin.String = deliveryNoteId_example // kotlin.String | 
try {
    apiInstance.downloadDeliveryNotePdf(deliveryNoteId)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#downloadDeliveryNotePdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#downloadDeliveryNotePdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryNoteId** | **kotlin.String**|  | |

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

<a id="getDeliveryNote"></a>
# **getDeliveryNote**
> DeliveryNote getDeliveryNote(deliveryNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val deliveryNoteId : kotlin.String = deliveryNoteId_example // kotlin.String | 
try {
    val result : DeliveryNote = apiInstance.getDeliveryNote(deliveryNoteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#getDeliveryNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#getDeliveryNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryNoteId** | **kotlin.String**|  | |

### Return type

[**DeliveryNote**](DeliveryNote.md)

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

<a id="listDeliveryNotes"></a>
# **listDeliveryNotes**
> kotlin.collections.List&lt;DeliveryNote&gt; listDeliveryNotes(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<DeliveryNote> = apiInstance.listDeliveryNotes(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#listDeliveryNotes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#listDeliveryNotes")
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

[**kotlin.collections.List&lt;DeliveryNote&gt;**](DeliveryNote.md)

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

<a id="pursueDeliveryNote"></a>
# **pursueDeliveryNote**
> Invoice pursueDeliveryNote(deliveryNoteId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryNoteApi()
val deliveryNoteId : kotlin.String = deliveryNoteId_example // kotlin.String | 
try {
    val result : Invoice = apiInstance.pursueDeliveryNote(deliveryNoteId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryNoteApi#pursueDeliveryNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryNoteApi#pursueDeliveryNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryNoteId** | **kotlin.String**|  | |

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

