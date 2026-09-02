# OffenlegungApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**offenlegungApi**](OffenlegungApi.md#offenlegungApi) | **GET** /api/v1/bookkeeping/offenlegung |  |


<a id="offenlegungApi"></a>
# **offenlegungApi**
> OffenlegungReport offenlegungApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OffenlegungApi()
try {
    val result : OffenlegungReport = apiInstance.offenlegungApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OffenlegungApi#offenlegungApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OffenlegungApi#offenlegungApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**OffenlegungReport**](OffenlegungReport.md)

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

