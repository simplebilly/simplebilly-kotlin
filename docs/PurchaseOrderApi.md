# PurchaseOrderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPurchaseOrder**](PurchaseOrderApi.md#createPurchaseOrder) | **POST** /api/v1/purchase-orders |  |
| [**deletePurchaseOrder**](PurchaseOrderApi.md#deletePurchaseOrder) | **DELETE** /api/v1/purchase-orders/{purchase_order_id} |  |
| [**getPurchaseOrder**](PurchaseOrderApi.md#getPurchaseOrder) | **GET** /api/v1/purchase-orders/{purchase_order_id} |  |
| [**listPurchaseOrders**](PurchaseOrderApi.md#listPurchaseOrders) | **GET** /api/v1/purchase-orders/ |  |
| [**matchInvoice**](PurchaseOrderApi.md#matchInvoice) | **POST** /api/v1/purchase-orders/{purchase_order_id}/match-invoice | 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product. |
| [**updatePurchaseOrder**](PurchaseOrderApi.md#updatePurchaseOrder) | **PUT** /api/v1/purchase-orders/{purchase_order_id} |  |
| [**updatePurchaseOrderStatus**](PurchaseOrderApi.md#updatePurchaseOrderStatus) | **PUT** /api/v1/purchase-orders/{purchase_order_id}/status |  |


<a id="createPurchaseOrder"></a>
# **createPurchaseOrder**
> PurchaseOrder createPurchaseOrder(purchaseOrder)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val purchaseOrder : PurchaseOrder =  // PurchaseOrder | 
try {
    val result : PurchaseOrder = apiInstance.createPurchaseOrder(purchaseOrder)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#createPurchaseOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#createPurchaseOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **purchaseOrder** | [**PurchaseOrder**](PurchaseOrder.md)|  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

<a id="deletePurchaseOrder"></a>
# **deletePurchaseOrder**
> deletePurchaseOrder(purchaseOrderId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
try {
    apiInstance.deletePurchaseOrder(purchaseOrderId)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#deletePurchaseOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#deletePurchaseOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **purchaseOrderId** | **kotlin.String**|  | |

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

<a id="getPurchaseOrder"></a>
# **getPurchaseOrder**
> PurchaseOrder getPurchaseOrder(purchaseOrderId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
try {
    val result : PurchaseOrder = apiInstance.getPurchaseOrder(purchaseOrderId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#getPurchaseOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#getPurchaseOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **purchaseOrderId** | **kotlin.String**|  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

<a id="listPurchaseOrders"></a>
# **listPurchaseOrders**
> kotlin.collections.List&lt;PurchaseOrder&gt; listPurchaseOrders(page, pageSize, status, supplierName, search)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val supplierName : kotlin.String = supplierName_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PurchaseOrder> = apiInstance.listPurchaseOrders(page, pageSize, status, supplierName, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#listPurchaseOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#listPurchaseOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **supplierName** | **kotlin.String**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;PurchaseOrder&gt;**](PurchaseOrder.md)

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

<a id="matchInvoice"></a>
# **matchInvoice**
> kotlin.Any matchInvoice(purchaseOrderId, invoiceMatchRequest)

3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
val invoiceMatchRequest : InvoiceMatchRequest =  // InvoiceMatchRequest | 
try {
    val result : kotlin.Any = apiInstance.matchInvoice(purchaseOrderId, invoiceMatchRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#matchInvoice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#matchInvoice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **purchaseOrderId** | **kotlin.String**|  | |
| **invoiceMatchRequest** | [**InvoiceMatchRequest**](InvoiceMatchRequest.md)|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="updatePurchaseOrder"></a>
# **updatePurchaseOrder**
> PurchaseOrder updatePurchaseOrder(purchaseOrderId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PurchaseOrder = apiInstance.updatePurchaseOrder(purchaseOrderId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#updatePurchaseOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#updatePurchaseOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **purchaseOrderId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

<a id="updatePurchaseOrderStatus"></a>
# **updatePurchaseOrderStatus**
> PurchaseOrder updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PurchaseOrderApi()
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
val purchaseOrderStatusUpdate : PurchaseOrderStatusUpdate =  // PurchaseOrderStatusUpdate | 
try {
    val result : PurchaseOrder = apiInstance.updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PurchaseOrderApi#updatePurchaseOrderStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PurchaseOrderApi#updatePurchaseOrderStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **purchaseOrderId** | **kotlin.String**|  | |
| **purchaseOrderStatusUpdate** | [**PurchaseOrderStatusUpdate**](PurchaseOrderStatusUpdate.md)|  | |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

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

