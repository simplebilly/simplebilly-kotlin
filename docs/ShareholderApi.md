# ShareholderApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createShareholder**](ShareholderApi.md#createShareholder) | **POST** /api/v1/shareholders |  |
| [**deleteShareholder**](ShareholderApi.md#deleteShareholder) | **DELETE** /api/v1/shareholders/{id} |  |
| [**getShareholder**](ShareholderApi.md#getShareholder) | **GET** /api/v1/shareholders/{id} |  |
| [**getShareholders**](ShareholderApi.md#getShareholders) | **GET** /api/v1/shareholders/ |  |
| [**updateShareholder**](ShareholderApi.md#updateShareholder) | **PUT** /api/v1/shareholders/{id} |  |


<a id="createShareholder"></a>
# **createShareholder**
> Shareholder createShareholder(shareholderCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShareholderApi()
val shareholderCreate : ShareholderCreate =  // ShareholderCreate | 
try {
    val result : Shareholder = apiInstance.createShareholder(shareholderCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareholderApi#createShareholder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareholderApi#createShareholder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shareholderCreate** | [**ShareholderCreate**](ShareholderCreate.md)|  | |

### Return type

[**Shareholder**](Shareholder.md)

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

<a id="deleteShareholder"></a>
# **deleteShareholder**
> deleteShareholder(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShareholderApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteShareholder(id)
} catch (e: ClientException) {
    println("4xx response calling ShareholderApi#deleteShareholder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareholderApi#deleteShareholder")
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

<a id="getShareholder"></a>
# **getShareholder**
> Shareholder getShareholder(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShareholderApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Shareholder = apiInstance.getShareholder(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareholderApi#getShareholder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareholderApi#getShareholder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Shareholder**](Shareholder.md)

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

<a id="getShareholders"></a>
# **getShareholders**
> kotlin.collections.List&lt;Shareholder&gt; getShareholders(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShareholderApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Shareholder> = apiInstance.getShareholders(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareholderApi#getShareholders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareholderApi#getShareholders")
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

[**kotlin.collections.List&lt;Shareholder&gt;**](Shareholder.md)

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

<a id="updateShareholder"></a>
# **updateShareholder**
> Shareholder updateShareholder(id, shareholderUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShareholderApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val shareholderUpdate : ShareholderUpdate =  // ShareholderUpdate | 
try {
    val result : Shareholder = apiInstance.updateShareholder(id, shareholderUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShareholderApi#updateShareholder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShareholderApi#updateShareholder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **shareholderUpdate** | [**ShareholderUpdate**](ShareholderUpdate.md)|  | |

### Return type

[**Shareholder**](Shareholder.md)

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

