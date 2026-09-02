# ContactApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**contactSchema**](ContactApi.md#contactSchema) | **GET** /api/v1/contacts/schema | Serve JSON Schema for client-side validation |
| [**contactTimeline**](ContactApi.md#contactTimeline) | **GET** /api/v1/contacts/{contact_id}/timeline | Get the full per-contact timeline (Xentral §4.6/4.7). |
| [**createContact**](ContactApi.md#createContact) | **POST** /api/v1/contacts | Create contact |
| [**deleteContact**](ContactApi.md#deleteContact) | **DELETE** /api/v1/contacts/{contact_id} | Soft-delete contact |
| [**getContact**](ContactApi.md#getContact) | **GET** /api/v1/contacts/{contact_id} | Get single contact |
| [**listContacts**](ContactApi.md#listContacts) | **GET** /api/v1/contacts | List contacts with search, type filter, and pagination |
| [**salesVolume**](ContactApi.md#salesVolume) | **GET** /api/v1/contacts/sales-volume | Sales volume per contact |
| [**updateContact**](ContactApi.md#updateContact) | **PUT** /api/v1/contacts/{contact_id} | Update contact |


<a id="contactSchema"></a>
# **contactSchema**
> kotlin.Any contactSchema()

Serve JSON Schema for client-side validation

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
try {
    val result : kotlin.Any = apiInstance.contactSchema()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#contactSchema")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#contactSchema")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="contactTimeline"></a>
# **contactTimeline**
> ContactTimelineResponse contactTimeline(contactId)

Get the full per-contact timeline (Xentral §4.6/4.7).

Aggregates communications, quotations, orders, invoices and uploaded documents for a contact, merged into a single reverse-chronological feed.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    val result : ContactTimelineResponse = apiInstance.contactTimeline(contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#contactTimeline")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#contactTimeline")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |

### Return type

[**ContactTimelineResponse**](ContactTimelineResponse.md)

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

<a id="createContact"></a>
# **createContact**
> Contact createContact(body)

Create contact

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Contact = apiInstance.createContact(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#createContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#createContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**Contact**](Contact.md)

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

<a id="deleteContact"></a>
# **deleteContact**
> deleteContact(contactId)

Soft-delete contact

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    apiInstance.deleteContact(contactId)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#deleteContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#deleteContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |

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

<a id="getContact"></a>
# **getContact**
> Contact getContact(contactId)

Get single contact

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    val result : Contact = apiInstance.getContact(contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#getContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#getContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |

### Return type

[**Contact**](Contact.md)

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

<a id="listContacts"></a>
# **listContacts**
> kotlin.collections.List&lt;Contact&gt; listContacts(page, pageSize, search, contactType, tag)

List contacts with search, type filter, and pagination

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val contactType : kotlin.String = contactType_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Contact> = apiInstance.listContacts(page, pageSize, search, contactType, tag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#listContacts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#listContacts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **contactType** | **kotlin.String**|  | [optional] |
| **tag** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Contact&gt;**](Contact.md)

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

<a id="salesVolume"></a>
# **salesVolume**
> SalesVolumeReport salesVolume(page, pageSize, search, contactType, tag)

Sales volume per contact

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val contactType : kotlin.String = contactType_example // kotlin.String | 
val tag : kotlin.String = tag_example // kotlin.String | 
try {
    val result : SalesVolumeReport = apiInstance.salesVolume(page, pageSize, search, contactType, tag)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#salesVolume")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#salesVolume")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **contactType** | **kotlin.String**|  | [optional] |
| **tag** | **kotlin.String**|  | [optional] |

### Return type

[**SalesVolumeReport**](SalesVolumeReport.md)

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

<a id="updateContact"></a>
# **updateContact**
> Contact updateContact(contactId, body)

Update contact

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ContactApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Contact = apiInstance.updateContact(contactId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ContactApi#updateContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ContactApi#updateContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Contact**](Contact.md)

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

