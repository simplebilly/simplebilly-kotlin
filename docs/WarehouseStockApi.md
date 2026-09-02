# WarehouseStockApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createWarehouseStock**](WarehouseStockApi.md#createWarehouseStock) | **POST** /api/v1/warehouses/{warehouse_id}/stock |  |
| [**deleteWarehouseStock**](WarehouseStockApi.md#deleteWarehouseStock) | **DELETE** /api/v1/warehouses/{warehouse_id}/stock/{product_id} |  |
| [**listWarehouseStock**](WarehouseStockApi.md#listWarehouseStock) | **GET** /api/v1/warehouses/{warehouse_id}/stock |  |
| [**updateWarehouseStock**](WarehouseStockApi.md#updateWarehouseStock) | **PUT** /api/v1/warehouses/{warehouse_id}/stock/{product_id} |  |


<a id="createWarehouseStock"></a>
# **createWarehouseStock**
> WarehouseStock createWarehouseStock(warehouseId, stockAdjustment)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseStockApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val stockAdjustment : StockAdjustment =  // StockAdjustment | 
try {
    val result : WarehouseStock = apiInstance.createWarehouseStock(warehouseId, stockAdjustment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseStockApi#createWarehouseStock")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseStockApi#createWarehouseStock")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |
| **stockAdjustment** | [**StockAdjustment**](StockAdjustment.md)|  | |

### Return type

[**WarehouseStock**](WarehouseStock.md)

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

<a id="deleteWarehouseStock"></a>
# **deleteWarehouseStock**
> deleteWarehouseStock(warehouseId, productId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseStockApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteWarehouseStock(warehouseId, productId)
} catch (e: ClientException) {
    println("4xx response calling WarehouseStockApi#deleteWarehouseStock")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseStockApi#deleteWarehouseStock")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |
| **productId** | **java.util.UUID**|  | |

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

<a id="listWarehouseStock"></a>
# **listWarehouseStock**
> kotlin.collections.List&lt;WarehouseStock&gt; listWarehouseStock(warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseStockApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<WarehouseStock> = apiInstance.listWarehouseStock(warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseStockApi#listWarehouseStock")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseStockApi#listWarehouseStock")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;WarehouseStock&gt;**](WarehouseStock.md)

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

<a id="updateWarehouseStock"></a>
# **updateWarehouseStock**
> WarehouseStock updateWarehouseStock(warehouseId, productId, stockAdjustment)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseStockApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val stockAdjustment : StockAdjustment =  // StockAdjustment | 
try {
    val result : WarehouseStock = apiInstance.updateWarehouseStock(warehouseId, productId, stockAdjustment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseStockApi#updateWarehouseStock")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseStockApi#updateWarehouseStock")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |
| **productId** | **java.util.UUID**|  | |
| **stockAdjustment** | [**StockAdjustment**](StockAdjustment.md)|  | |

### Return type

[**WarehouseStock**](WarehouseStock.md)

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

