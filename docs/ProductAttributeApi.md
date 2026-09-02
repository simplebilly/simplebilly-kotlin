# ProductAttributeApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProductAttribute**](ProductAttributeApi.md#createProductAttribute) | **POST** /api/v1/product-attributes |  |
| [**deleteProductAttribute**](ProductAttributeApi.md#deleteProductAttribute) | **DELETE** /api/v1/product-attributes/{attribute_id} |  |
| [**getProductAttribute**](ProductAttributeApi.md#getProductAttribute) | **GET** /api/v1/product-attributes/{attribute_id} |  |
| [**listProductAttributes**](ProductAttributeApi.md#listProductAttributes) | **GET** /api/v1/product-attributes/ |  |
| [**updateProductAttribute**](ProductAttributeApi.md#updateProductAttribute) | **PUT** /api/v1/product-attributes/{attribute_id} |  |


<a id="createProductAttribute"></a>
# **createProductAttribute**
> ProductAttribute createProductAttribute(productAttributeCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductAttributeApi()
val productAttributeCreate : ProductAttributeCreate =  // ProductAttributeCreate | 
try {
    val result : ProductAttribute = apiInstance.createProductAttribute(productAttributeCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAttributeApi#createProductAttribute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAttributeApi#createProductAttribute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productAttributeCreate** | [**ProductAttributeCreate**](ProductAttributeCreate.md)|  | |

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

<a id="deleteProductAttribute"></a>
# **deleteProductAttribute**
> deleteProductAttribute(attributeId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductAttributeApi()
val attributeId : kotlin.String = attributeId_example // kotlin.String | 
try {
    apiInstance.deleteProductAttribute(attributeId)
} catch (e: ClientException) {
    println("4xx response calling ProductAttributeApi#deleteProductAttribute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAttributeApi#deleteProductAttribute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attributeId** | **kotlin.String**|  | |

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

<a id="getProductAttribute"></a>
# **getProductAttribute**
> ProductAttribute getProductAttribute(attributeId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductAttributeApi()
val attributeId : kotlin.String = attributeId_example // kotlin.String | 
try {
    val result : ProductAttribute = apiInstance.getProductAttribute(attributeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAttributeApi#getProductAttribute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAttributeApi#getProductAttribute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attributeId** | **kotlin.String**|  | |

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

<a id="listProductAttributes"></a>
# **listProductAttributes**
> kotlin.collections.List&lt;ProductAttribute&gt; listProductAttributes(page, pageSize, productId, isFilterable, search)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductAttributeApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val isFilterable : kotlin.Boolean = true // kotlin.Boolean | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ProductAttribute> = apiInstance.listProductAttributes(page, pageSize, productId, isFilterable, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAttributeApi#listProductAttributes")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAttributeApi#listProductAttributes")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **productId** | **java.util.UUID**|  | [optional] |
| **isFilterable** | **kotlin.Boolean**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ProductAttribute&gt;**](ProductAttribute.md)

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

<a id="updateProductAttribute"></a>
# **updateProductAttribute**
> ProductAttribute updateProductAttribute(attributeId, productAttributeUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductAttributeApi()
val attributeId : kotlin.String = attributeId_example // kotlin.String | 
val productAttributeUpdate : ProductAttributeUpdate =  // ProductAttributeUpdate | 
try {
    val result : ProductAttribute = apiInstance.updateProductAttribute(attributeId, productAttributeUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductAttributeApi#updateProductAttribute")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductAttributeApi#updateProductAttribute")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **attributeId** | **kotlin.String**|  | |
| **productAttributeUpdate** | [**ProductAttributeUpdate**](ProductAttributeUpdate.md)|  | |

### Return type

[**ProductAttribute**](ProductAttribute.md)

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

