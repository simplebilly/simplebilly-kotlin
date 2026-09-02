# CustomerCommunicationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCommunication**](CustomerCommunicationApi.md#createCommunication) | **POST** /api/v1/communications |  |
| [**customercommunicationRestore**](CustomerCommunicationApi.md#customercommunicationRestore) | **POST** /api/v1/communications/{communication_id}/restore |  |
| [**deleteCommunication**](CustomerCommunicationApi.md#deleteCommunication) | **DELETE** /api/v1/communications/{communication_id} |  |
| [**getCommunication**](CustomerCommunicationApi.md#getCommunication) | **GET** /api/v1/communications/{communication_id} |  |
| [**getContactHistory**](CustomerCommunicationApi.md#getContactHistory) | **GET** /api/v1/contacts/{contact_id}/communications |  |
| [**listCommunications**](CustomerCommunicationApi.md#listCommunications) | **GET** /api/v1/communications/ |  |
| [**updateCommunication**](CustomerCommunicationApi.md#updateCommunication) | **PUT** /api/v1/communications/{communication_id} |  |


<a id="createCommunication"></a>
# **createCommunication**
> CustomerCommunication createCommunication(customerCommunicationCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val customerCommunicationCreate : CustomerCommunicationCreate =  // CustomerCommunicationCreate | 
try {
    val result : CustomerCommunication = apiInstance.createCommunication(customerCommunicationCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#createCommunication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#createCommunication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerCommunicationCreate** | [**CustomerCommunicationCreate**](CustomerCommunicationCreate.md)|  | |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

<a id="customercommunicationRestore"></a>
# **customercommunicationRestore**
> CustomerCommunication customercommunicationRestore(communicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val communicationId : kotlin.String = communicationId_example // kotlin.String | 
try {
    val result : CustomerCommunication = apiInstance.customercommunicationRestore(communicationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#customercommunicationRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#customercommunicationRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **communicationId** | **kotlin.String**|  | |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

<a id="deleteCommunication"></a>
# **deleteCommunication**
> deleteCommunication(communicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val communicationId : kotlin.String = communicationId_example // kotlin.String | 
try {
    apiInstance.deleteCommunication(communicationId)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#deleteCommunication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#deleteCommunication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **communicationId** | **kotlin.String**|  | |

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

<a id="getCommunication"></a>
# **getCommunication**
> CustomerCommunication getCommunication(communicationId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val communicationId : kotlin.String = communicationId_example // kotlin.String | 
try {
    val result : CustomerCommunication = apiInstance.getCommunication(communicationId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#getCommunication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#getCommunication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **communicationId** | **kotlin.String**|  | |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

<a id="getContactHistory"></a>
# **getContactHistory**
> ContactHistoryResponse getContactHistory(contactId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    val result : ContactHistoryResponse = apiInstance.getContactHistory(contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#getContactHistory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#getContactHistory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |

### Return type

[**ContactHistoryResponse**](ContactHistoryResponse.md)

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

<a id="listCommunications"></a>
# **listCommunications**
> kotlin.collections.List&lt;CustomerCommunication&gt; listCommunications(page, pageSize, contactId, channel, direction, from, to)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val contactId : kotlin.String = contactId_example // kotlin.String | Filter history to a single contact.
val channel : CommunicationChannel =  // CommunicationChannel | 
val direction : CommunicationDirection =  // CommunicationDirection | 
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only include communications after this ISO date (inclusive).
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only include communications before this ISO date (inclusive).
try {
    val result : kotlin.collections.List<CustomerCommunication> = apiInstance.listCommunications(page, pageSize, contactId, channel, direction, from, to)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#listCommunications")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#listCommunications")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **contactId** | **kotlin.String**| Filter history to a single contact. | [optional] |
| **channel** | [**CommunicationChannel**](.md)|  | [optional] [enum: email, call, meeting, chat, note] |
| **direction** | [**CommunicationDirection**](.md)|  | [optional] [enum: inbound, outbound] |
| **from** | **java.time.LocalDate**| Only include communications after this ISO date (inclusive). | [optional] |
| **to** | **java.time.LocalDate**| Only include communications before this ISO date (inclusive). | [optional] |

### Return type

[**kotlin.collections.List&lt;CustomerCommunication&gt;**](CustomerCommunication.md)

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

<a id="updateCommunication"></a>
# **updateCommunication**
> CustomerCommunication updateCommunication(communicationId, customerCommunicationUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerCommunicationApi()
val communicationId : kotlin.String = communicationId_example // kotlin.String | 
val customerCommunicationUpdate : CustomerCommunicationUpdate =  // CustomerCommunicationUpdate | 
try {
    val result : CustomerCommunication = apiInstance.updateCommunication(communicationId, customerCommunicationUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerCommunicationApi#updateCommunication")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerCommunicationApi#updateCommunication")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **communicationId** | **kotlin.String**|  | |
| **customerCommunicationUpdate** | [**CustomerCommunicationUpdate**](CustomerCommunicationUpdate.md)|  | |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

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

