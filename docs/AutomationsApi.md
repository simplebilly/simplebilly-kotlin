# AutomationsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listAutomations**](AutomationsApi.md#listAutomations) | **GET** /api/v1/automations |  |
| [**triggerAutomation**](AutomationsApi.md#triggerAutomation) | **POST** /api/v1/automations/{key}/trigger |  |
| [**updateAutomation**](AutomationsApi.md#updateAutomation) | **PUT** /api/v1/automations/{key} |  |


<a id="listAutomations"></a>
# **listAutomations**
> kotlin.collections.List&lt;AutomationDto&gt; listAutomations()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AutomationsApi()
try {
    val result : kotlin.collections.List<AutomationDto> = apiInstance.listAutomations()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AutomationsApi#listAutomations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AutomationsApi#listAutomations")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;AutomationDto&gt;**](AutomationDto.md)

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

<a id="triggerAutomation"></a>
# **triggerAutomation**
> kotlin.Any triggerAutomation(key)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AutomationsApi()
val key : kotlin.String = key_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.triggerAutomation(key)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AutomationsApi#triggerAutomation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AutomationsApi#triggerAutomation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |

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

 - **Content-Type**: Not defined
 - **Accept**: application/json

<a id="updateAutomation"></a>
# **updateAutomation**
> AutomationDto updateAutomation(key, updateAutomation)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AutomationsApi()
val key : kotlin.String = key_example // kotlin.String | 
val updateAutomation : UpdateAutomation =  // UpdateAutomation | 
try {
    val result : AutomationDto = apiInstance.updateAutomation(key, updateAutomation)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AutomationsApi#updateAutomation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AutomationsApi#updateAutomation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **key** | **kotlin.String**|  | |
| **updateAutomation** | [**UpdateAutomation**](UpdateAutomation.md)|  | |

### Return type

[**AutomationDto**](AutomationDto.md)

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

