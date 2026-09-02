# SupportTicketApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTicketApi**](SupportTicketApi.md#createTicketApi) | **POST** /api/v1/support/tickets |  |
| [**deleteTicketApi**](SupportTicketApi.md#deleteTicketApi) | **DELETE** /api/v1/support/tickets/{ticket_id} |  |
| [**getTicketApi**](SupportTicketApi.md#getTicketApi) | **GET** /api/v1/support/tickets/{ticket_id} |  |
| [**listTicketsApi**](SupportTicketApi.md#listTicketsApi) | **GET** /api/v1/support/tickets |  |
| [**updateTicketApi**](SupportTicketApi.md#updateTicketApi) | **PUT** /api/v1/support/tickets/{ticket_id} |  |


<a id="createTicketApi"></a>
# **createTicketApi**
> SupportTicket createTicketApi(createTicketRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportTicketApi()
val createTicketRequest : CreateTicketRequest =  // CreateTicketRequest | 
try {
    val result : SupportTicket = apiInstance.createTicketApi(createTicketRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportTicketApi#createTicketApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportTicketApi#createTicketApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createTicketRequest** | [**CreateTicketRequest**](CreateTicketRequest.md)|  | |

### Return type

[**SupportTicket**](SupportTicket.md)

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

<a id="deleteTicketApi"></a>
# **deleteTicketApi**
> deleteTicketApi(ticketId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportTicketApi()
val ticketId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteTicketApi(ticketId)
} catch (e: ClientException) {
    println("4xx response calling SupportTicketApi#deleteTicketApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportTicketApi#deleteTicketApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ticketId** | **java.util.UUID**|  | |

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

<a id="getTicketApi"></a>
# **getTicketApi**
> SupportTicket getTicketApi(ticketId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportTicketApi()
val ticketId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : SupportTicket = apiInstance.getTicketApi(ticketId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportTicketApi#getTicketApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportTicketApi#getTicketApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ticketId** | **java.util.UUID**|  | |

### Return type

[**SupportTicket**](SupportTicket.md)

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

<a id="listTicketsApi"></a>
# **listTicketsApi**
> kotlin.collections.List&lt;SupportTicket&gt; listTicketsApi(status, priority, assignedTo, channelType, customerId, search, page, pageSize)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportTicketApi()
val status : kotlin.String = status_example // kotlin.String | 
val priority : kotlin.String = priority_example // kotlin.String | 
val assignedTo : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val channelType : kotlin.String = channelType_example // kotlin.String | 
val customerId : kotlin.String = customerId_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<SupportTicket> = apiInstance.listTicketsApi(status, priority, assignedTo, channelType, customerId, search, page, pageSize)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportTicketApi#listTicketsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportTicketApi#listTicketsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**|  | [optional] |
| **priority** | **kotlin.String**|  | [optional] |
| **assignedTo** | **java.util.UUID**|  | [optional] |
| **channelType** | **kotlin.String**|  | [optional] |
| **customerId** | **kotlin.String**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;SupportTicket&gt;**](SupportTicket.md)

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

<a id="updateTicketApi"></a>
# **updateTicketApi**
> SupportTicket updateTicketApi(ticketId, supportTicketUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportTicketApi()
val ticketId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val supportTicketUpdate : SupportTicketUpdate =  // SupportTicketUpdate | 
try {
    val result : SupportTicket = apiInstance.updateTicketApi(ticketId, supportTicketUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportTicketApi#updateTicketApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportTicketApi#updateTicketApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ticketId** | **java.util.UUID**|  | |
| **supportTicketUpdate** | [**SupportTicketUpdate**](SupportTicketUpdate.md)|  | |

### Return type

[**SupportTicket**](SupportTicket.md)

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

