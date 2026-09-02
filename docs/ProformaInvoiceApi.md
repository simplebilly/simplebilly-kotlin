# ProformaInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**convertProformaToInvoice**](ProformaInvoiceApi.md#convertProformaToInvoice) | **POST** /api/v1/proforma-invoices/{proforma_id}/convert |  |
| [**createProformaInvoice**](ProformaInvoiceApi.md#createProformaInvoice) | **POST** /api/v1/proforma-invoices |  |
| [**deleteProformaInvoice**](ProformaInvoiceApi.md#deleteProformaInvoice) | **DELETE** /api/v1/proforma-invoices/{proforma_id} |  |
| [**getProformaInvoice**](ProformaInvoiceApi.md#getProformaInvoice) | **GET** /api/v1/proforma-invoices/{proforma_id} |  |
| [**listProformaInvoices**](ProformaInvoiceApi.md#listProformaInvoices) | **GET** /api/v1/proforma-invoices/ |  |
| [**updateProformaInvoice**](ProformaInvoiceApi.md#updateProformaInvoice) | **PUT** /api/v1/proforma-invoices/{proforma_id} |  |


<a id="convertProformaToInvoice"></a>
# **convertProformaToInvoice**
> ConvertResponse convertProformaToInvoice(proformaId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProformaInvoiceApi()
val proformaId : kotlin.String = proformaId_example // kotlin.String | 
try {
    val result : ConvertResponse = apiInstance.convertProformaToInvoice(proformaId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProformaInvoiceApi#convertProformaToInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProformaInvoiceApi#convertProformaToInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **proformaId** | **kotlin.String**|  | |

### Return type

[**ConvertResponse**](ConvertResponse.md)

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

<a id="createProformaInvoice"></a>
# **createProformaInvoice**
> ProformaInvoice createProformaInvoice(proformaInvoice)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProformaInvoiceApi()
val proformaInvoice : ProformaInvoice =  // ProformaInvoice | 
try {
    val result : ProformaInvoice = apiInstance.createProformaInvoice(proformaInvoice)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProformaInvoiceApi#createProformaInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProformaInvoiceApi#createProformaInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **proformaInvoice** | [**ProformaInvoice**](ProformaInvoice.md)|  | |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="deleteProformaInvoice"></a>
# **deleteProformaInvoice**
> deleteProformaInvoice(proformaId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProformaInvoiceApi()
val proformaId : kotlin.String = proformaId_example // kotlin.String | 
try {
    apiInstance.deleteProformaInvoice(proformaId)
} catch (e: ClientException) {
    println("4xx response calling ProformaInvoiceApi#deleteProformaInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProformaInvoiceApi#deleteProformaInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **proformaId** | **kotlin.String**|  | |

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
 - **Accept**: application/json

<a id="getProformaInvoice"></a>
# **getProformaInvoice**
> ProformaInvoice getProformaInvoice(proformaId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProformaInvoiceApi()
val proformaId : kotlin.String = proformaId_example // kotlin.String | 
try {
    val result : ProformaInvoice = apiInstance.getProformaInvoice(proformaId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProformaInvoiceApi#getProformaInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProformaInvoiceApi#getProformaInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **proformaId** | **kotlin.String**|  | |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

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

<a id="listProformaInvoices"></a>
# **listProformaInvoices**
> kotlin.collections.List&lt;ProformaInvoice&gt; listProformaInvoices(page, pageSize, status, customerId, orderNumber)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProformaInvoiceApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val customerId : kotlin.String = customerId_example // kotlin.String | 
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ProformaInvoice> = apiInstance.listProformaInvoices(page, pageSize, status, customerId, orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProformaInvoiceApi#listProformaInvoices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProformaInvoiceApi#listProformaInvoices")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **customerId** | **kotlin.String**|  | [optional] |
| **orderNumber** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ProformaInvoice&gt;**](ProformaInvoice.md)

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

<a id="updateProformaInvoice"></a>
# **updateProformaInvoice**
> ProformaInvoice updateProformaInvoice(proformaId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProformaInvoiceApi()
val proformaId : kotlin.String = proformaId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : ProformaInvoice = apiInstance.updateProformaInvoice(proformaId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProformaInvoiceApi#updateProformaInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProformaInvoiceApi#updateProformaInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **proformaId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

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

 - **Content-Type**: application/json
 - **Accept**: application/json

