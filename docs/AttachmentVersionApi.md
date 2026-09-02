# AttachmentVersionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createAttachmentVersion**](AttachmentVersionApi.md#createAttachmentVersion) | **POST** /api/v1/attachments/{attachment_id}/versions |  |
| [**listAttachmentVersions**](AttachmentVersionApi.md#listAttachmentVersions) | **GET** /api/v1/attachments/{attachment_id}/versions |  |
| [**restoreAttachmentVersion**](AttachmentVersionApi.md#restoreAttachmentVersion) | **POST** /api/v1/attachments/{attachment_id}/versions/{version_id}/restore |  |


<a id="createAttachmentVersion"></a>
# **createAttachmentVersion**
> AttachmentVersion createAttachmentVersion(attachmentId, newVersionRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentVersionApi()
val attachmentId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val newVersionRequest : NewVersionRequest =  // NewVersionRequest | 
try {
    val result : AttachmentVersion = apiInstance.createAttachmentVersion(attachmentId, newVersionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentVersionApi#createAttachmentVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentVersionApi#createAttachmentVersion")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attachmentId** | **java.util.UUID**|  | |
| **newVersionRequest** | [**NewVersionRequest**](NewVersionRequest.md)|  | |

### Return type

[**AttachmentVersion**](AttachmentVersion.md)

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

<a id="listAttachmentVersions"></a>
# **listAttachmentVersions**
> kotlin.collections.List&lt;AttachmentVersion&gt; listAttachmentVersions(attachmentId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentVersionApi()
val attachmentId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.collections.List<AttachmentVersion> = apiInstance.listAttachmentVersions(attachmentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentVersionApi#listAttachmentVersions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentVersionApi#listAttachmentVersions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attachmentId** | **java.util.UUID**|  | |

### Return type

[**kotlin.collections.List&lt;AttachmentVersion&gt;**](AttachmentVersion.md)

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

<a id="restoreAttachmentVersion"></a>
# **restoreAttachmentVersion**
> Attachment restoreAttachmentVersion(attachmentId, versionId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AttachmentVersionApi()
val attachmentId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val versionId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Attachment = apiInstance.restoreAttachmentVersion(attachmentId, versionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AttachmentVersionApi#restoreAttachmentVersion")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AttachmentVersionApi#restoreAttachmentVersion")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attachmentId** | **java.util.UUID**|  | |
| **versionId** | **java.util.UUID**|  | |

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

