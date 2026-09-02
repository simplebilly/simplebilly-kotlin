# AttachmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**attachmentRestore**](AttachmentApi.md#attachmentRestore) | **POST** /api/v1/attachments/{id}/restore |  |
| [**createAttachment**](AttachmentApi.md#createAttachment) | **POST** /api/v1/attachments |  |
| [**deleteAttachment**](AttachmentApi.md#deleteAttachment) | **DELETE** /api/v1/attachments/{id} |  |
| [**getAttachment**](AttachmentApi.md#getAttachment) | **GET** /api/v1/attachments/{id} |  |
| [**listAttachments**](AttachmentApi.md#listAttachments) | **GET** /api/v1/attachments/ |  |
| [**saveAttachmentOcrText**](AttachmentApi.md#saveAttachmentOcrText) | **PUT** /api/v1/attachments/{attachment_id}/ocr-text | Persist client-side OCR output for an attachment. |


<a id="attachmentRestore"></a>
# **attachmentRestore**
> Attachment attachmentRestore(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Attachment = apiInstance.attachmentRestore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentApi#attachmentRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentApi#attachmentRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Attachment**](Attachment.md)

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

<a id="createAttachment"></a>
# **createAttachment**
> Attachment createAttachment(attachmentCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentApi()
val attachmentCreate : AttachmentCreate =  // AttachmentCreate | 
try {
    val result : Attachment = apiInstance.createAttachment(attachmentCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentApi#createAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentApi#createAttachment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attachmentCreate** | [**AttachmentCreate**](AttachmentCreate.md)|  | |

### Return type

[**Attachment**](Attachment.md)

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

<a id="deleteAttachment"></a>
# **deleteAttachment**
> deleteAttachment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteAttachment(id)
} catch (e: ClientException) {
    println("4xx response calling AttachmentApi#deleteAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentApi#deleteAttachment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="getAttachment"></a>
# **getAttachment**
> Attachment getAttachment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Attachment = apiInstance.getAttachment(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentApi#getAttachment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentApi#getAttachment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Attachment**](Attachment.md)

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

<a id="listAttachments"></a>
# **listAttachments**
> kotlin.collections.List&lt;Attachment&gt; listAttachments(page, pageSize, contactId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Attachment> = apiInstance.listAttachments(page, pageSize, contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentApi#listAttachments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentApi#listAttachments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **contactId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Attachment&gt;**](Attachment.md)

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

<a id="saveAttachmentOcrText"></a>
# **saveAttachmentOcrText**
> Attachment saveAttachmentOcrText(attachmentId, ocrTextRequest)

Persist client-side OCR output for an attachment.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentApi()
val attachmentId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val ocrTextRequest : OcrTextRequest =  // OcrTextRequest | 
try {
    val result : Attachment = apiInstance.saveAttachmentOcrText(attachmentId, ocrTextRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentApi#saveAttachmentOcrText")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentApi#saveAttachmentOcrText")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attachmentId** | **java.util.UUID**|  | |
| **ocrTextRequest** | [**OcrTextRequest**](OcrTextRequest.md)|  | |

### Return type

[**Attachment**](Attachment.md)

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

