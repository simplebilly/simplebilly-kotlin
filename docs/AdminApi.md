# AdminApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**triggerMirror**](AdminApi.md#triggerMirror) | **POST** /api/v1/admin/storage/mirror |  |


<a id="triggerMirror"></a>
# **triggerMirror**
> MirrorTriggerResponse triggerMirror()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AdminApi()
try {
    val result : MirrorTriggerResponse = apiInstance.triggerMirror()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AdminApi#triggerMirror")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AdminApi#triggerMirror")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**MirrorTriggerResponse**](MirrorTriggerResponse.md)

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

