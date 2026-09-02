# GroupFigureApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createGroupFigure**](GroupFigureApi.md#createGroupFigure) | **POST** /api/v1/group-figures |  |
| [**deleteGroupFigure**](GroupFigureApi.md#deleteGroupFigure) | **DELETE** /api/v1/group-figures/{year} |  |
| [**getGroupFigure**](GroupFigureApi.md#getGroupFigure) | **GET** /api/v1/group-figures/{year} |  |
| [**getGroupFigures**](GroupFigureApi.md#getGroupFigures) | **GET** /api/v1/group-figures/ |  |
| [**updateGroupFigure**](GroupFigureApi.md#updateGroupFigure) | **PUT** /api/v1/group-figures/{year} |  |


<a id="createGroupFigure"></a>
# **createGroupFigure**
> GroupFigure createGroupFigure(groupFigureCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupFigureApi()
val groupFigureCreate : GroupFigureCreate =  // GroupFigureCreate | 
try {
    val result : GroupFigure = apiInstance.createGroupFigure(groupFigureCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupFigureApi#createGroupFigure")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupFigureApi#createGroupFigure")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **groupFigureCreate** | [**GroupFigureCreate**](GroupFigureCreate.md)|  | |

### Return type

[**GroupFigure**](GroupFigure.md)

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

<a id="deleteGroupFigure"></a>
# **deleteGroupFigure**
> deleteGroupFigure(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupFigureApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    apiInstance.deleteGroupFigure(year)
} catch (e: ClientException) {
    println("4xx response calling GroupFigureApi#deleteGroupFigure")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupFigureApi#deleteGroupFigure")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

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

<a id="getGroupFigure"></a>
# **getGroupFigure**
> GroupFigure getGroupFigure(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupFigureApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : GroupFigure = apiInstance.getGroupFigure(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupFigureApi#getGroupFigure")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupFigureApi#getGroupFigure")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**GroupFigure**](GroupFigure.md)

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

<a id="getGroupFigures"></a>
# **getGroupFigures**
> kotlin.collections.List&lt;GroupFigure&gt; getGroupFigures(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupFigureApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<GroupFigure> = apiInstance.getGroupFigures(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupFigureApi#getGroupFigures")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupFigureApi#getGroupFigures")
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

[**kotlin.collections.List&lt;GroupFigure&gt;**](GroupFigure.md)

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

<a id="updateGroupFigure"></a>
# **updateGroupFigure**
> GroupFigure updateGroupFigure(year, groupFigureUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GroupFigureApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val groupFigureUpdate : GroupFigureUpdate =  // GroupFigureUpdate | 
try {
    val result : GroupFigure = apiInstance.updateGroupFigure(year, groupFigureUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GroupFigureApi#updateGroupFigure")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GroupFigureApi#updateGroupFigure")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |
| **groupFigureUpdate** | [**GroupFigureUpdate**](GroupFigureUpdate.md)|  | |

### Return type

[**GroupFigure**](GroupFigure.md)

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

