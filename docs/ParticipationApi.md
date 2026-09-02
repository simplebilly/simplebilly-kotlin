# ParticipationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createParticipation**](ParticipationApi.md#createParticipation) | **POST** /api/v1/participations |  |
| [**deleteParticipation**](ParticipationApi.md#deleteParticipation) | **DELETE** /api/v1/participations/{id} |  |
| [**getParticipation**](ParticipationApi.md#getParticipation) | **GET** /api/v1/participations/{id} |  |
| [**getParticipations**](ParticipationApi.md#getParticipations) | **GET** /api/v1/participations/ |  |
| [**updateParticipation**](ParticipationApi.md#updateParticipation) | **PUT** /api/v1/participations/{id} |  |


<a id="createParticipation"></a>
# **createParticipation**
> Participation createParticipation(participationCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ParticipationApi()
val participationCreate : ParticipationCreate =  // ParticipationCreate | 
try {
    val result : Participation = apiInstance.createParticipation(participationCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipationApi#createParticipation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipationApi#createParticipation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **participationCreate** | [**ParticipationCreate**](ParticipationCreate.md)|  | |

### Return type

[**Participation**](Participation.md)

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

<a id="deleteParticipation"></a>
# **deleteParticipation**
> deleteParticipation(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ParticipationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteParticipation(id)
} catch (e: ClientException) {
    println("4xx response calling ParticipationApi#deleteParticipation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipationApi#deleteParticipation")
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

<a id="getParticipation"></a>
# **getParticipation**
> Participation getParticipation(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ParticipationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Participation = apiInstance.getParticipation(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipationApi#getParticipation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipationApi#getParticipation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Participation**](Participation.md)

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

<a id="getParticipations"></a>
# **getParticipations**
> kotlin.collections.List&lt;Participation&gt; getParticipations(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ParticipationApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Participation> = apiInstance.getParticipations(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipationApi#getParticipations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipationApi#getParticipations")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;Participation&gt;**](Participation.md)

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

<a id="updateParticipation"></a>
# **updateParticipation**
> Participation updateParticipation(id, participationUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ParticipationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val participationUpdate : ParticipationUpdate =  // ParticipationUpdate | 
try {
    val result : Participation = apiInstance.updateParticipation(id, participationUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ParticipationApi#updateParticipation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ParticipationApi#updateParticipation")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **participationUpdate** | [**ParticipationUpdate**](ParticipationUpdate.md)|  | |

### Return type

[**Participation**](Participation.md)

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

