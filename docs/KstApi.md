# KstApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**kstApi**](KstApi.md#kstApi) | **GET** /api/v1/bookkeeping/kst |  |


<a id="kstApi"></a>
# **kstApi**
> KstErgebnis kstApi(year, gewinn)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KstApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val gewinn : kotlin.String = gewinn_example // kotlin.String | 
try {
    val result : KstErgebnis = apiInstance.kstApi(year, gewinn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KstApi#kstApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KstApi#kstApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |
| **gewinn** | **kotlin.String**|  | [optional] |

### Return type

[**KstErgebnis**](KstErgebnis.md)

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

