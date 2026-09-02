# EventSubscriptionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createEventSubscription**](EventSubscriptionApi.md#createEventSubscription) | **POST** /api/v1/event-subscriptions |  |
| [**deleteEventSubscription**](EventSubscriptionApi.md#deleteEventSubscription) | **DELETE** /api/v1/event-subscriptions/{subscription_id} |  |
| [**listEventSubscriptions**](EventSubscriptionApi.md#listEventSubscriptions) | **GET** /api/v1/event-subscriptions/ |  |


<a id="createEventSubscription"></a>
# **createEventSubscription**
> EventSubscription createEventSubscription(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EventSubscriptionApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : EventSubscription = apiInstance.createEventSubscription(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventSubscriptionApi#createEventSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventSubscriptionApi#createEventSubscription")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**EventSubscription**](EventSubscription.md)

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

<a id="deleteEventSubscription"></a>
# **deleteEventSubscription**
> deleteEventSubscription(subscriptionId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EventSubscriptionApi()
val subscriptionId : kotlin.String = subscriptionId_example // kotlin.String | 
try {
    apiInstance.deleteEventSubscription(subscriptionId)
} catch (e: ClientException) {
    println("4xx response calling EventSubscriptionApi#deleteEventSubscription")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventSubscriptionApi#deleteEventSubscription")
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
 - **Accept**: application/json

<a id="listEventSubscriptions"></a>
# **listEventSubscriptions**
> kotlin.collections.List&lt;EventSubscription&gt; listEventSubscriptions()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EventSubscriptionApi()
try {
    val result : kotlin.collections.List<EventSubscription> = apiInstance.listEventSubscriptions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EventSubscriptionApi#listEventSubscriptions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EventSubscriptionApi#listEventSubscriptions")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;EventSubscription&gt;**](EventSubscription.md)

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

