# UstvaApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**jahresustApi**](UstvaApi.md#jahresustApi) | **GET** /api/v1/bookkeeping/jahresust |  |
| [**ustvaApi**](UstvaApi.md#ustvaApi) | **GET** /api/v1/bookkeeping/ustva |  |


<a id="jahresustApi"></a>
# **jahresustApi**
> JahresUstErgebnis jahresustApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UstvaApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : JahresUstErgebnis = apiInstance.jahresustApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UstvaApi#jahresustApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UstvaApi#jahresustApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**JahresUstErgebnis**](JahresUstErgebnis.md)

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

<a id="ustvaApi"></a>
# **ustvaApi**
> UstvaErgebnis ustvaApi(zeitraum)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UstvaApi()
val zeitraum : kotlin.String = zeitraum_example // kotlin.String | 
try {
    val result : UstvaErgebnis = apiInstance.ustvaApi(zeitraum)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UstvaApi#ustvaApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UstvaApi#ustvaApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zeitraum** | **kotlin.String**|  | |

### Return type

[**UstvaErgebnis**](UstvaErgebnis.md)

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

