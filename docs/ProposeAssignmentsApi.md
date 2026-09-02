# ProposeAssignmentsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**proposeAssignmentsApi**](ProposeAssignmentsApi.md#proposeAssignmentsApi) | **GET** /api/v1/bookkeeping/propose-assignments |  |


<a id="proposeAssignmentsApi"></a>
# **proposeAssignmentsApi**
> kotlin.collections.List&lt;ProposedAssignment&gt; proposeAssignmentsApi(minConfidence, customerId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ProposeAssignmentsApi()
val minConfidence : kotlin.Double = 1.2 // kotlin.Double | 
val customerId : kotlin.String = customerId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<ProposedAssignment> = apiInstance.proposeAssignmentsApi(minConfidence, customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ProposeAssignmentsApi#proposeAssignmentsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ProposeAssignmentsApi#proposeAssignmentsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **minConfidence** | **kotlin.Double**|  | [optional] |
| **customerId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;ProposedAssignment&gt;**](ProposedAssignment.md)

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

