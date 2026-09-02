# RecurringTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createRecurringTemplate**](RecurringTemplateApi.md#createRecurringTemplate) | **POST** /api/v1/recurring-templates |  |
| [**deleteRecurringTemplate**](RecurringTemplateApi.md#deleteRecurringTemplate) | **DELETE** /api/v1/recurring-templates/{template_id} |  |
| [**getRecurringTemplate**](RecurringTemplateApi.md#getRecurringTemplate) | **GET** /api/v1/recurring-templates/{template_id} |  |
| [**listRecurringTemplates**](RecurringTemplateApi.md#listRecurringTemplates) | **GET** /api/v1/recurring-templates/ |  |


<a id="createRecurringTemplate"></a>
# **createRecurringTemplate**
> RecurringTemplate createRecurringTemplate(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RecurringTemplateApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : RecurringTemplate = apiInstance.createRecurringTemplate(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecurringTemplateApi#createRecurringTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecurringTemplateApi#createRecurringTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**RecurringTemplate**](RecurringTemplate.md)

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

<a id="deleteRecurringTemplate"></a>
# **deleteRecurringTemplate**
> deleteRecurringTemplate(templateId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RecurringTemplateApi()
val templateId : kotlin.String = templateId_example // kotlin.String | 
try {
    apiInstance.deleteRecurringTemplate(templateId)
} catch (e: ClientException) {
    println("4xx response calling RecurringTemplateApi#deleteRecurringTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecurringTemplateApi#deleteRecurringTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **templateId** | **kotlin.String**|  | |

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

<a id="getRecurringTemplate"></a>
# **getRecurringTemplate**
> RecurringTemplate getRecurringTemplate(templateId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RecurringTemplateApi()
val templateId : kotlin.String = templateId_example // kotlin.String | 
try {
    val result : RecurringTemplate = apiInstance.getRecurringTemplate(templateId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecurringTemplateApi#getRecurringTemplate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecurringTemplateApi#getRecurringTemplate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **templateId** | **kotlin.String**|  | |

### Return type

[**RecurringTemplate**](RecurringTemplate.md)

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

<a id="listRecurringTemplates"></a>
# **listRecurringTemplates**
> kotlin.collections.List&lt;RecurringTemplate&gt; listRecurringTemplates()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RecurringTemplateApi()
try {
    val result : kotlin.collections.List<RecurringTemplate> = apiInstance.listRecurringTemplates()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RecurringTemplateApi#listRecurringTemplates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RecurringTemplateApi#listRecurringTemplates")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;RecurringTemplate&gt;**](RecurringTemplate.md)

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

