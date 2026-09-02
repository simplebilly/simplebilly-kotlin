# ProductCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProductCategory**](ProductCategoryApi.md#createProductCategory) | **POST** /api/v1/product-categories |  |
| [**deleteProductCategory**](ProductCategoryApi.md#deleteProductCategory) | **DELETE** /api/v1/product-categories/{category_id} |  |
| [**getProductCategory**](ProductCategoryApi.md#getProductCategory) | **GET** /api/v1/product-categories/{category_id} |  |
| [**listProductCategories**](ProductCategoryApi.md#listProductCategories) | **GET** /api/v1/product-categories |  |
| [**updateProductCategory**](ProductCategoryApi.md#updateProductCategory) | **PUT** /api/v1/product-categories/{category_id} |  |


<a id="createProductCategory"></a>
# **createProductCategory**
> ProductCategory createProductCategory(productCategory)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductCategoryApi()
val productCategory : ProductCategory =  // ProductCategory | 
try {
    val result : ProductCategory = apiInstance.createProductCategory(productCategory)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductCategoryApi#createProductCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductCategoryApi#createProductCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productCategory** | [**ProductCategory**](ProductCategory.md)|  | |

### Return type

[**ProductCategory**](ProductCategory.md)

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

<a id="deleteProductCategory"></a>
# **deleteProductCategory**
> deleteProductCategory(categoryId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductCategoryApi()
val categoryId : kotlin.String = categoryId_example // kotlin.String | 
try {
    apiInstance.deleteProductCategory(categoryId)
} catch (e: ClientException) {
    println("4xx response calling ProductCategoryApi#deleteProductCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductCategoryApi#deleteProductCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **categoryId** | **kotlin.String**|  | |

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

<a id="getProductCategory"></a>
# **getProductCategory**
> ProductCategory getProductCategory(categoryId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductCategoryApi()
val categoryId : kotlin.String = categoryId_example // kotlin.String | 
try {
    val result : ProductCategory = apiInstance.getProductCategory(categoryId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductCategoryApi#getProductCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductCategoryApi#getProductCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **categoryId** | **kotlin.String**|  | |

### Return type

[**ProductCategory**](ProductCategory.md)

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

<a id="listProductCategories"></a>
# **listProductCategories**
> kotlin.collections.List&lt;ProductCategory&gt; listProductCategories()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductCategoryApi()
try {
    val result : kotlin.collections.List<ProductCategory> = apiInstance.listProductCategories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductCategoryApi#listProductCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductCategoryApi#listProductCategories")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ProductCategory&gt;**](ProductCategory.md)

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

<a id="updateProductCategory"></a>
# **updateProductCategory**
> ProductCategory updateProductCategory(categoryId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductCategoryApi()
val categoryId : kotlin.String = categoryId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : ProductCategory = apiInstance.updateProductCategory(categoryId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductCategoryApi#updateProductCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductCategoryApi#updateProductCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **categoryId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**ProductCategory**](ProductCategory.md)

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

