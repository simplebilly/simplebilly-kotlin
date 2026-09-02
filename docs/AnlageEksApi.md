# AnlageEksApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**eksApi**](AnlageEksApi.md#eksApi) | **GET** /api/v1/bookkeeping/eks |  |


<a id="eksApi"></a>
# **eksApi**
> EksErgebnis eksApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AnlageEksApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EksErgebnis = apiInstance.eksApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnlageEksApi#eksApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnlageEksApi#eksApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**EksErgebnis**](EksErgebnis.md)

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

