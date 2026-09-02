# ServiceJobApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createServiceJob**](ServiceJobApi.md#createServiceJob) | **POST** /api/v1/service-jobs |  |
| [**deleteServiceJob**](ServiceJobApi.md#deleteServiceJob) | **DELETE** /api/v1/service-jobs/{id} |  |
| [**getServiceJob**](ServiceJobApi.md#getServiceJob) | **GET** /api/v1/service-jobs/{id} |  |
| [**getServiceJobs**](ServiceJobApi.md#getServiceJobs) | **GET** /api/v1/service-jobs/ |  |
| [**updateServiceJob**](ServiceJobApi.md#updateServiceJob) | **PUT** /api/v1/service-jobs/{id} |  |


<a id="createServiceJob"></a>
# **createServiceJob**
> ServiceJob createServiceJob(serviceJobCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceJobApi()
val serviceJobCreate : ServiceJobCreate =  // ServiceJobCreate | 
try {
    val result : ServiceJob = apiInstance.createServiceJob(serviceJobCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceJobApi#createServiceJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceJobApi#createServiceJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **serviceJobCreate** | [**ServiceJobCreate**](ServiceJobCreate.md)|  | |

### Return type

[**ServiceJob**](ServiceJob.md)

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

<a id="deleteServiceJob"></a>
# **deleteServiceJob**
> deleteServiceJob(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceJobApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteServiceJob(id)
} catch (e: ClientException) {
    println("4xx response calling ServiceJobApi#deleteServiceJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceJobApi#deleteServiceJob")
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

<a id="getServiceJob"></a>
# **getServiceJob**
> ServiceJob getServiceJob(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceJobApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : ServiceJob = apiInstance.getServiceJob(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceJobApi#getServiceJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceJobApi#getServiceJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**ServiceJob**](ServiceJob.md)

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

<a id="getServiceJobs"></a>
# **getServiceJobs**
> kotlin.collections.List&lt;ServiceJob&gt; getServiceJobs(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceJobApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<ServiceJob> = apiInstance.getServiceJobs(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceJobApi#getServiceJobs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceJobApi#getServiceJobs")
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

[**kotlin.collections.List&lt;ServiceJob&gt;**](ServiceJob.md)

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

<a id="updateServiceJob"></a>
# **updateServiceJob**
> ServiceJob updateServiceJob(id, serviceJobUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ServiceJobApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val serviceJobUpdate : ServiceJobUpdate =  // ServiceJobUpdate | 
try {
    val result : ServiceJob = apiInstance.updateServiceJob(id, serviceJobUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ServiceJobApi#updateServiceJob")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ServiceJobApi#updateServiceJob")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **serviceJobUpdate** | [**ServiceJobUpdate**](ServiceJobUpdate.md)|  | |

### Return type

[**ServiceJob**](ServiceJob.md)

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

