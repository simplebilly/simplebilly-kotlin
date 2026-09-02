# ZugferdApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**generateZugferdApi**](ZugferdApi.md#generateZugferdApi) | **GET** /api/v1/invoices/{id}/zugferd |  |


<a id="generateZugferdApi"></a>
# **generateZugferdApi**
> generateZugferdApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ZugferdApi()
val id : kotlin.String = id_example // kotlin.String | 
val supplierName : kotlin.String = supplierName_example // kotlin.String | 
val supplierStreet : kotlin.String = supplierStreet_example // kotlin.String | 
val supplierCity : kotlin.String = supplierCity_example // kotlin.String | 
val supplierZip : kotlin.String = supplierZip_example // kotlin.String | 
val supplierCountry : kotlin.String = supplierCountry_example // kotlin.String | 
val supplierVatId : kotlin.String = supplierVatId_example // kotlin.String | 
try {
    apiInstance.generateZugferdApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId)
} catch (e: ClientException) {
    println("4xx response calling ZugferdApi#generateZugferdApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ZugferdApi#generateZugferdApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |
| **supplierName** | **kotlin.String**|  | [optional] |
| **supplierStreet** | **kotlin.String**|  | [optional] |
| **supplierCity** | **kotlin.String**|  | [optional] |
| **supplierZip** | **kotlin.String**|  | [optional] |
| **supplierCountry** | **kotlin.String**|  | [optional] |
| **supplierVatId** | **kotlin.String**|  | [optional] |

### Return type

null (empty response body)

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
 - **Accept**: Not defined

