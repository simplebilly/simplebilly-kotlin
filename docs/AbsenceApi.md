# AbsenceApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createAbsence**](AbsenceApi.md#createAbsence) | **POST** /api/v1/absences |  |
| [**deleteAbsence**](AbsenceApi.md#deleteAbsence) | **DELETE** /api/v1/absences/{id} |  |
| [**getAbsence**](AbsenceApi.md#getAbsence) | **GET** /api/v1/absences/{id} |  |
| [**getAbsences**](AbsenceApi.md#getAbsences) | **GET** /api/v1/absences/ |  |
| [**updateAbsence**](AbsenceApi.md#updateAbsence) | **PUT** /api/v1/absences/{id} |  |


<a id="createAbsence"></a>
# **createAbsence**
> Absence createAbsence(absenceCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AbsenceApi()
val absenceCreate : AbsenceCreate =  // AbsenceCreate | 
try {
    val result : Absence = apiInstance.createAbsence(absenceCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AbsenceApi#createAbsence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AbsenceApi#createAbsence")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **absenceCreate** | [**AbsenceCreate**](AbsenceCreate.md)|  | |

### Return type

[**Absence**](Absence.md)

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

<a id="deleteAbsence"></a>
# **deleteAbsence**
> deleteAbsence(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AbsenceApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteAbsence(id)
} catch (e: ClientException) {
    println("4xx response calling AbsenceApi#deleteAbsence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AbsenceApi#deleteAbsence")
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

<a id="getAbsence"></a>
# **getAbsence**
> Absence getAbsence(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AbsenceApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Absence = apiInstance.getAbsence(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AbsenceApi#getAbsence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AbsenceApi#getAbsence")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Absence**](Absence.md)

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

<a id="getAbsences"></a>
# **getAbsences**
> kotlin.collections.List&lt;Absence&gt; getAbsences(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AbsenceApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Absence> = apiInstance.getAbsences(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AbsenceApi#getAbsences")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AbsenceApi#getAbsences")
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

[**kotlin.collections.List&lt;Absence&gt;**](Absence.md)

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

<a id="updateAbsence"></a>
# **updateAbsence**
> Absence updateAbsence(id, absenceUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = AbsenceApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val absenceUpdate : AbsenceUpdate =  // AbsenceUpdate | 
try {
    val result : Absence = apiInstance.updateAbsence(id, absenceUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling AbsenceApi#updateAbsence")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling AbsenceApi#updateAbsence")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **absenceUpdate** | [**AbsenceUpdate**](AbsenceUpdate.md)|  | |

### Return type

[**Absence**](Absence.md)

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

