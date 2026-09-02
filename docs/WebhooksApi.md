# WebhooksApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createSubscription**](WebhooksApi.md#createSubscription) | **POST** /api/v1/webhook-subscriptions | Create a webhook subscription (outbound hook). |
| [**deleteSubscription**](WebhooksApi.md#deleteSubscription) | **DELETE** /api/v1/webhook-subscriptions/{subscription_id} | Delete a webhook subscription. |
| [**emitApi**](WebhooksApi.md#emitApi) | **POST** /api/v1/webhooks/emit | Manually fire an event against matching hooks (for testing/flows). |
| [**listEvent**](WebhooksApi.md#listEvent) | **GET** /api/v1/webhook-events | List webhook events (inbound + outbound log). |
| [**listSubscriptions**](WebhooksApi.md#listSubscriptions) | **GET** /api/v1/webhook-subscriptions | List webhook subscriptions for the tenant. |
| [**updateSubscription**](WebhooksApi.md#updateSubscription) | **PUT** /api/v1/webhook-subscriptions/{subscription_id} | Update a webhook subscription. |


<a id="createSubscription"></a>
# **createSubscription**
> WebhookSubscription createSubscription(createSubscriptionRequest)

Create a webhook subscription (outbound hook).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebhooksApi()
val createSubscriptionRequest : CreateSubscriptionRequest =  // CreateSubscriptionRequest | 
try {
    val result : WebhookSubscription = apiInstance.createSubscription(createSubscriptionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#createSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#createSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createSubscriptionRequest** | [**CreateSubscriptionRequest**](CreateSubscriptionRequest.md)|  | |

### Return type

[**WebhookSubscription**](WebhookSubscription.md)

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

<a id="deleteSubscription"></a>
# **deleteSubscription**
> deleteSubscription(subscriptionId)

Delete a webhook subscription.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebhooksApi()
val subscriptionId : kotlin.String = subscriptionId_example // kotlin.String | 
try {
    apiInstance.deleteSubscription(subscriptionId)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#deleteSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#deleteSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subscriptionId** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="emitApi"></a>
# **emitApi**
> emitApi(emitEventRequest)

Manually fire an event against matching hooks (for testing/flows).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebhooksApi()
val emitEventRequest : EmitEventRequest =  // EmitEventRequest | 
try {
    apiInstance.emitApi(emitEventRequest)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#emitApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#emitApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **emitEventRequest** | [**EmitEventRequest**](EmitEventRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="listEvent"></a>
# **listEvent**
> kotlin.collections.List&lt;WebhookEvent&gt; listEvent()

List webhook events (inbound + outbound log).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebhooksApi()
try {
    val result : kotlin.collections.List<WebhookEvent> = apiInstance.listEvent()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#listEvent")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#listEvent")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;WebhookEvent&gt;**](WebhookEvent.md)

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

<a id="listSubscriptions"></a>
# **listSubscriptions**
> kotlin.collections.List&lt;WebhookSubscription&gt; listSubscriptions()

List webhook subscriptions for the tenant.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebhooksApi()
try {
    val result : kotlin.collections.List<WebhookSubscription> = apiInstance.listSubscriptions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#listSubscriptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#listSubscriptions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;WebhookSubscription&gt;**](WebhookSubscription.md)

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

<a id="updateSubscription"></a>
# **updateSubscription**
> WebhookSubscription updateSubscription(subscriptionId, updateSubscriptionRequest)

Update a webhook subscription.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WebhooksApi()
val subscriptionId : kotlin.String = subscriptionId_example // kotlin.String | 
val updateSubscriptionRequest : UpdateSubscriptionRequest =  // UpdateSubscriptionRequest | 
try {
    val result : WebhookSubscription = apiInstance.updateSubscription(subscriptionId, updateSubscriptionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WebhooksApi#updateSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WebhooksApi#updateSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **subscriptionId** | **kotlin.String**|  | |
| **updateSubscriptionRequest** | [**UpdateSubscriptionRequest**](UpdateSubscriptionRequest.md)|  | |

### Return type

[**WebhookSubscription**](WebhookSubscription.md)

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

