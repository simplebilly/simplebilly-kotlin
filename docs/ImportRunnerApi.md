# ImportRunnerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getImportStatus**](ImportRunnerApi.md#getImportStatus) | **GET** /api/v1/import/{job_id} |  |
| [**startImport**](ImportRunnerApi.md#startImport) | **POST** /api/v1/import/start |  |
| [**testImportConnection**](ImportRunnerApi.md#testImportConnection) | **POST** /api/v1/import/test |  |


<a id="getImportStatus"></a>
# **getImportStatus**
> ImportJobStatus getImportStatus(jobId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ImportRunnerApi()
val jobId : kotlin.String = jobId_example // kotlin.String | 
try {
    val result : ImportJobStatus = apiInstance.getImportStatus(jobId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImportRunnerApi#getImportStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImportRunnerApi#getImportStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **jobId** | **kotlin.String**|  | |

### Return type

[**ImportJobStatus**](ImportJobStatus.md)

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

<a id="startImport"></a>
# **startImport**
> ImportStartResponse startImport(importStartRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ImportRunnerApi()
val importStartRequest : ImportStartRequest =  // ImportStartRequest | 
try {
    val result : ImportStartResponse = apiInstance.startImport(importStartRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImportRunnerApi#startImport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImportRunnerApi#startImport")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **importStartRequest** | [**ImportStartRequest**](ImportStartRequest.md)|  | |

### Return type

[**ImportStartResponse**](ImportStartResponse.md)

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

<a id="testImportConnection"></a>
# **testImportConnection**
> ImportTestResponse testImportConnection(importTestRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ImportRunnerApi()
val importTestRequest : ImportTestRequest =  // ImportTestRequest | 
try {
    val result : ImportTestResponse = apiInstance.testImportConnection(importTestRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ImportRunnerApi#testImportConnection")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ImportRunnerApi#testImportConnection")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **importTestRequest** | [**ImportTestRequest**](ImportTestRequest.md)|  | |

### Return type

[**ImportTestResponse**](ImportTestResponse.md)

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

