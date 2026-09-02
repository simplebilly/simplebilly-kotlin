# ShippingRuleApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createShippingRule**](ShippingRuleApi.md#createShippingRule) | **POST** /api/v1/shipping-rules |  |
| [**deleteShippingRule**](ShippingRuleApi.md#deleteShippingRule) | **DELETE** /api/v1/shipping-rules/{rule_id} |  |
| [**getShippingRule**](ShippingRuleApi.md#getShippingRule) | **GET** /api/v1/shipping-rules/{rule_id} |  |
| [**listShippingRules**](ShippingRuleApi.md#listShippingRules) | **GET** /api/v1/shipping-rules/ |  |
| [**updateShippingRule**](ShippingRuleApi.md#updateShippingRule) | **PUT** /api/v1/shipping-rules/{rule_id} |  |


<a id="createShippingRule"></a>
# **createShippingRule**
> ShippingRule createShippingRule(shippingRuleCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingRuleApi()
val shippingRuleCreate : ShippingRuleCreate =  // ShippingRuleCreate | 
try {
    val result : ShippingRule = apiInstance.createShippingRule(shippingRuleCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingRuleApi#createShippingRule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingRuleApi#createShippingRule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shippingRuleCreate** | [**ShippingRuleCreate**](ShippingRuleCreate.md)|  | |

### Return type

[**ShippingRule**](ShippingRule.md)

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

<a id="deleteShippingRule"></a>
# **deleteShippingRule**
> deleteShippingRule(ruleId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingRuleApi()
val ruleId : kotlin.String = ruleId_example // kotlin.String | 
try {
    apiInstance.deleteShippingRule(ruleId)
} catch (e: ClientException) {
    println("4xx response calling ShippingRuleApi#deleteShippingRule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingRuleApi#deleteShippingRule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ruleId** | **kotlin.String**|  | |

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

<a id="getShippingRule"></a>
# **getShippingRule**
> ShippingRule getShippingRule(ruleId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingRuleApi()
val ruleId : kotlin.String = ruleId_example // kotlin.String | 
try {
    val result : ShippingRule = apiInstance.getShippingRule(ruleId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingRuleApi#getShippingRule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingRuleApi#getShippingRule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ruleId** | **kotlin.String**|  | |

### Return type

[**ShippingRule**](ShippingRule.md)

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

<a id="listShippingRules"></a>
# **listShippingRules**
> kotlin.collections.List&lt;ShippingRule&gt; listShippingRules(page, pageSize, country)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingRuleApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val country : kotlin.String = country_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ShippingRule> = apiInstance.listShippingRules(page, pageSize, country)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingRuleApi#listShippingRules")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingRuleApi#listShippingRules")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **country** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ShippingRule&gt;**](ShippingRule.md)

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

<a id="updateShippingRule"></a>
# **updateShippingRule**
> ShippingRule updateShippingRule(ruleId, shippingRuleUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingRuleApi()
val ruleId : kotlin.String = ruleId_example // kotlin.String | 
val shippingRuleUpdate : ShippingRuleUpdate =  // ShippingRuleUpdate | 
try {
    val result : ShippingRule = apiInstance.updateShippingRule(ruleId, shippingRuleUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingRuleApi#updateShippingRule")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingRuleApi#updateShippingRule")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ruleId** | **kotlin.String**|  | |
| **shippingRuleUpdate** | [**ShippingRuleUpdate**](ShippingRuleUpdate.md)|  | |

### Return type

[**ShippingRule**](ShippingRule.md)

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

