# GoodsReceiptApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createGoodsReceipt**](GoodsReceiptApi.md#createGoodsReceipt) | **POST** /api/v1/goods-receipts |  |
| [**deleteGoodsReceipt**](GoodsReceiptApi.md#deleteGoodsReceipt) | **DELETE** /api/v1/goods-receipts/{goods_receipt_id} |  |
| [**getGoodsReceipt**](GoodsReceiptApi.md#getGoodsReceipt) | **GET** /api/v1/goods-receipts/{goods_receipt_id} |  |
| [**listGoodsReceipts**](GoodsReceiptApi.md#listGoodsReceipts) | **GET** /api/v1/goods-receipts/ |  |


<a id="createGoodsReceipt"></a>
# **createGoodsReceipt**
> GoodsReceipt createGoodsReceipt(goodsReceipt)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GoodsReceiptApi()
val goodsReceipt : GoodsReceipt =  // GoodsReceipt | 
try {
    val result : GoodsReceipt = apiInstance.createGoodsReceipt(goodsReceipt)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GoodsReceiptApi#createGoodsReceipt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GoodsReceiptApi#createGoodsReceipt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **goodsReceipt** | [**GoodsReceipt**](GoodsReceipt.md)|  | |

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

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

<a id="deleteGoodsReceipt"></a>
# **deleteGoodsReceipt**
> deleteGoodsReceipt(goodsReceiptId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GoodsReceiptApi()
val goodsReceiptId : kotlin.String = goodsReceiptId_example // kotlin.String | 
try {
    apiInstance.deleteGoodsReceipt(goodsReceiptId)
} catch (e: ClientException) {
    println("4xx response calling GoodsReceiptApi#deleteGoodsReceipt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GoodsReceiptApi#deleteGoodsReceipt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **goodsReceiptId** | **kotlin.String**|  | |

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

<a id="getGoodsReceipt"></a>
# **getGoodsReceipt**
> GoodsReceipt getGoodsReceipt(goodsReceiptId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GoodsReceiptApi()
val goodsReceiptId : kotlin.String = goodsReceiptId_example // kotlin.String | 
try {
    val result : GoodsReceipt = apiInstance.getGoodsReceipt(goodsReceiptId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GoodsReceiptApi#getGoodsReceipt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GoodsReceiptApi#getGoodsReceipt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **goodsReceiptId** | **kotlin.String**|  | |

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

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

<a id="listGoodsReceipts"></a>
# **listGoodsReceipts**
> kotlin.collections.List&lt;GoodsReceipt&gt; listGoodsReceipts(page, pageSize, purchaseOrderId, supplierName, warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GoodsReceiptApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val purchaseOrderId : kotlin.String = purchaseOrderId_example // kotlin.String | 
val supplierName : kotlin.String = supplierName_example // kotlin.String | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<GoodsReceipt> = apiInstance.listGoodsReceipts(page, pageSize, purchaseOrderId, supplierName, warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GoodsReceiptApi#listGoodsReceipts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GoodsReceiptApi#listGoodsReceipts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **purchaseOrderId** | **kotlin.String**|  | [optional] |
| **supplierName** | **kotlin.String**|  | [optional] |
| **warehouseId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;GoodsReceipt&gt;**](GoodsReceipt.md)

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

