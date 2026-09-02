# AnlageGApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**anlageGApi**](AnlageGApi.md#anlageGApi) | **GET** /api/v1/bookkeeping/anlage-g |  |


<a id="anlageGApi"></a>
# **anlageGApi**
> AnlageGErgebnis anlageGApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AnlageGApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AnlageGErgebnis = apiInstance.anlageGApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnlageGApi#anlageGApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnlageGApi#anlageGApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**AnlageGErgebnis**](AnlageGErgebnis.md)

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

