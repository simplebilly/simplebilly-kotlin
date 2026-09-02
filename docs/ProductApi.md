# ProductApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProductApi**](ProductApi.md#createProductApi) | **POST** /api/v1/products |  |
| [**deleteProductApi**](ProductApi.md#deleteProductApi) | **DELETE** /api/v1/products/{product_id} |  |
| [**getProductApi**](ProductApi.md#getProductApi) | **GET** /api/v1/products/{product_id} |  |
| [**getProductStockApi**](ProductApi.md#getProductStockApi) | **GET** /api/v1/products/{product_id}/stock |  |
| [**getProductsApi**](ProductApi.md#getProductsApi) | **GET** /api/v1/products/ |  |
| [**listLowStockProductsApi**](ProductApi.md#listLowStockProductsApi) | **GET** /api/v1/products/low-stock |  |
| [**productRestore**](ProductApi.md#productRestore) | **POST** /api/v1/products/{product_id}/restore |  |
| [**updateProductApi**](ProductApi.md#updateProductApi) | **PUT** /api/v1/products/{product_id} |  |
| [**updateProductStockApi**](ProductApi.md#updateProductStockApi) | **PUT** /api/v1/products/{product_id}/stock |  |


<a id="createProductApi"></a>
# **createProductApi**
> Product createProductApi(productCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productCreate : ProductCreate =  // ProductCreate | 
try {
    val result : Product = apiInstance.createProductApi(productCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#createProductApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#createProductApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productCreate** | [**ProductCreate**](ProductCreate.md)|  | |

### Return type

[**Product**](Product.md)

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

<a id="deleteProductApi"></a>
# **deleteProductApi**
> deleteProductApi(productId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteProductApi(productId)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#deleteProductApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#deleteProductApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
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

<a id="getProductApi"></a>
# **getProductApi**
> Product getProductApi(productId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Product = apiInstance.getProductApi(productId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#getProductApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#getProductApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |

### Return type

[**Product**](Product.md)

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

<a id="getProductStockApi"></a>
# **getProductStockApi**
> ProductStock getProductStockApi(productId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : ProductStock = apiInstance.getProductStockApi(productId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#getProductStockApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#getProductStockApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |

### Return type

[**ProductStock**](ProductStock.md)

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

<a id="getProductsApi"></a>
# **getProductsApi**
> kotlin.collections.List&lt;Product&gt; getProductsApi(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Product> = apiInstance.getProductsApi(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#getProductsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#getProductsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;Product&gt;**](Product.md)

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

<a id="listLowStockProductsApi"></a>
# **listLowStockProductsApi**
> kotlin.collections.List&lt;ProductStock&gt; listLowStockProductsApi(threshold)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val threshold : kotlin.Long = 789 // kotlin.Long | 
try {
    val result : kotlin.collections.List<ProductStock> = apiInstance.listLowStockProductsApi(threshold)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#listLowStockProductsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#listLowStockProductsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **threshold** | **kotlin.Long**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ProductStock&gt;**](ProductStock.md)

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

<a id="productRestore"></a>
# **productRestore**
> Product productRestore(productId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Product = apiInstance.productRestore(productId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#productRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#productRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |

### Return type

[**Product**](Product.md)

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

<a id="updateProductApi"></a>
# **updateProductApi**
> Product updateProductApi(productId, productUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val productUpdate : ProductUpdate =  // ProductUpdate | 
try {
    val result : Product = apiInstance.updateProductApi(productId, productUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#updateProductApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#updateProductApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |
| **productUpdate** | [**ProductUpdate**](ProductUpdate.md)|  | |

### Return type

[**Product**](Product.md)

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

<a id="updateProductStockApi"></a>
# **updateProductStockApi**
> ProductStock updateProductStockApi(productId, stockUpdateRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val stockUpdateRequest : StockUpdateRequest =  // StockUpdateRequest | 
try {
    val result : ProductStock = apiInstance.updateProductStockApi(productId, stockUpdateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductApi#updateProductStockApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductApi#updateProductStockApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |
| **stockUpdateRequest** | [**StockUpdateRequest**](StockUpdateRequest.md)|  | |

### Return type

[**ProductStock**](ProductStock.md)

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

