# EuerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**euerApi**](EuerApi.md#euerApi) | **GET** /api/v1/bookkeeping/euer |  |
| [**euerKategorienApi**](EuerApi.md#euerKategorienApi) | **GET** /api/v1/bookkeeping/euer/kategorien |  |


<a id="euerApi"></a>
# **euerApi**
> EuerErgebnis euerApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EuerApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EuerErgebnis = apiInstance.euerApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EuerApi#euerApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EuerApi#euerApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**EuerErgebnis**](EuerErgebnis.md)

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

<a id="euerKategorienApi"></a>
# **euerKategorienApi**
> EuerDetailErgebnis euerKategorienApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EuerApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EuerDetailErgebnis = apiInstance.euerKategorienApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EuerApi#euerKategorienApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EuerApi#euerKategorienApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**EuerDetailErgebnis**](EuerDetailErgebnis.md)

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

