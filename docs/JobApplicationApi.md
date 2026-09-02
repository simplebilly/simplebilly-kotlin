# JobApplicationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**applyPublic**](JobApplicationApi.md#applyPublic) | **POST** /api/v1/public/jobs/{posting_id}/apply |  |
| [**deleteJobApplication**](JobApplicationApi.md#deleteJobApplication) | **DELETE** /api/v1/job-applications/{application_id} |  |
| [**downloadCv**](JobApplicationApi.md#downloadCv) | **GET** /api/v1/job-applications/{application_id}/cv |  |
| [**getJobApplication**](JobApplicationApi.md#getJobApplication) | **GET** /api/v1/job-applications/{application_id} |  |
| [**inboundEmail**](JobApplicationApi.md#inboundEmail) | **POST** /api/v1/public/jobs/inbound-email | Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox. |
| [**listJobApplications**](JobApplicationApi.md#listJobApplications) | **GET** /api/v1/job-applications |  |
| [**listPublicPostings**](JobApplicationApi.md#listPublicPostings) | **GET** /api/v1/public/jobs |  |
| [**scoreJobApplication**](JobApplicationApi.md#scoreJobApplication) | **POST** /api/v1/job-applications/{application_id}/score |  |
| [**updateJobApplicationStatus**](JobApplicationApi.md#updateJobApplicationStatus) | **PATCH** /api/v1/job-applications/{application_id}/status |  |


<a id="applyPublic"></a>
# **applyPublic**
> applyPublic(postingId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val postingId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.applyPublic(postingId)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#applyPublic")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#applyPublic")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **postingId** | **java.util.UUID**|  | |

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

<a id="deleteJobApplication"></a>
# **deleteJobApplication**
> JobApplication deleteJobApplication(applicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val applicationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : JobApplication = apiInstance.deleteJobApplication(applicationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#deleteJobApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#deleteJobApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **applicationId** | **java.util.UUID**|  | |

### Return type

[**JobApplication**](JobApplication.md)

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

<a id="downloadCv"></a>
# **downloadCv**
> downloadCv(applicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val applicationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.downloadCv(applicationId)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#downloadCv")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#downloadCv")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **applicationId** | **java.util.UUID**|  | |

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

<a id="getJobApplication"></a>
# **getJobApplication**
> JobApplication getJobApplication(applicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val applicationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : JobApplication = apiInstance.getJobApplication(applicationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#getJobApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#getJobApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **applicationId** | **java.util.UUID**|  | |

### Return type

[**JobApplication**](JobApplication.md)

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

<a id="inboundEmail"></a>
# **inboundEmail**
> inboundEmail()

Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
try {
    apiInstance.inboundEmail()
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#inboundEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#inboundEmail")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="listJobApplications"></a>
# **listJobApplications**
> kotlin.collections.List&lt;JobApplication&gt; listJobApplications(postingId, status, page, pageSize)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val postingId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val status : kotlin.String = status_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<JobApplication> = apiInstance.listJobApplications(postingId, status, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#listJobApplications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#listJobApplications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **postingId** | **java.util.UUID**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;JobApplication&gt;**](JobApplication.md)

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

<a id="listPublicPostings"></a>
# **listPublicPostings**
> kotlin.collections.List&lt;PublicPosting&gt; listPublicPostings()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
try {
    val result : kotlin.collections.List<PublicPosting> = apiInstance.listPublicPostings()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#listPublicPostings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#listPublicPostings")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PublicPosting&gt;**](PublicPosting.md)

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

<a id="scoreJobApplication"></a>
# **scoreJobApplication**
> JobApplication scoreJobApplication(applicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val applicationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : JobApplication = apiInstance.scoreJobApplication(applicationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#scoreJobApplication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#scoreJobApplication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **applicationId** | **java.util.UUID**|  | |

### Return type

[**JobApplication**](JobApplication.md)

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

<a id="updateJobApplicationStatus"></a>
# **updateJobApplicationStatus**
> JobApplication updateJobApplicationStatus(applicationId, applicationStatusDto)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = JobApplicationApi()
val applicationId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val applicationStatusDto : ApplicationStatusDto =  // ApplicationStatusDto | 
try {
    val result : JobApplication = apiInstance.updateJobApplicationStatus(applicationId, applicationStatusDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling JobApplicationApi#updateJobApplicationStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling JobApplicationApi#updateJobApplicationStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **applicationId** | **java.util.UUID**|  | |
| **applicationStatusDto** | [**ApplicationStatusDto**](ApplicationStatusDto.md)|  | |

### Return type

[**JobApplication**](JobApplication.md)

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

