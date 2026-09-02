# SupplierInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createSupplierInvoice**](SupplierInvoiceApi.md#createSupplierInvoice) | **POST** /api/v1/supplier-invoices |  |
| [**deleteSupplierInvoice**](SupplierInvoiceApi.md#deleteSupplierInvoice) | **DELETE** /api/v1/supplier-invoices/{supplier_invoice_id} |  |
| [**getSupplierInvoice**](SupplierInvoiceApi.md#getSupplierInvoice) | **GET** /api/v1/supplier-invoices/{supplier_invoice_id} |  |
| [**listSupplierInvoices**](SupplierInvoiceApi.md#listSupplierInvoices) | **GET** /api/v1/supplier-invoices/ |  |
| [**updateSupplierInvoice**](SupplierInvoiceApi.md#updateSupplierInvoice) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id} |  |
| [**updateSupplierInvoiceStatus**](SupplierInvoiceApi.md#updateSupplierInvoiceStatus) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id}/status |  |


<a id="createSupplierInvoice"></a>
# **createSupplierInvoice**
> SupplierInvoice createSupplierInvoice(supplierInvoice)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierInvoiceApi()
val supplierInvoice : SupplierInvoice =  // SupplierInvoice | 
try {
    val result : SupplierInvoice = apiInstance.createSupplierInvoice(supplierInvoice)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierInvoiceApi#createSupplierInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierInvoiceApi#createSupplierInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierInvoice** | [**SupplierInvoice**](SupplierInvoice.md)|  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

<a id="deleteSupplierInvoice"></a>
# **deleteSupplierInvoice**
> deleteSupplierInvoice(supplierInvoiceId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierInvoiceApi()
val supplierInvoiceId : kotlin.String = supplierInvoiceId_example // kotlin.String | 
try {
    apiInstance.deleteSupplierInvoice(supplierInvoiceId)
} catch (e: ClientException) {
    println("4xx response calling SupplierInvoiceApi#deleteSupplierInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierInvoiceApi#deleteSupplierInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierInvoiceId** | **kotlin.String**|  | |

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

<a id="getSupplierInvoice"></a>
# **getSupplierInvoice**
> SupplierInvoice getSupplierInvoice(supplierInvoiceId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierInvoiceApi()
val supplierInvoiceId : kotlin.String = supplierInvoiceId_example // kotlin.String | 
try {
    val result : SupplierInvoice = apiInstance.getSupplierInvoice(supplierInvoiceId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierInvoiceApi#getSupplierInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierInvoiceApi#getSupplierInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierInvoiceId** | **kotlin.String**|  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

<a id="listSupplierInvoices"></a>
# **listSupplierInvoices**
> kotlin.collections.List&lt;SupplierInvoice&gt; listSupplierInvoices(page, pageSize, status, purchaseOrderId, supplierName)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierInvoiceApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
val supplierName : kotlin.String = supplierName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<SupplierInvoice> = apiInstance.listSupplierInvoices(page, pageSize, status, purchaseOrderId, supplierName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierInvoiceApi#listSupplierInvoices")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierInvoiceApi#listSupplierInvoices")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **purchaseOrderId** | **kotlin.String**|  | [optional] |
| **supplierName** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;SupplierInvoice&gt;**](SupplierInvoice.md)

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

<a id="updateSupplierInvoice"></a>
# **updateSupplierInvoice**
> SupplierInvoice updateSupplierInvoice(supplierInvoiceId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierInvoiceApi()
val supplierInvoiceId : kotlin.String = supplierInvoiceId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : SupplierInvoice = apiInstance.updateSupplierInvoice(supplierInvoiceId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierInvoiceApi#updateSupplierInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierInvoiceApi#updateSupplierInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierInvoiceId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

<a id="updateSupplierInvoiceStatus"></a>
# **updateSupplierInvoiceStatus**
> SupplierInvoice updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierInvoiceApi()
val supplierInvoiceId : kotlin.String = supplierInvoiceId_example // kotlin.String | 
val supplierInvoiceStatusUpdate : SupplierInvoiceStatusUpdate =  // SupplierInvoiceStatusUpdate | 
try {
    val result : SupplierInvoice = apiInstance.updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierInvoiceApi#updateSupplierInvoiceStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierInvoiceApi#updateSupplierInvoiceStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierInvoiceId** | **kotlin.String**|  | |
| **supplierInvoiceStatusUpdate** | [**SupplierInvoiceStatusUpdate**](SupplierInvoiceStatusUpdate.md)|  | |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

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

