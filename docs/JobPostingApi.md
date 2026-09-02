# JobPostingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createJobPosting**](JobPostingApi.md#createJobPosting) | **POST** /api/v1/job-postings |  |
| [**deleteJobPosting**](JobPostingApi.md#deleteJobPosting) | **DELETE** /api/v1/job-postings/{id} |  |
| [**getJobPosting**](JobPostingApi.md#getJobPosting) | **GET** /api/v1/job-postings/{id} |  |
| [**listJobPostings**](JobPostingApi.md#listJobPostings) | **GET** /api/v1/job-postings |  |
| [**updateJobPosting**](JobPostingApi.md#updateJobPosting) | **PUT** /api/v1/job-postings/{id} |  |


<a id="createJobPosting"></a>
# **createJobPosting**
> JobPosting createJobPosting(jobPostingCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobPostingApi()
val jobPostingCreate : JobPostingCreate =  // JobPostingCreate | 
try {
    val result : JobPosting = apiInstance.createJobPosting(jobPostingCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobPostingApi#createJobPosting")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobPostingApi#createJobPosting")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **jobPostingCreate** | [**JobPostingCreate**](JobPostingCreate.md)|  | |

### Return type

[**JobPosting**](JobPosting.md)

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

<a id="deleteJobPosting"></a>
# **deleteJobPosting**
> deleteJobPosting(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobPostingApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteJobPosting(id)
} catch (e: ClientException) {
    println("4xx response calling JobPostingApi#deleteJobPosting")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobPostingApi#deleteJobPosting")
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

<a id="getJobPosting"></a>
# **getJobPosting**
> JobPosting getJobPosting(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobPostingApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : JobPosting = apiInstance.getJobPosting(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobPostingApi#getJobPosting")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobPostingApi#getJobPosting")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**JobPosting**](JobPosting.md)

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

<a id="listJobPostings"></a>
# **listJobPostings**
> kotlin.collections.List&lt;JobPosting&gt; listJobPostings(status, page, pageSize)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobPostingApi()
val status : kotlin.String = status_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<JobPosting> = apiInstance.listJobPostings(status, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobPostingApi#listJobPostings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobPostingApi#listJobPostings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;JobPosting&gt;**](JobPosting.md)

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

<a id="updateJobPosting"></a>
# **updateJobPosting**
> JobPosting updateJobPosting(id, jobPostingUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobPostingApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val jobPostingUpdate : JobPostingUpdate =  // JobPostingUpdate | 
try {
    val result : JobPosting = apiInstance.updateJobPosting(id, jobPostingUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobPostingApi#updateJobPosting")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobPostingApi#updateJobPosting")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **jobPostingUpdate** | [**JobPostingUpdate**](JobPostingUpdate.md)|  | |

### Return type

[**JobPosting**](JobPosting.md)

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

