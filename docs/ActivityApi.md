# ActivityApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createActivity**](ActivityApi.md#createActivity) | **POST** /api/v1/activities |  |
| [**deleteActivity**](ActivityApi.md#deleteActivity) | **DELETE** /api/v1/activities/{activity_id} |  |
| [**getActivity**](ActivityApi.md#getActivity) | **GET** /api/v1/activities/{activity_id} |  |
| [**listActivities**](ActivityApi.md#listActivities) | **GET** /api/v1/activities/ |  |
| [**updateActivity**](ActivityApi.md#updateActivity) | **PUT** /api/v1/activities/{activity_id} |  |
| [**updateActivityStatus**](ActivityApi.md#updateActivityStatus) | **PUT** /api/v1/activities/{activity_id}/status |  |


<a id="createActivity"></a>
# **createActivity**
> Activity createActivity(activity)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivityApi()
val activity : Activity =  // Activity | 
try {
    val result : Activity = apiInstance.createActivity(activity)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityApi#createActivity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityApi#createActivity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **activity** | [**Activity**](Activity.md)|  | |

### Return type

[**Activity**](Activity.md)

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

<a id="deleteActivity"></a>
# **deleteActivity**
> deleteActivity(activityId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivityApi()
val activityId : kotlin.String = activityId_example // kotlin.String | 
try {
    apiInstance.deleteActivity(activityId)
} catch (e: ClientException) {
    println("4xx response calling ActivityApi#deleteActivity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityApi#deleteActivity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **activityId** | **kotlin.String**|  | |

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

<a id="getActivity"></a>
# **getActivity**
> Activity getActivity(activityId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivityApi()
val activityId : kotlin.String = activityId_example // kotlin.String | 
try {
    val result : Activity = apiInstance.getActivity(activityId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityApi#getActivity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityApi#getActivity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **activityId** | **kotlin.String**|  | |

### Return type

[**Activity**](Activity.md)

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

<a id="listActivities"></a>
# **listActivities**
> kotlin.collections.List&lt;Activity&gt; listActivities(page, pageSize, contactId, activityType, status, assignedTo, overdueOnly)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivityApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val contactId : kotlin.String = contactId_example // kotlin.String | 
val activityType : kotlin.String = activityType_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
val assignedTo : kotlin.String = assignedTo_example // kotlin.String | 
val overdueOnly : kotlin.Boolean = true // kotlin.Boolean | Only show overdue follow-ups.
try {
    val result : kotlin.collections.List<Activity> = apiInstance.listActivities(page, pageSize, contactId, activityType, status, assignedTo, overdueOnly)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityApi#listActivities")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityApi#listActivities")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **contactId** | **kotlin.String**|  | [optional] |
| **activityType** | **kotlin.String**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **assignedTo** | **kotlin.String**|  | [optional] |
| **overdueOnly** | **kotlin.Boolean**| Only show overdue follow-ups. | [optional] |

### Return type

[**kotlin.collections.List&lt;Activity&gt;**](Activity.md)

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

<a id="updateActivity"></a>
# **updateActivity**
> Activity updateActivity(activityId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivityApi()
val activityId : kotlin.String = activityId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Activity = apiInstance.updateActivity(activityId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityApi#updateActivity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityApi#updateActivity")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **activityId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Activity**](Activity.md)

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

<a id="updateActivityStatus"></a>
# **updateActivityStatus**
> Activity updateActivityStatus(activityId, activityStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ActivityApi()
val activityId : kotlin.String = activityId_example // kotlin.String | 
val activityStatusUpdate : ActivityStatusUpdate =  // ActivityStatusUpdate | 
try {
    val result : Activity = apiInstance.updateActivityStatus(activityId, activityStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ActivityApi#updateActivityStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ActivityApi#updateActivityStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **activityId** | **kotlin.String**|  | |
| **activityStatusUpdate** | [**ActivityStatusUpdate**](ActivityStatusUpdate.md)|  | |

### Return type

[**Activity**](Activity.md)

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

