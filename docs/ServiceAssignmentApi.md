# ServiceAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createServiceAssignment**](ServiceAssignmentApi.md#createServiceAssignment) | **POST** /api/v1/service-assignments |  |
| [**deleteServiceAssignment**](ServiceAssignmentApi.md#deleteServiceAssignment) | **DELETE** /api/v1/service-assignments/{id} |  |
| [**getServiceAssignment**](ServiceAssignmentApi.md#getServiceAssignment) | **GET** /api/v1/service-assignments/{id} |  |
| [**getServiceAssignments**](ServiceAssignmentApi.md#getServiceAssignments) | **GET** /api/v1/service-assignments/ |  |
| [**updateServiceAssignment**](ServiceAssignmentApi.md#updateServiceAssignment) | **PUT** /api/v1/service-assignments/{id} |  |


<a id="createServiceAssignment"></a>
# **createServiceAssignment**
> ServiceAssignment createServiceAssignment(serviceAssignmentCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceAssignmentApi()
val serviceAssignmentCreate : ServiceAssignmentCreate =  // ServiceAssignmentCreate | 
try {
    val result : ServiceAssignment = apiInstance.createServiceAssignment(serviceAssignmentCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceAssignmentApi#createServiceAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceAssignmentApi#createServiceAssignment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serviceAssignmentCreate** | [**ServiceAssignmentCreate**](ServiceAssignmentCreate.md)|  | |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

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

<a id="deleteServiceAssignment"></a>
# **deleteServiceAssignment**
> deleteServiceAssignment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceAssignmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteServiceAssignment(id)
} catch (e: ClientException) {
    println("4xx response calling ServiceAssignmentApi#deleteServiceAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceAssignmentApi#deleteServiceAssignment")
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

<a id="getServiceAssignment"></a>
# **getServiceAssignment**
> ServiceAssignment getServiceAssignment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceAssignmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : ServiceAssignment = apiInstance.getServiceAssignment(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceAssignmentApi#getServiceAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceAssignmentApi#getServiceAssignment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

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

<a id="getServiceAssignments"></a>
# **getServiceAssignments**
> kotlin.collections.List&lt;ServiceAssignment&gt; getServiceAssignments(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceAssignmentApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<ServiceAssignment> = apiInstance.getServiceAssignments(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceAssignmentApi#getServiceAssignments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceAssignmentApi#getServiceAssignments")
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

[**kotlin.collections.List&lt;ServiceAssignment&gt;**](ServiceAssignment.md)

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

<a id="updateServiceAssignment"></a>
# **updateServiceAssignment**
> ServiceAssignment updateServiceAssignment(id, serviceAssignmentUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceAssignmentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val serviceAssignmentUpdate : ServiceAssignmentUpdate =  // ServiceAssignmentUpdate | 
try {
    val result : ServiceAssignment = apiInstance.updateServiceAssignment(id, serviceAssignmentUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceAssignmentApi#updateServiceAssignment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceAssignmentApi#updateServiceAssignment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **serviceAssignmentUpdate** | [**ServiceAssignmentUpdate**](ServiceAssignmentUpdate.md)|  | |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

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

