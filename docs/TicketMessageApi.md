# TicketMessageApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listMessagesApi**](TicketMessageApi.md#listMessagesApi) | **GET** /api/v1/support/tickets/{ticket_id}/messages |  |
| [**sendMessageApi**](TicketMessageApi.md#sendMessageApi) | **POST** /api/v1/support/tickets/{ticket_id}/messages |  |


<a id="listMessagesApi"></a>
# **listMessagesApi**
> kotlin.collections.List&lt;TicketMessage&gt; listMessagesApi(ticketId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TicketMessageApi()
val ticketId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.collections.List<TicketMessage> = apiInstance.listMessagesApi(ticketId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TicketMessageApi#listMessagesApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TicketMessageApi#listMessagesApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ticketId** | **java.util.UUID**|  | |

### Return type

[**kotlin.collections.List&lt;TicketMessage&gt;**](TicketMessage.md)

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

<a id="sendMessageApi"></a>
# **sendMessageApi**
> TicketMessage sendMessageApi(ticketId, sendMessageDto)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TicketMessageApi()
val ticketId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val sendMessageDto : SendMessageDto =  // SendMessageDto | 
try {
    val result : TicketMessage = apiInstance.sendMessageApi(ticketId, sendMessageDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TicketMessageApi#sendMessageApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TicketMessageApi#sendMessageApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **ticketId** | **java.util.UUID**|  | |
| **sendMessageDto** | [**SendMessageDto**](SendMessageDto.md)|  | |

### Return type

[**TicketMessage**](TicketMessage.md)

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

