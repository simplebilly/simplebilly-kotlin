# FristenApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**fristenApi**](FristenApi.md#fristenApi) | **GET** /api/v1/bookkeeping/fristen |  |


<a id="fristenApi"></a>
# **fristenApi**
> FristenErgebnis fristenApi(bundesland, voranmeldungsrhythmus, dauerfristverlaengerung, estAktiv, gewstAktiv, monate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = FristenApi()
val bundesland : kotlin.String = bundesland_example // kotlin.String | 
val voranmeldungsrhythmus : kotlin.String = voranmeldungsrhythmus_example // kotlin.String | 
val dauerfristverlaengerung : kotlin.Boolean = true // kotlin.Boolean | 
val estAktiv : kotlin.Boolean = true // kotlin.Boolean | 
val gewstAktiv : kotlin.Boolean = true // kotlin.Boolean | 
val monate : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : FristenErgebnis = apiInstance.fristenApi(bundesland, voranmeldungsrhythmus, dauerfristverlaengerung, estAktiv, gewstAktiv, monate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling FristenApi#fristenApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling FristenApi#fristenApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bundesland** | **kotlin.String**|  | [optional] |
| **voranmeldungsrhythmus** | **kotlin.String**|  | [optional] |
| **dauerfristverlaengerung** | **kotlin.Boolean**|  | [optional] |
| **estAktiv** | **kotlin.Boolean**|  | [optional] |
| **gewstAktiv** | **kotlin.Boolean**|  | [optional] |
| **monate** | **kotlin.Int**|  | [optional] |

### Return type

[**FristenErgebnis**](FristenErgebnis.md)

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

