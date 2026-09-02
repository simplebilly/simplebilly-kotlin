# DeclarationApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createDeclaration**](DeclarationApi.md#createDeclaration) | **POST** /api/v1/declarations |  |
| [**declarationRestore**](DeclarationApi.md#declarationRestore) | **POST** /api/v1/declarations/{id}/restore |  |
| [**deleteDeclaration**](DeclarationApi.md#deleteDeclaration) | **DELETE** /api/v1/declarations/{id} |  |
| [**getDeclaration**](DeclarationApi.md#getDeclaration) | **GET** /api/v1/declarations/{id} |  |
| [**getDeclarations**](DeclarationApi.md#getDeclarations) | **GET** /api/v1/declarations/ |  |
| [**updateDeclaration**](DeclarationApi.md#updateDeclaration) | **PUT** /api/v1/declarations/{id} |  |


<a id="createDeclaration"></a>
# **createDeclaration**
> Declaration createDeclaration(declarationCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeclarationApi()
val declarationCreate : DeclarationCreate =  // DeclarationCreate | 
try {
    val result : Declaration = apiInstance.createDeclaration(declarationCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeclarationApi#createDeclaration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeclarationApi#createDeclaration")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **declarationCreate** | [**DeclarationCreate**](DeclarationCreate.md)|  | |

### Return type

[**Declaration**](Declaration.md)

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

<a id="declarationRestore"></a>
# **declarationRestore**
> Declaration declarationRestore(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeclarationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Declaration = apiInstance.declarationRestore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeclarationApi#declarationRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeclarationApi#declarationRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Declaration**](Declaration.md)

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

<a id="deleteDeclaration"></a>
# **deleteDeclaration**
> deleteDeclaration(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeclarationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteDeclaration(id)
} catch (e: ClientException) {
    println("4xx response calling DeclarationApi#deleteDeclaration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeclarationApi#deleteDeclaration")
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

<a id="getDeclaration"></a>
# **getDeclaration**
> Declaration getDeclaration(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeclarationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Declaration = apiInstance.getDeclaration(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeclarationApi#getDeclaration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeclarationApi#getDeclaration")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Declaration**](Declaration.md)

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

<a id="getDeclarations"></a>
# **getDeclarations**
> kotlin.collections.List&lt;Declaration&gt; getDeclarations(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeclarationApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Declaration> = apiInstance.getDeclarations(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeclarationApi#getDeclarations")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeclarationApi#getDeclarations")
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

[**kotlin.collections.List&lt;Declaration&gt;**](Declaration.md)

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

<a id="updateDeclaration"></a>
# **updateDeclaration**
> Declaration updateDeclaration(id, declarationUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeclarationApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val declarationUpdate : DeclarationUpdate =  // DeclarationUpdate | 
try {
    val result : Declaration = apiInstance.updateDeclaration(id, declarationUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeclarationApi#updateDeclaration")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeclarationApi#updateDeclaration")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **declarationUpdate** | [**DeclarationUpdate**](DeclarationUpdate.md)|  | |

### Return type

[**Declaration**](Declaration.md)

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

