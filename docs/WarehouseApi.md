# WarehouseApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createWarehouse**](WarehouseApi.md#createWarehouse) | **POST** /api/v1/warehouses |  |
| [**deleteWarehouse**](WarehouseApi.md#deleteWarehouse) | **DELETE** /api/v1/warehouses/{warehouse_id} |  |
| [**getWarehouse**](WarehouseApi.md#getWarehouse) | **GET** /api/v1/warehouses/{warehouse_id} |  |
| [**listWarehouses**](WarehouseApi.md#listWarehouses) | **GET** /api/v1/warehouses/ |  |
| [**updateWarehouse**](WarehouseApi.md#updateWarehouse) | **PUT** /api/v1/warehouses/{warehouse_id} |  |


<a id="createWarehouse"></a>
# **createWarehouse**
> Warehouse createWarehouse(warehouse)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseApi()
val warehouse : Warehouse =  // Warehouse | 
try {
    val result : Warehouse = apiInstance.createWarehouse(warehouse)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseApi#createWarehouse")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseApi#createWarehouse")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouse** | [**Warehouse**](Warehouse.md)|  | |

### Return type

[**Warehouse**](Warehouse.md)

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

<a id="deleteWarehouse"></a>
# **deleteWarehouse**
> deleteWarehouse(warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    apiInstance.deleteWarehouse(warehouseId)
} catch (e: ClientException) {
    println("4xx response calling WarehouseApi#deleteWarehouse")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseApi#deleteWarehouse")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |

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

<a id="getWarehouse"></a>
# **getWarehouse**
> Warehouse getWarehouse(warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    val result : Warehouse = apiInstance.getWarehouse(warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseApi#getWarehouse")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseApi#getWarehouse")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |

### Return type

[**Warehouse**](Warehouse.md)

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

<a id="listWarehouses"></a>
# **listWarehouses**
> kotlin.collections.List&lt;Warehouse&gt; listWarehouses(page, pageSize, search, isActive)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val isActive : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.collections.List<Warehouse> = apiInstance.listWarehouses(page, pageSize, search, isActive)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseApi#listWarehouses")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseApi#listWarehouses")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **isActive** | **kotlin.Boolean**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Warehouse&gt;**](Warehouse.md)

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

<a id="updateWarehouse"></a>
# **updateWarehouse**
> Warehouse updateWarehouse(warehouseId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WarehouseApi()
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Warehouse = apiInstance.updateWarehouse(warehouseId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WarehouseApi#updateWarehouse")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WarehouseApi#updateWarehouse")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **warehouseId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Warehouse**](Warehouse.md)

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

