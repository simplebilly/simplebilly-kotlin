# PriceTierApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPriceTier**](PriceTierApi.md#createPriceTier) | **POST** /api/v1/price-tiers |  |
| [**deletePriceTier**](PriceTierApi.md#deletePriceTier) | **DELETE** /api/v1/price-tiers/{price_tier_id} |  |
| [**getPriceTier**](PriceTierApi.md#getPriceTier) | **GET** /api/v1/price-tiers/{price_tier_id} |  |
| [**getResolvedPrice**](PriceTierApi.md#getResolvedPrice) | **GET** /api/v1/price-tiers/resolved |  |
| [**listPriceTiers**](PriceTierApi.md#listPriceTiers) | **GET** /api/v1/price-tiers/ |  |
| [**updatePriceTier**](PriceTierApi.md#updatePriceTier) | **PUT** /api/v1/price-tiers/{price_tier_id} |  |


<a id="createPriceTier"></a>
# **createPriceTier**
> PriceTier createPriceTier(priceTierCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PriceTierApi()
val priceTierCreate : PriceTierCreate =  // PriceTierCreate | 
try {
    val result : PriceTier = apiInstance.createPriceTier(priceTierCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PriceTierApi#createPriceTier")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PriceTierApi#createPriceTier")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **priceTierCreate** | [**PriceTierCreate**](PriceTierCreate.md)|  | |

### Return type

[**PriceTier**](PriceTier.md)

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

<a id="deletePriceTier"></a>
# **deletePriceTier**
> deletePriceTier(priceTierId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PriceTierApi()
val priceTierId : kotlin.String = priceTierId_example // kotlin.String | 
try {
    apiInstance.deletePriceTier(priceTierId)
} catch (e: ClientException) {
    println("4xx response calling PriceTierApi#deletePriceTier")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PriceTierApi#deletePriceTier")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **priceTierId** | **kotlin.String**|  | |

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

<a id="getPriceTier"></a>
# **getPriceTier**
> PriceTier getPriceTier(priceTierId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PriceTierApi()
val priceTierId : kotlin.String = priceTierId_example // kotlin.String | 
try {
    val result : PriceTier = apiInstance.getPriceTier(priceTierId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PriceTierApi#getPriceTier")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PriceTierApi#getPriceTier")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **priceTierId** | **kotlin.String**|  | |

### Return type

[**PriceTier**](PriceTier.md)

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

<a id="getResolvedPrice"></a>
# **getResolvedPrice**
> ResolvedPriceResponse getResolvedPrice(productId, quantity, contactId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PriceTierApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val quantity : kotlin.Long = 789 // kotlin.Long | 
val contactId : kotlin.String = contactId_example // kotlin.String | Contact used to match customer-group-scoped tiers.
try {
    val result : ResolvedPriceResponse = apiInstance.getResolvedPrice(productId, quantity, contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PriceTierApi#getResolvedPrice")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PriceTierApi#getResolvedPrice")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |
| **quantity** | **kotlin.Long**|  | [optional] |
| **contactId** | **kotlin.String**| Contact used to match customer-group-scoped tiers. | [optional] |

### Return type

[**ResolvedPriceResponse**](ResolvedPriceResponse.md)

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

<a id="listPriceTiers"></a>
# **listPriceTiers**
> kotlin.collections.List&lt;PriceTier&gt; listPriceTiers(page, pageSize, productId, customerGroupId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PriceTierApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val customerGroupId : kotlin.String = customerGroupId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PriceTier> = apiInstance.listPriceTiers(page, pageSize, productId, customerGroupId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PriceTierApi#listPriceTiers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PriceTierApi#listPriceTiers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **productId** | **java.util.UUID**|  | [optional] |
| **customerGroupId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;PriceTier&gt;**](PriceTier.md)

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

<a id="updatePriceTier"></a>
# **updatePriceTier**
> PriceTier updatePriceTier(priceTierId, priceTierUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PriceTierApi()
val priceTierId : kotlin.String = priceTierId_example // kotlin.String | 
val priceTierUpdate : PriceTierUpdate =  // PriceTierUpdate | 
try {
    val result : PriceTier = apiInstance.updatePriceTier(priceTierId, priceTierUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PriceTierApi#updatePriceTier")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PriceTierApi#updatePriceTier")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **priceTierId** | **kotlin.String**|  | |
| **priceTierUpdate** | [**PriceTierUpdate**](PriceTierUpdate.md)|  | |

### Return type

[**PriceTier**](PriceTier.md)

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

