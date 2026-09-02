# EmailTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createEmailTemplate**](EmailTemplateApi.md#createEmailTemplate) | **POST** /api/v1/email-templates |  |
| [**deleteEmailTemplate**](EmailTemplateApi.md#deleteEmailTemplate) | **DELETE** /api/v1/email-templates/{email_template_id} |  |
| [**getEmailTemplate**](EmailTemplateApi.md#getEmailTemplate) | **GET** /api/v1/email-templates/{email_template_id} |  |
| [**listEmailTemplates**](EmailTemplateApi.md#listEmailTemplates) | **GET** /api/v1/email-templates/ |  |
| [**renderEmailTemplate**](EmailTemplateApi.md#renderEmailTemplate) | **POST** /api/v1/email-templates/{email_template_id}/render |  |
| [**updateEmailTemplate**](EmailTemplateApi.md#updateEmailTemplate) | **PUT** /api/v1/email-templates/{email_template_id} |  |


<a id="createEmailTemplate"></a>
# **createEmailTemplate**
> EmailTemplate createEmailTemplate(emailTemplateCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmailTemplateApi()
val emailTemplateCreate : EmailTemplateCreate =  // EmailTemplateCreate | 
try {
    val result : EmailTemplate = apiInstance.createEmailTemplate(emailTemplateCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailTemplateApi#createEmailTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailTemplateApi#createEmailTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emailTemplateCreate** | [**EmailTemplateCreate**](EmailTemplateCreate.md)|  | |

### Return type

[**EmailTemplate**](EmailTemplate.md)

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

<a id="deleteEmailTemplate"></a>
# **deleteEmailTemplate**
> deleteEmailTemplate(emailTemplateId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmailTemplateApi()
val emailTemplateId : kotlin.String = emailTemplateId_example // kotlin.String | 
try {
    apiInstance.deleteEmailTemplate(emailTemplateId)
} catch (e: ClientException) {
    println("4xx response calling EmailTemplateApi#deleteEmailTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailTemplateApi#deleteEmailTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emailTemplateId** | **kotlin.String**|  | |

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

<a id="getEmailTemplate"></a>
# **getEmailTemplate**
> EmailTemplate getEmailTemplate(emailTemplateId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmailTemplateApi()
val emailTemplateId : kotlin.String = emailTemplateId_example // kotlin.String | 
try {
    val result : EmailTemplate = apiInstance.getEmailTemplate(emailTemplateId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailTemplateApi#getEmailTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailTemplateApi#getEmailTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emailTemplateId** | **kotlin.String**|  | |

### Return type

[**EmailTemplate**](EmailTemplate.md)

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

<a id="listEmailTemplates"></a>
# **listEmailTemplates**
> kotlin.collections.List&lt;EmailTemplate&gt; listEmailTemplates(page, pageSize, status, search)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmailTemplateApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<EmailTemplate> = apiInstance.listEmailTemplates(page, pageSize, status, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailTemplateApi#listEmailTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailTemplateApi#listEmailTemplates")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;EmailTemplate&gt;**](EmailTemplate.md)

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

<a id="renderEmailTemplate"></a>
# **renderEmailTemplate**
> kotlin.Any renderEmailTemplate(emailTemplateId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmailTemplateApi()
val emailTemplateId : kotlin.String = emailTemplateId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.renderEmailTemplate(emailTemplateId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailTemplateApi#renderEmailTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailTemplateApi#renderEmailTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emailTemplateId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="updateEmailTemplate"></a>
# **updateEmailTemplate**
> EmailTemplate updateEmailTemplate(emailTemplateId, emailTemplateUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmailTemplateApi()
val emailTemplateId : kotlin.String = emailTemplateId_example // kotlin.String | 
val emailTemplateUpdate : EmailTemplateUpdate =  // EmailTemplateUpdate | 
try {
    val result : EmailTemplate = apiInstance.updateEmailTemplate(emailTemplateId, emailTemplateUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmailTemplateApi#updateEmailTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmailTemplateApi#updateEmailTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emailTemplateId** | **kotlin.String**|  | |
| **emailTemplateUpdate** | [**EmailTemplateUpdate**](EmailTemplateUpdate.md)|  | |

### Return type

[**EmailTemplate**](EmailTemplate.md)

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

