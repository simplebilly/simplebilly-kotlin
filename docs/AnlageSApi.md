# AnlageSApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**anlageSApi**](AnlageSApi.md#anlageSApi) | **GET** /api/v1/bookkeeping/anlage-s |  |


<a id="anlageSApi"></a>
# **anlageSApi**
> AnlageSErgebnis anlageSApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AnlageSApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : AnlageSErgebnis = apiInstance.anlageSApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AnlageSApi#anlageSApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AnlageSApi#anlageSApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**AnlageSErgebnis**](AnlageSErgebnis.md)

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

