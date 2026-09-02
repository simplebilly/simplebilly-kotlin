# ComplianceTrainingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createComplianceTraining**](ComplianceTrainingApi.md#createComplianceTraining) | **POST** /api/v1/compliance-trainings |  |
| [**deleteComplianceTraining**](ComplianceTrainingApi.md#deleteComplianceTraining) | **DELETE** /api/v1/compliance-trainings/{id} |  |
| [**getComplianceTraining**](ComplianceTrainingApi.md#getComplianceTraining) | **GET** /api/v1/compliance-trainings/{id} |  |
| [**getComplianceTrainings**](ComplianceTrainingApi.md#getComplianceTrainings) | **GET** /api/v1/compliance-trainings/ |  |
| [**updateComplianceTraining**](ComplianceTrainingApi.md#updateComplianceTraining) | **PUT** /api/v1/compliance-trainings/{id} |  |


<a id="createComplianceTraining"></a>
# **createComplianceTraining**
> ComplianceTraining createComplianceTraining(complianceTrainingCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ComplianceTrainingApi()
val complianceTrainingCreate : ComplianceTrainingCreate =  // ComplianceTrainingCreate | 
try {
    val result : ComplianceTraining = apiInstance.createComplianceTraining(complianceTrainingCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceTrainingApi#createComplianceTraining")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceTrainingApi#createComplianceTraining")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **complianceTrainingCreate** | [**ComplianceTrainingCreate**](ComplianceTrainingCreate.md)|  | |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

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

<a id="deleteComplianceTraining"></a>
# **deleteComplianceTraining**
> deleteComplianceTraining(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ComplianceTrainingApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteComplianceTraining(id)
} catch (e: ClientException) {
    println("4xx response calling ComplianceTrainingApi#deleteComplianceTraining")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceTrainingApi#deleteComplianceTraining")
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

<a id="getComplianceTraining"></a>
# **getComplianceTraining**
> ComplianceTraining getComplianceTraining(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ComplianceTrainingApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : ComplianceTraining = apiInstance.getComplianceTraining(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceTrainingApi#getComplianceTraining")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceTrainingApi#getComplianceTraining")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

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

<a id="getComplianceTrainings"></a>
# **getComplianceTrainings**
> kotlin.collections.List&lt;ComplianceTraining&gt; getComplianceTrainings(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ComplianceTrainingApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<ComplianceTraining> = apiInstance.getComplianceTrainings(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceTrainingApi#getComplianceTrainings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceTrainingApi#getComplianceTrainings")
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

[**kotlin.collections.List&lt;ComplianceTraining&gt;**](ComplianceTraining.md)

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

<a id="updateComplianceTraining"></a>
# **updateComplianceTraining**
> ComplianceTraining updateComplianceTraining(id, complianceTrainingUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ComplianceTrainingApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val complianceTrainingUpdate : ComplianceTrainingUpdate =  // ComplianceTrainingUpdate | 
try {
    val result : ComplianceTraining = apiInstance.updateComplianceTraining(id, complianceTrainingUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ComplianceTrainingApi#updateComplianceTraining")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ComplianceTrainingApi#updateComplianceTraining")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **complianceTrainingUpdate** | [**ComplianceTrainingUpdate**](ComplianceTrainingUpdate.md)|  | |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

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

