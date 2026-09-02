# KostenVorschauApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kostenVorschauApi**](KostenVorschauApi.md#kostenVorschauApi) | **GET** /api/v1/bookkeeping/kosten-vorschau |  |


<a id="kostenVorschauApi"></a>
# **kostenVorschauApi**
> KostenVorschau kostenVorschauApi(year, month)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KostenVorschauApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : KostenVorschau = apiInstance.kostenVorschauApi(year, month)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KostenVorschauApi#kostenVorschauApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KostenVorschauApi#kostenVorschauApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |
| **month** | **kotlin.Int**|  | |

### Return type

[**KostenVorschau**](KostenVorschau.md)

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

