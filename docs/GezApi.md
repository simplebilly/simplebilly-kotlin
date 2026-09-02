# GezApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**gezApi**](GezApi.md#gezApi) | **GET** /api/v1/bookkeeping/gez |  |


<a id="gezApi"></a>
# **gezApi**
> GezReport gezApi(jahr, betriebsstaetten, kfz, hotelzimmer, beschaefigte)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GezApi()
val jahr : kotlin.Int = 56 // kotlin.Int | 
val betriebsstaetten : kotlin.String = betriebsstaetten_example // kotlin.String | Liste der Betriebsstätten als JSON, z.B. `[{\"name\":\"Filiale 1\",\"beschaefigte\":12}]`.
val kfz : kotlin.Long = 789 // kotlin.Long | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind).
val hotelzimmer : kotlin.Long = 789 // kotlin.Long | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen.
val beschaefigte : kotlin.Long = 789 // kotlin.Long | Gesamtzahl der Beschäftigten (verwendet nur, wenn `betriebsstaetten` fehlt; dann wird eine einzelne Betriebsstätte angenommen).
try {
    val result : GezReport = apiInstance.gezApi(jahr, betriebsstaetten, kfz, hotelzimmer, beschaefigte)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GezApi#gezApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GezApi#gezApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **jahr** | **kotlin.Int**|  | [optional] |
| **betriebsstaetten** | **kotlin.String**| Liste der Betriebsstätten als JSON, z.B. &#x60;[{\&quot;name\&quot;:\&quot;Filiale 1\&quot;,\&quot;beschaefigte\&quot;:12}]&#x60;. | [optional] |
| **kfz** | **kotlin.Long**| Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). | [optional] |
| **hotelzimmer** | **kotlin.Long**| Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. | [optional] |
| **beschaefigte** | **kotlin.Long**| Gesamtzahl der Beschäftigten (verwendet nur, wenn &#x60;betriebsstaetten&#x60; fehlt; dann wird eine einzelne Betriebsstätte angenommen). | [optional] |

### Return type

[**GezReport**](GezReport.md)

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

