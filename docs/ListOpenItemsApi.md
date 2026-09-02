# ListOpenItemsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listOpenItemsApi**](ListOpenItemsApi.md#listOpenItemsApi) | **GET** /api/v1/bookkeeping/open-items |  |


<a id="listOpenItemsApi"></a>
# **listOpenItemsApi**
> kotlin.collections.List&lt;OpenItem&gt; listOpenItemsApi(reminderLevel1Days, reminderLevel2Days, reminderLevel3Days, customerId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ListOpenItemsApi()
val reminderLevel1Days : kotlin.Long = 789 // kotlin.Long | 
val reminderLevel2Days : kotlin.Long = 789 // kotlin.Long | 
val reminderLevel3Days : kotlin.Long = 789 // kotlin.Long | 
val customerId : kotlin.String = customerId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<OpenItem> = apiInstance.listOpenItemsApi(reminderLevel1Days, reminderLevel2Days, reminderLevel3Days, customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ListOpenItemsApi#listOpenItemsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ListOpenItemsApi#listOpenItemsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **reminderLevel1Days** | **kotlin.Long**|  | [optional] |
| **reminderLevel2Days** | **kotlin.Long**|  | [optional] |
| **reminderLevel3Days** | **kotlin.Long**|  | [optional] |
| **customerId** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;OpenItem&gt;**](OpenItem.md)

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

