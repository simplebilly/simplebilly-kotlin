# AiApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**aiSuggestApi**](AiApi.md#aiSuggestApi) | **POST** /api/v1/support/ai/suggest |  |
| [**createWorkerApi**](AiApi.md#createWorkerApi) | **POST** /api/v1/support/ai/workers |  |
| [**listWorkersApi**](AiApi.md#listWorkersApi) | **GET** /api/v1/support/ai/workers |  |
| [**runWorkerApi**](AiApi.md#runWorkerApi) | **POST** /api/v1/support/ai/workers/{worker_id}/run |  |


<a id="aiSuggestApi"></a>
# **aiSuggestApi**
> AiSuggestion aiSuggestApi(aiSuggestionRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AiApi()
val aiSuggestionRequest : AiSuggestionRequest =  // AiSuggestionRequest | 
try {
    val result : AiSuggestion = apiInstance.aiSuggestApi(aiSuggestionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiApi#aiSuggestApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiApi#aiSuggestApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiSuggestionRequest** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  | |

### Return type

[**AiSuggestion**](AiSuggestion.md)

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

<a id="createWorkerApi"></a>
# **createWorkerApi**
> AiWorkerConfig createWorkerApi(aiConfigDto)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AiApi()
val aiConfigDto : AiConfigDto =  // AiConfigDto | 
try {
    val result : AiWorkerConfig = apiInstance.createWorkerApi(aiConfigDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiApi#createWorkerApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiApi#createWorkerApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **aiConfigDto** | [**AiConfigDto**](AiConfigDto.md)|  | |

### Return type

[**AiWorkerConfig**](AiWorkerConfig.md)

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

<a id="listWorkersApi"></a>
# **listWorkersApi**
> kotlin.collections.List&lt;AiWorkerConfig&gt; listWorkersApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AiApi()
try {
    val result : kotlin.collections.List<AiWorkerConfig> = apiInstance.listWorkersApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiApi#listWorkersApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiApi#listWorkersApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;AiWorkerConfig&gt;**](AiWorkerConfig.md)

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

<a id="runWorkerApi"></a>
# **runWorkerApi**
> AiSuggestion runWorkerApi(workerId, aiSuggestionRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AiApi()
val workerId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val aiSuggestionRequest : AiSuggestionRequest =  // AiSuggestionRequest | 
try {
    val result : AiSuggestion = apiInstance.runWorkerApi(workerId, aiSuggestionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AiApi#runWorkerApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AiApi#runWorkerApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **workerId** | **java.util.UUID**|  | |
| **aiSuggestionRequest** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  | |

### Return type

[**AiSuggestion**](AiSuggestion.md)

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

