# TrainingAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTrainingAssignment**](TrainingAssignmentApi.md#createTrainingAssignment) | **POST** /api/v1/training-assignments |  |
| [**deleteTrainingAssignment**](TrainingAssignmentApi.md#deleteTrainingAssignment) | **DELETE** /api/v1/training-assignments/{id} |  |
| [**getTrainingAssignment**](TrainingAssignmentApi.md#getTrainingAssignment) | **GET** /api/v1/training-assignments/{id} |  |
| [**getTrainingAssignments**](TrainingAssignmentApi.md#getTrainingAssignments) | **GET** /api/v1/training-assignments/ |  |
| [**updateTrainingAssignment**](TrainingAssignmentApi.md#updateTrainingAssignment) | **PUT** /api/v1/training-assignments/{id} |  |


<a id="createTrainingAssignment"></a>
# **createTrainingAssignment**
> TrainingAssignment createTrainingAssignment(trainingAssignmentCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingAssignmentApi()
val trainingAssignmentCreate : TrainingAssignmentCreate =  // TrainingAssignmentCreate | 
try {
    val result : TrainingAssignment = apiInstance.createTrainingAssignment(trainingAssignmentCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingAssignmentApi#createTrainingAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingAssignmentApi#createTrainingAssignment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **trainingAssignmentCreate** | [**TrainingAssignmentCreate**](TrainingAssignmentCreate.md)|  | |

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

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

<a id="deleteTrainingAssignment"></a>
# **deleteTrainingAssignment**
> deleteTrainingAssignment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingAssignmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteTrainingAssignment(id)
} catch (e: ClientException) {
    println("4xx response calling TrainingAssignmentApi#deleteTrainingAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingAssignmentApi#deleteTrainingAssignment")
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
 - **Accept**: application/json

<a id="getTrainingAssignment"></a>
# **getTrainingAssignment**
> TrainingAssignment getTrainingAssignment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingAssignmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : TrainingAssignment = apiInstance.getTrainingAssignment(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingAssignmentApi#getTrainingAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingAssignmentApi#getTrainingAssignment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

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

<a id="getTrainingAssignments"></a>
# **getTrainingAssignments**
> kotlin.collections.List&lt;TrainingAssignment&gt; getTrainingAssignments(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingAssignmentApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<TrainingAssignment> = apiInstance.getTrainingAssignments(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingAssignmentApi#getTrainingAssignments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingAssignmentApi#getTrainingAssignments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;TrainingAssignment&gt;**](TrainingAssignment.md)

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

<a id="updateTrainingAssignment"></a>
# **updateTrainingAssignment**
> TrainingAssignment updateTrainingAssignment(id, trainingAssignmentUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TrainingAssignmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val trainingAssignmentUpdate : TrainingAssignmentUpdate =  // TrainingAssignmentUpdate | 
try {
    val result : TrainingAssignment = apiInstance.updateTrainingAssignment(id, trainingAssignmentUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TrainingAssignmentApi#updateTrainingAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TrainingAssignmentApi#updateTrainingAssignment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **trainingAssignmentUpdate** | [**TrainingAssignmentUpdate**](TrainingAssignmentUpdate.md)|  | |

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

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

