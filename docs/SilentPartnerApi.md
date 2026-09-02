# SilentPartnerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createSilentPartner**](SilentPartnerApi.md#createSilentPartner) | **POST** /api/v1/silent-partners |  |
| [**deleteSilentPartner**](SilentPartnerApi.md#deleteSilentPartner) | **DELETE** /api/v1/silent-partners/{id} |  |
| [**getSilentPartner**](SilentPartnerApi.md#getSilentPartner) | **GET** /api/v1/silent-partners/{id} |  |
| [**getSilentPartners**](SilentPartnerApi.md#getSilentPartners) | **GET** /api/v1/silent-partners/ |  |
| [**updateSilentPartner**](SilentPartnerApi.md#updateSilentPartner) | **PUT** /api/v1/silent-partners/{id} |  |


<a id="createSilentPartner"></a>
# **createSilentPartner**
> SilentPartner createSilentPartner(silentPartnerCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SilentPartnerApi()
val silentPartnerCreate : SilentPartnerCreate =  // SilentPartnerCreate | 
try {
    val result : SilentPartner = apiInstance.createSilentPartner(silentPartnerCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SilentPartnerApi#createSilentPartner")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SilentPartnerApi#createSilentPartner")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **silentPartnerCreate** | [**SilentPartnerCreate**](SilentPartnerCreate.md)|  | |

### Return type

[**SilentPartner**](SilentPartner.md)

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

<a id="deleteSilentPartner"></a>
# **deleteSilentPartner**
> deleteSilentPartner(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SilentPartnerApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteSilentPartner(id)
} catch (e: ClientException) {
    println("4xx response calling SilentPartnerApi#deleteSilentPartner")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SilentPartnerApi#deleteSilentPartner")
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

<a id="getSilentPartner"></a>
# **getSilentPartner**
> SilentPartner getSilentPartner(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SilentPartnerApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : SilentPartner = apiInstance.getSilentPartner(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SilentPartnerApi#getSilentPartner")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SilentPartnerApi#getSilentPartner")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**SilentPartner**](SilentPartner.md)

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

<a id="getSilentPartners"></a>
# **getSilentPartners**
> kotlin.collections.List&lt;SilentPartner&gt; getSilentPartners(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SilentPartnerApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<SilentPartner> = apiInstance.getSilentPartners(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SilentPartnerApi#getSilentPartners")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SilentPartnerApi#getSilentPartners")
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

[**kotlin.collections.List&lt;SilentPartner&gt;**](SilentPartner.md)

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

<a id="updateSilentPartner"></a>
# **updateSilentPartner**
> SilentPartner updateSilentPartner(id, silentPartnerUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SilentPartnerApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val silentPartnerUpdate : SilentPartnerUpdate =  // SilentPartnerUpdate | 
try {
    val result : SilentPartner = apiInstance.updateSilentPartner(id, silentPartnerUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SilentPartnerApi#updateSilentPartner")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SilentPartnerApi#updateSilentPartner")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **silentPartnerUpdate** | [**SilentPartnerUpdate**](SilentPartnerUpdate.md)|  | |

### Return type

[**SilentPartner**](SilentPartner.md)

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

