# ShippingThresholdApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createShippingThreshold**](ShippingThresholdApi.md#createShippingThreshold) | **POST** /api/v1/shipping-thresholds |  |
| [**deleteShippingThreshold**](ShippingThresholdApi.md#deleteShippingThreshold) | **DELETE** /api/v1/shipping-thresholds/{threshold_id} |  |
| [**getDeliverable**](ShippingThresholdApi.md#getDeliverable) | **GET** /api/v1/shipping-thresholds/deliverable |  |
| [**getShippingThreshold**](ShippingThresholdApi.md#getShippingThreshold) | **GET** /api/v1/shipping-thresholds/{threshold_id} |  |
| [**listShippingThresholds**](ShippingThresholdApi.md#listShippingThresholds) | **GET** /api/v1/shipping-thresholds/ |  |
| [**updateShippingThreshold**](ShippingThresholdApi.md#updateShippingThreshold) | **PUT** /api/v1/shipping-thresholds/{threshold_id} |  |


<a id="createShippingThreshold"></a>
# **createShippingThreshold**
> ShippingThreshold createShippingThreshold(shippingThresholdCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingThresholdApi()
val shippingThresholdCreate : ShippingThresholdCreate =  // ShippingThresholdCreate | 
try {
    val result : ShippingThreshold = apiInstance.createShippingThreshold(shippingThresholdCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingThresholdApi#createShippingThreshold")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingThresholdApi#createShippingThreshold")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shippingThresholdCreate** | [**ShippingThresholdCreate**](ShippingThresholdCreate.md)|  | |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

<a id="deleteShippingThreshold"></a>
# **deleteShippingThreshold**
> deleteShippingThreshold(thresholdId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingThresholdApi()
val thresholdId : kotlin.String = thresholdId_example // kotlin.String | 
try {
    apiInstance.deleteShippingThreshold(thresholdId)
} catch (e: ClientException) {
    println("4xx response calling ShippingThresholdApi#deleteShippingThreshold")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingThresholdApi#deleteShippingThreshold")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **thresholdId** | **kotlin.String**|  | |

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

<a id="getDeliverable"></a>
# **getDeliverable**
> DeliverableResponse getDeliverable(productId, warehouseId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingThresholdApi()
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
try {
    val result : DeliverableResponse = apiInstance.getDeliverable(productId, warehouseId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingThresholdApi#getDeliverable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingThresholdApi#getDeliverable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **productId** | **java.util.UUID**|  | |
| **warehouseId** | **kotlin.String**|  | [optional] |

### Return type

[**DeliverableResponse**](DeliverableResponse.md)

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

<a id="getShippingThreshold"></a>
# **getShippingThreshold**
> ShippingThreshold getShippingThreshold(thresholdId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingThresholdApi()
val thresholdId : kotlin.String = thresholdId_example // kotlin.String | 
try {
    val result : ShippingThreshold = apiInstance.getShippingThreshold(thresholdId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingThresholdApi#getShippingThreshold")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingThresholdApi#getShippingThreshold")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **thresholdId** | **kotlin.String**|  | |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

<a id="listShippingThresholds"></a>
# **listShippingThresholds**
> kotlin.collections.List&lt;ShippingThreshold&gt; listShippingThresholds(page, pageSize, productId, warehouseId, isActive)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingThresholdApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val isActive : kotlin.Boolean = true // kotlin.Boolean | 
try {
    val result : kotlin.collections.List<ShippingThreshold> = apiInstance.listShippingThresholds(page, pageSize, productId, warehouseId, isActive)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingThresholdApi#listShippingThresholds")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingThresholdApi#listShippingThresholds")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **productId** | **java.util.UUID**|  | [optional] |
| **warehouseId** | **kotlin.String**|  | [optional] |
| **isActive** | **kotlin.Boolean**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ShippingThreshold&gt;**](ShippingThreshold.md)

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

<a id="updateShippingThreshold"></a>
# **updateShippingThreshold**
> ShippingThreshold updateShippingThreshold(thresholdId, shippingThresholdUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingThresholdApi()
val thresholdId : kotlin.String = thresholdId_example // kotlin.String | 
val shippingThresholdUpdate : ShippingThresholdUpdate =  // ShippingThresholdUpdate | 
try {
    val result : ShippingThreshold = apiInstance.updateShippingThreshold(thresholdId, shippingThresholdUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingThresholdApi#updateShippingThreshold")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingThresholdApi#updateShippingThreshold")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **thresholdId** | **kotlin.String**|  | |
| **shippingThresholdUpdate** | [**ShippingThresholdUpdate**](ShippingThresholdUpdate.md)|  | |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

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

