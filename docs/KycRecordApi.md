# KycRecordApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createKycRecord**](KycRecordApi.md#createKycRecord) | **POST** /api/v1/kyc-records |  |
| [**deleteKycRecord**](KycRecordApi.md#deleteKycRecord) | **DELETE** /api/v1/kyc-records/{id} |  |
| [**getKycRecord**](KycRecordApi.md#getKycRecord) | **GET** /api/v1/kyc-records/{id} |  |
| [**getKycRecords**](KycRecordApi.md#getKycRecords) | **GET** /api/v1/kyc-records/ |  |
| [**updateKycRecord**](KycRecordApi.md#updateKycRecord) | **PUT** /api/v1/kyc-records/{id} |  |


<a id="createKycRecord"></a>
# **createKycRecord**
> KycRecord createKycRecord(kycRecordCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KycRecordApi()
val kycRecordCreate : KycRecordCreate =  // KycRecordCreate | 
try {
    val result : KycRecord = apiInstance.createKycRecord(kycRecordCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KycRecordApi#createKycRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KycRecordApi#createKycRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **kycRecordCreate** | [**KycRecordCreate**](KycRecordCreate.md)|  | |

### Return type

[**KycRecord**](KycRecord.md)

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

<a id="deleteKycRecord"></a>
# **deleteKycRecord**
> deleteKycRecord(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KycRecordApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteKycRecord(id)
} catch (e: ClientException) {
    println("4xx response calling KycRecordApi#deleteKycRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KycRecordApi#deleteKycRecord")
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

<a id="getKycRecord"></a>
# **getKycRecord**
> KycRecord getKycRecord(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KycRecordApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : KycRecord = apiInstance.getKycRecord(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KycRecordApi#getKycRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KycRecordApi#getKycRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**KycRecord**](KycRecord.md)

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

<a id="getKycRecords"></a>
# **getKycRecords**
> kotlin.collections.List&lt;KycRecord&gt; getKycRecords(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KycRecordApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<KycRecord> = apiInstance.getKycRecords(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KycRecordApi#getKycRecords")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KycRecordApi#getKycRecords")
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

[**kotlin.collections.List&lt;KycRecord&gt;**](KycRecord.md)

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

<a id="updateKycRecord"></a>
# **updateKycRecord**
> KycRecord updateKycRecord(id, kycRecordUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = KycRecordApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val kycRecordUpdate : KycRecordUpdate =  // KycRecordUpdate | 
try {
    val result : KycRecord = apiInstance.updateKycRecord(id, kycRecordUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling KycRecordApi#updateKycRecord")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling KycRecordApi#updateKycRecord")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **kycRecordUpdate** | [**KycRecordUpdate**](KycRecordUpdate.md)|  | |

### Return type

[**KycRecord**](KycRecord.md)

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

