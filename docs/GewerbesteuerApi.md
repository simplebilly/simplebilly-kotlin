# GewerbesteuerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gewerbesteuerApi**](GewerbesteuerApi.md#gewerbesteuerApi) | **GET** /api/v1/bookkeeping/gewerbesteuer |  |


<a id="gewerbesteuerApi"></a>
# **gewerbesteuerApi**
> GewerbesteuerErgebnis gewerbesteuerApi(year, hebesatz, gewerbeertrag, country, gemeindeschluessel)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GewerbesteuerApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val hebesatz : kotlin.String = hebesatz_example // kotlin.String | 
val gewerbeertrag : kotlin.String = gewerbeertrag_example // kotlin.String | 
val country : kotlin.String = country_example // kotlin.String | 
val gemeindeschluessel : kotlin.String = gemeindeschluessel_example // kotlin.String | 
try {
    val result : GewerbesteuerErgebnis = apiInstance.gewerbesteuerApi(year, hebesatz, gewerbeertrag, country, gemeindeschluessel)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GewerbesteuerApi#gewerbesteuerApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GewerbesteuerApi#gewerbesteuerApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |
| **hebesatz** | **kotlin.String**|  | [optional] |
| **gewerbeertrag** | **kotlin.String**|  | [optional] |
| **country** | **kotlin.String**|  | [optional] |
| **gemeindeschluessel** | **kotlin.String**|  | [optional] |

### Return type

[**GewerbesteuerErgebnis**](GewerbesteuerErgebnis.md)

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

