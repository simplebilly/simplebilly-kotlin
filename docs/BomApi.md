# BomApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createBom**](BomApi.md#createBom) | **POST** /api/v1/boms |  |
| [**deleteBom**](BomApi.md#deleteBom) | **DELETE** /api/v1/boms/{bom_id} |  |
| [**getBom**](BomApi.md#getBom) | **GET** /api/v1/boms/{bom_id} |  |
| [**listBoms**](BomApi.md#listBoms) | **GET** /api/v1/boms/ |  |
| [**updateBom**](BomApi.md#updateBom) | **PUT** /api/v1/boms/{bom_id} |  |


<a id="createBom"></a>
# **createBom**
> Bom createBom(bomCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BomApi()
val bomCreate : BomCreate =  // BomCreate | 
try {
    val result : Bom = apiInstance.createBom(bomCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BomApi#createBom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BomApi#createBom")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bomCreate** | [**BomCreate**](BomCreate.md)|  | |

### Return type

[**Bom**](Bom.md)

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

<a id="deleteBom"></a>
# **deleteBom**
> deleteBom(bomId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BomApi()
val bomId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteBom(bomId)
} catch (e: ClientException) {
    println("4xx response calling BomApi#deleteBom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BomApi#deleteBom")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bomId** | **java.util.UUID**|  | |

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

<a id="getBom"></a>
# **getBom**
> Bom getBom(bomId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BomApi()
val bomId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Bom = apiInstance.getBom(bomId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BomApi#getBom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BomApi#getBom")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bomId** | **java.util.UUID**|  | |

### Return type

[**Bom**](Bom.md)

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

<a id="listBoms"></a>
# **listBoms**
> kotlin.collections.List&lt;Bom&gt; listBoms(page, pageSize, search, productId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BomApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val productId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | Filter by finished product id.
try {
    val result : kotlin.collections.List<Bom> = apiInstance.listBoms(page, pageSize, search, productId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BomApi#listBoms")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BomApi#listBoms")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **productId** | **java.util.UUID**| Filter by finished product id. | [optional] |

### Return type

[**kotlin.collections.List&lt;Bom&gt;**](Bom.md)

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

<a id="updateBom"></a>
# **updateBom**
> Bom updateBom(bomId, bomUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BomApi()
val bomId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val bomUpdate : BomUpdate =  // BomUpdate | 
try {
    val result : Bom = apiInstance.updateBom(bomId, bomUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BomApi#updateBom")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BomApi#updateBom")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **bomId** | **java.util.UUID**|  | |
| **bomUpdate** | [**BomUpdate**](BomUpdate.md)|  | |

### Return type

[**Bom**](Bom.md)

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

