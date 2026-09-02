# GenerateQrcodeApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**generateQrcodeApi**](GenerateQrcodeApi.md#generateQrcodeApi) | **GET** /api/v1/invoices/{id}/qrcode |  |


<a id="generateQrcodeApi"></a>
# **generateQrcodeApi**
> QRCodeResponse generateQrcodeApi(id, iban, holderName, bic, amount, reference, purpose)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GenerateQrcodeApi()
val id : kotlin.String = id_example // kotlin.String | 
val iban : kotlin.String = iban_example // kotlin.String | 
val holderName : kotlin.String = holderName_example // kotlin.String | 
val bic : kotlin.String = bic_example // kotlin.String | 
val amount : kotlin.String = amount_example // kotlin.String | 
val reference : kotlin.String = reference_example // kotlin.String | 
val purpose : kotlin.String = purpose_example // kotlin.String | 
try {
    val result : QRCodeResponse = apiInstance.generateQrcodeApi(id, iban, holderName, bic, amount, reference, purpose)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GenerateQrcodeApi#generateQrcodeApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GenerateQrcodeApi#generateQrcodeApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |
| **iban** | **kotlin.String**|  | |
| **holderName** | **kotlin.String**|  | [optional] |
| **bic** | **kotlin.String**|  | [optional] |
| **amount** | **kotlin.String**|  | [optional] |
| **reference** | **kotlin.String**|  | [optional] |
| **purpose** | **kotlin.String**|  | [optional] |

### Return type

[**QRCodeResponse**](QRCodeResponse.md)

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

