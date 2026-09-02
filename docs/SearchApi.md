# SearchApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**globalSearch**](SearchApi.md#globalSearch) | **GET** /api/v1/search | GET /api/v1/search?q&#x3D;... |
| [**myPermissions**](SearchApi.md#myPermissions) | **GET** /api/v1/me/permissions | GET /api/v1/me/permissions — resolved permissions from the auth token, used by the frontend to show/hide admin navigation. |


<a id="globalSearch"></a>
# **globalSearch**
> kotlin.Any globalSearch(q)

GET /api/v1/search?q&#x3D;...

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SearchApi()
val q : kotlin.String = q_example // kotlin.String | Search text (min 2 chars)
try {
    val result : kotlin.Any = apiInstance.globalSearch(q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#globalSearch")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#globalSearch")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**| Search text (min 2 chars) | |

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

<a id="myPermissions"></a>
# **myPermissions**
> kotlin.Any myPermissions()

GET /api/v1/me/permissions — resolved permissions from the auth token, used by the frontend to show/hide admin navigation.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SearchApi()
try {
    val result : kotlin.Any = apiInstance.myPermissions()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SearchApi#myPermissions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SearchApi#myPermissions")
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

