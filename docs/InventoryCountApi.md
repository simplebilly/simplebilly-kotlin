# InventoryCountApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createInventoryCount**](InventoryCountApi.md#createInventoryCount) | **POST** /api/v1/inventory-counts |  |
| [**deleteInventoryCount**](InventoryCountApi.md#deleteInventoryCount) | **DELETE** /api/v1/inventory-counts/{inventory_count_id} |  |
| [**generateInventoryCount**](InventoryCountApi.md#generateInventoryCount) | **POST** /api/v1/inventory-counts/generate |  |
| [**getInventoryCount**](InventoryCountApi.md#getInventoryCount) | **GET** /api/v1/inventory-counts/{inventory_count_id} |  |
| [**listInventoryCounts**](InventoryCountApi.md#listInventoryCounts) | **GET** /api/v1/inventory-counts/ |  |
| [**updateInventoryCount**](InventoryCountApi.md#updateInventoryCount) | **PUT** /api/v1/inventory-counts/{inventory_count_id} |  |
| [**updateInventoryCountStatus**](InventoryCountApi.md#updateInventoryCountStatus) | **PUT** /api/v1/inventory-counts/{inventory_count_id}/status |  |


<a id="createInventoryCount"></a>
# **createInventoryCount**
> InventoryCount createInventoryCount(inventoryCount)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val inventoryCount : InventoryCount =  // InventoryCount | 
try {
    val result : InventoryCount = apiInstance.createInventoryCount(inventoryCount)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#createInventoryCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#createInventoryCount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inventoryCount** | [**InventoryCount**](InventoryCount.md)|  | |

### Return type

[**InventoryCount**](InventoryCount.md)

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

<a id="deleteInventoryCount"></a>
# **deleteInventoryCount**
> deleteInventoryCount(inventoryCountId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val inventoryCountId : kotlin.String = inventoryCountId_example // kotlin.String | 
try {
    apiInstance.deleteInventoryCount(inventoryCountId)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#deleteInventoryCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#deleteInventoryCount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inventoryCountId** | **kotlin.String**|  | |

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

<a id="generateInventoryCount"></a>
# **generateInventoryCount**
> InventoryCount generateInventoryCount(generateCountRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val generateCountRequest : GenerateCountRequest =  // GenerateCountRequest | 
try {
    val result : InventoryCount = apiInstance.generateInventoryCount(generateCountRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#generateInventoryCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#generateInventoryCount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **generateCountRequest** | [**GenerateCountRequest**](GenerateCountRequest.md)|  | |

### Return type

[**InventoryCount**](InventoryCount.md)

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

<a id="getInventoryCount"></a>
# **getInventoryCount**
> InventoryCount getInventoryCount(inventoryCountId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val inventoryCountId : kotlin.String = inventoryCountId_example // kotlin.String | 
try {
    val result : InventoryCount = apiInstance.getInventoryCount(inventoryCountId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#getInventoryCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#getInventoryCount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inventoryCountId** | **kotlin.String**|  | |

### Return type

[**InventoryCount**](InventoryCount.md)

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

<a id="listInventoryCounts"></a>
# **listInventoryCounts**
> kotlin.collections.List&lt;InventoryCount&gt; listInventoryCounts(page, pageSize, status, warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<InventoryCount> = apiInstance.listInventoryCounts(page, pageSize, status, warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#listInventoryCounts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#listInventoryCounts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **warehouseId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;InventoryCount&gt;**](InventoryCount.md)

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

<a id="updateInventoryCount"></a>
# **updateInventoryCount**
> InventoryCount updateInventoryCount(inventoryCountId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val inventoryCountId : kotlin.String = inventoryCountId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : InventoryCount = apiInstance.updateInventoryCount(inventoryCountId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#updateInventoryCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#updateInventoryCount")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inventoryCountId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**InventoryCount**](InventoryCount.md)

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

<a id="updateInventoryCountStatus"></a>
# **updateInventoryCountStatus**
> InventoryCount updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryCountApi()
val inventoryCountId : kotlin.String = inventoryCountId_example // kotlin.String | 
val inventoryCountStatusUpdate : InventoryCountStatusUpdate =  // InventoryCountStatusUpdate | 
try {
    val result : InventoryCount = apiInstance.updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryCountApi#updateInventoryCountStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryCountApi#updateInventoryCountStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inventoryCountId** | **kotlin.String**|  | |
| **inventoryCountStatusUpdate** | [**InventoryCountStatusUpdate**](InventoryCountStatusUpdate.md)|  | |

### Return type

[**InventoryCount**](InventoryCount.md)

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

