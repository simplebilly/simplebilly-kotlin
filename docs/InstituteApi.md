# InstituteApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**instituteStatusApi**](InstituteApi.md#instituteStatusApi) | **GET** /api/v1/bookkeeping/institute/status |  |


<a id="instituteStatusApi"></a>
# **instituteStatusApi**
> InstituteStatus instituteStatusApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InstituteApi()
try {
    val result : InstituteStatus = apiInstance.instituteStatusApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InstituteApi#instituteStatusApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InstituteApi#instituteStatusApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InstituteStatus**](InstituteStatus.md)

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

