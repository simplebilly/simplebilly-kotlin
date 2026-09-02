# WorkflowsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listWorkflowsApi**](WorkflowsApi.md#listWorkflowsApi) | **GET** /api/v1/workflows |  |
| [**setWorkflowEnabledApi**](WorkflowsApi.md#setWorkflowEnabledApi) | **PUT** /api/v1/workflows/{workflow_id}/enabled |  |


<a id="listWorkflowsApi"></a>
# **listWorkflowsApi**
> kotlin.collections.List&lt;Workflow&gt; listWorkflowsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WorkflowsApi()
try {
    val result : kotlin.collections.List<Workflow> = apiInstance.listWorkflowsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowsApi#listWorkflowsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowsApi#listWorkflowsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;Workflow&gt;**](Workflow.md)

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

<a id="setWorkflowEnabledApi"></a>
# **setWorkflowEnabledApi**
> Workflow setWorkflowEnabledApi(workflowId, workflowEnabledUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = WorkflowsApi()
val workflowId : kotlin.String = workflowId_example // kotlin.String | 
val workflowEnabledUpdate : WorkflowEnabledUpdate =  // WorkflowEnabledUpdate | 
try {
    val result : Workflow = apiInstance.setWorkflowEnabledApi(workflowId, workflowEnabledUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling WorkflowsApi#setWorkflowEnabledApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling WorkflowsApi#setWorkflowEnabledApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **workflowId** | **kotlin.String**|  | |
| **workflowEnabledUpdate** | [**WorkflowEnabledUpdate**](WorkflowEnabledUpdate.md)|  | |

### Return type

[**Workflow**](Workflow.md)

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

