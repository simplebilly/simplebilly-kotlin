# TrainingsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getMyTrainings**](TrainingsApi.md#getMyTrainings) | **GET** /api/v1/trainings/me |  |
| [**getTrainingContent**](TrainingsApi.md#getTrainingContent) | **GET** /api/v1/trainings/content/{code} |  |
| [**getTrainingOverview**](TrainingsApi.md#getTrainingOverview) | **GET** /api/v1/trainings/overview |  |
| [**submitTrainingResult**](TrainingsApi.md#submitTrainingResult) | **POST** /api/v1/trainings/submit-result |  |


<a id="getMyTrainings"></a>
# **getMyTrainings**
> kotlin.collections.List&lt;MyTrainingItem&gt; getMyTrainings()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingsApi()
try {
    val result : kotlin.collections.List<MyTrainingItem> = apiInstance.getMyTrainings()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingsApi#getMyTrainings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingsApi#getMyTrainings")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;MyTrainingItem&gt;**](MyTrainingItem.md)

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

<a id="getTrainingContent"></a>
# **getTrainingContent**
> TrainingContent getTrainingContent(code)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingsApi()
val code : kotlin.String = code_example // kotlin.String | Training code, e.g. data_privacy
try {
    val result : TrainingContent = apiInstance.getTrainingContent(code)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingsApi#getTrainingContent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingsApi#getTrainingContent")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **code** | **kotlin.String**| Training code, e.g. data_privacy | |

### Return type

[**TrainingContent**](TrainingContent.md)

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

<a id="getTrainingOverview"></a>
# **getTrainingOverview**
> kotlin.collections.List&lt;HrTrainingOverview&gt; getTrainingOverview()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingsApi()
try {
    val result : kotlin.collections.List<HrTrainingOverview> = apiInstance.getTrainingOverview()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingsApi#getTrainingOverview")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingsApi#getTrainingOverview")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;HrTrainingOverview&gt;**](HrTrainingOverview.md)

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

<a id="submitTrainingResult"></a>
# **submitTrainingResult**
> SubmitResultResponse submitTrainingResult(submitResultDto)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingsApi()
val submitResultDto : SubmitResultDto =  // SubmitResultDto | 
try {
    val result : SubmitResultResponse = apiInstance.submitTrainingResult(submitResultDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingsApi#submitTrainingResult")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingsApi#submitTrainingResult")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **submitResultDto** | [**SubmitResultDto**](SubmitResultDto.md)|  | |

### Return type

[**SubmitResultResponse**](SubmitResultResponse.md)

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

