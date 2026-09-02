# PaymentGatewayApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPaymentGatewayApi**](PaymentGatewayApi.md#createPaymentGatewayApi) | **POST** /api/v1/payment-gateways |  |
| [**deletePaymentGatewayApi**](PaymentGatewayApi.md#deletePaymentGatewayApi) | **DELETE** /api/v1/payment-gateways/{gateway_id} |  |
| [**listPaymentGatewaysApi**](PaymentGatewayApi.md#listPaymentGatewaysApi) | **GET** /api/v1/payment-gateways/ |  |
| [**oauthAuthorizeApi**](PaymentGatewayApi.md#oauthAuthorizeApi) | **POST** /api/v1/payment-gateways/oauth/authorize |  |
| [**oauthCallbackApi**](PaymentGatewayApi.md#oauthCallbackApi) | **POST** /api/v1/payment-gateways/oauth/callback |  |
| [**updatePaymentGatewayApi**](PaymentGatewayApi.md#updatePaymentGatewayApi) | **PUT** /api/v1/payment-gateways/{gateway_id} |  |


<a id="createPaymentGatewayApi"></a>
# **createPaymentGatewayApi**
> PaymentGateway createPaymentGatewayApi(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentGatewayApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PaymentGateway = apiInstance.createPaymentGatewayApi(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentGatewayApi#createPaymentGatewayApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentGatewayApi#createPaymentGatewayApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**PaymentGateway**](PaymentGateway.md)

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

<a id="deletePaymentGatewayApi"></a>
# **deletePaymentGatewayApi**
> deletePaymentGatewayApi(gatewayId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentGatewayApi()
val gatewayId : kotlin.String = gatewayId_example // kotlin.String | 
try {
    apiInstance.deletePaymentGatewayApi(gatewayId)
} catch (e: ClientException) {
    println("4xx response calling PaymentGatewayApi#deletePaymentGatewayApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentGatewayApi#deletePaymentGatewayApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayId** | **kotlin.String**|  | |

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

<a id="listPaymentGatewaysApi"></a>
# **listPaymentGatewaysApi**
> kotlin.collections.List&lt;PaymentGateway&gt; listPaymentGatewaysApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentGatewayApi()
try {
    val result : kotlin.collections.List<PaymentGateway> = apiInstance.listPaymentGatewaysApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentGatewayApi#listPaymentGatewaysApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentGatewayApi#listPaymentGatewaysApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PaymentGateway&gt;**](PaymentGateway.md)

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

<a id="oauthAuthorizeApi"></a>
# **oauthAuthorizeApi**
> GatewayOAuthAuthorizeResponse oauthAuthorizeApi(gatewayOAuthAuthorizeRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentGatewayApi()
val gatewayOAuthAuthorizeRequest : GatewayOAuthAuthorizeRequest =  // GatewayOAuthAuthorizeRequest | 
try {
    val result : GatewayOAuthAuthorizeResponse = apiInstance.oauthAuthorizeApi(gatewayOAuthAuthorizeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentGatewayApi#oauthAuthorizeApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentGatewayApi#oauthAuthorizeApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayOAuthAuthorizeRequest** | [**GatewayOAuthAuthorizeRequest**](GatewayOAuthAuthorizeRequest.md)|  | |

### Return type

[**GatewayOAuthAuthorizeResponse**](GatewayOAuthAuthorizeResponse.md)

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

<a id="oauthCallbackApi"></a>
# **oauthCallbackApi**
> PaymentGateway oauthCallbackApi(gatewayOAuthCallbackRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentGatewayApi()
val gatewayOAuthCallbackRequest : GatewayOAuthCallbackRequest =  // GatewayOAuthCallbackRequest | 
try {
    val result : PaymentGateway = apiInstance.oauthCallbackApi(gatewayOAuthCallbackRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentGatewayApi#oauthCallbackApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentGatewayApi#oauthCallbackApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayOAuthCallbackRequest** | [**GatewayOAuthCallbackRequest**](GatewayOAuthCallbackRequest.md)|  | |

### Return type

[**PaymentGateway**](PaymentGateway.md)

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

<a id="updatePaymentGatewayApi"></a>
# **updatePaymentGatewayApi**
> PaymentGateway updatePaymentGatewayApi(gatewayId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentGatewayApi()
val gatewayId : kotlin.String = gatewayId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PaymentGateway = apiInstance.updatePaymentGatewayApi(gatewayId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentGatewayApi#updatePaymentGatewayApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentGatewayApi#updatePaymentGatewayApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gatewayId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**PaymentGateway**](PaymentGateway.md)

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

