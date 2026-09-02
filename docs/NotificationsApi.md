# NotificationsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**deleteNotification**](NotificationsApi.md#deleteNotification) | **DELETE** /api/v1/notifications/{id} |  |
| [**listNotifications**](NotificationsApi.md#listNotifications) | **GET** /api/v1/notifications |  |
| [**markAllRead**](NotificationsApi.md#markAllRead) | **PUT** /api/v1/notifications/read-all |  |
| [**markAsRead**](NotificationsApi.md#markAsRead) | **PUT** /api/v1/notifications/{id}/read |  |
| [**unreadCount**](NotificationsApi.md#unreadCount) | **GET** /api/v1/notifications/unread-count |  |


<a id="deleteNotification"></a>
# **deleteNotification**
> deleteNotification(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteNotification(id)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#deleteNotification")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#deleteNotification")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="listNotifications"></a>
# **listNotifications**
> kotlin.collections.List&lt;NotificationDto&gt; listNotifications()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
try {
    val result : kotlin.collections.List<NotificationDto> = apiInstance.listNotifications()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#listNotifications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#listNotifications")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;NotificationDto&gt;**](NotificationDto.md)

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

<a id="markAllRead"></a>
# **markAllRead**
> kotlin.Long markAllRead()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
try {
    val result : kotlin.Long = apiInstance.markAllRead()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#markAllRead")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#markAllRead")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.Long**

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
 - **Accept**: text/plain

<a id="markAsRead"></a>
# **markAsRead**
> markAsRead(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.markAsRead(id)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#markAsRead")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#markAsRead")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

<a id="unreadCount"></a>
# **unreadCount**
> kotlin.Long unreadCount()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = NotificationsApi()
try {
    val result : kotlin.Long = apiInstance.unreadCount()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling NotificationsApi#unreadCount")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling NotificationsApi#unreadCount")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

**kotlin.Long**

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
 - **Accept**: text/plain

