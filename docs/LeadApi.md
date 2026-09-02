# LeadApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listLeadsApi**](LeadApi.md#listLeadsApi) | **GET** /api/v1/support/leads |  |
| [**updateLeadApi**](LeadApi.md#updateLeadApi) | **PUT** /api/v1/support/leads/{lead_id} |  |


<a id="listLeadsApi"></a>
# **listLeadsApi**
> kotlin.collections.List&lt;Lead&gt; listLeadsApi(status, source, search, page, pageSize)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LeadApi()
val status : kotlin.String = status_example // kotlin.String | 
val source : kotlin.String = source_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<Lead> = apiInstance.listLeadsApi(status, source, search, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LeadApi#listLeadsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LeadApi#listLeadsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] |
| **source** | **kotlin.String**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Lead&gt;**](Lead.md)

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

<a id="updateLeadApi"></a>
# **updateLeadApi**
> Lead updateLeadApi(leadId, leadUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = LeadApi()
val leadId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val leadUpdate : LeadUpdate =  // LeadUpdate | 
try {
    val result : Lead = apiInstance.updateLeadApi(leadId, leadUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling LeadApi#updateLeadApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling LeadApi#updateLeadApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **leadId** | **java.util.UUID**|  | |
| **leadUpdate** | [**LeadUpdate**](LeadUpdate.md)|  | |

### Return type

[**Lead**](Lead.md)

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

