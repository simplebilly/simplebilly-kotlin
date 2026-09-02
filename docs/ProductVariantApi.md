# ProductVariantApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createProductVariant**](ProductVariantApi.md#createProductVariant) | **POST** /api/v1/product-variants |  |
| [**deleteProductVariant**](ProductVariantApi.md#deleteProductVariant) | **DELETE** /api/v1/product-variants/{variant_id} |  |
| [**generateProductVariants**](ProductVariantApi.md#generateProductVariants) | **POST** /api/v1/product-variants/generate |  |
| [**getProductVariant**](ProductVariantApi.md#getProductVariant) | **GET** /api/v1/product-variants/{variant_id} |  |
| [**listProductVariants**](ProductVariantApi.md#listProductVariants) | **GET** /api/v1/product-variants/ |  |
| [**updateProductVariant**](ProductVariantApi.md#updateProductVariant) | **PUT** /api/v1/product-variants/{variant_id} |  |


<a id="createProductVariant"></a>
# **createProductVariant**
> ProductVariant createProductVariant(productVariant)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductVariantApi()
val productVariant : ProductVariant =  // ProductVariant | 
try {
    val result : ProductVariant = apiInstance.createProductVariant(productVariant)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductVariantApi#createProductVariant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductVariantApi#createProductVariant")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productVariant** | [**ProductVariant**](ProductVariant.md)|  | |

### Return type

[**ProductVariant**](ProductVariant.md)

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

<a id="deleteProductVariant"></a>
# **deleteProductVariant**
> deleteProductVariant(variantId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductVariantApi()
val variantId : kotlin.String = variantId_example // kotlin.String | 
try {
    apiInstance.deleteProductVariant(variantId)
} catch (e: ClientException) {
    println("4xx response calling ProductVariantApi#deleteProductVariant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductVariantApi#deleteProductVariant")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **variantId** | **kotlin.String**|  | |

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

<a id="generateProductVariants"></a>
# **generateProductVariants**
> kotlin.collections.List&lt;ProductVariant&gt; generateProductVariants(generateVariantsRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductVariantApi()
val generateVariantsRequest : GenerateVariantsRequest =  // GenerateVariantsRequest | 
try {
    val result : kotlin.collections.List<ProductVariant> = apiInstance.generateProductVariants(generateVariantsRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductVariantApi#generateProductVariants")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductVariantApi#generateProductVariants")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **generateVariantsRequest** | [**GenerateVariantsRequest**](GenerateVariantsRequest.md)|  | |

### Return type

[**kotlin.collections.List&lt;ProductVariant&gt;**](ProductVariant.md)

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

<a id="getProductVariant"></a>
# **getProductVariant**
> ProductVariant getProductVariant(variantId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductVariantApi()
val variantId : kotlin.String = variantId_example // kotlin.String | 
try {
    val result : ProductVariant = apiInstance.getProductVariant(variantId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductVariantApi#getProductVariant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductVariantApi#getProductVariant")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **variantId** | **kotlin.String**|  | |

### Return type

[**ProductVariant**](ProductVariant.md)

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

<a id="listProductVariants"></a>
# **listProductVariants**
> kotlin.collections.List&lt;ProductVariant&gt; listProductVariants(page, pageSize, productId, isActive)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductVariantApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val isActive : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.collections.List<ProductVariant> = apiInstance.listProductVariants(page, pageSize, productId, isActive)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductVariantApi#listProductVariants")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductVariantApi#listProductVariants")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **productId** | **java.util.UUID**|  | [optional] |
| **isActive** | **kotlin.Boolean**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ProductVariant&gt;**](ProductVariant.md)

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

<a id="updateProductVariant"></a>
# **updateProductVariant**
> ProductVariant updateProductVariant(variantId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProductVariantApi()
val variantId : kotlin.String = variantId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : ProductVariant = apiInstance.updateProductVariant(variantId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProductVariantApi#updateProductVariant")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProductVariantApi#updateProductVariant")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **variantId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**ProductVariant**](ProductVariant.md)

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

