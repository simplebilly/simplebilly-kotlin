# PostingCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPostingCategory**](PostingCategoryApi.md#createPostingCategory) | **POST** /api/v1/posting-categories |  |
| [**deletePostingCategory**](PostingCategoryApi.md#deletePostingCategory) | **DELETE** /api/v1/posting-categories/{category_id} |  |
| [**listPostingCategories**](PostingCategoryApi.md#listPostingCategories) | **GET** /api/v1/posting-categories |  |
| [**seedPostingCategories**](PostingCategoryApi.md#seedPostingCategories) | **POST** /api/v1/posting-categories/seed/{skr_version} |  |
| [**updatePostingCategory**](PostingCategoryApi.md#updatePostingCategory) | **PUT** /api/v1/posting-categories/{category_id} |  |


<a id="createPostingCategory"></a>
# **createPostingCategory**
> PostingCategory createPostingCategory(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PostingCategoryApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PostingCategory = apiInstance.createPostingCategory(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PostingCategoryApi#createPostingCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostingCategoryApi#createPostingCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

### Return type

[**PostingCategory**](PostingCategory.md)

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

<a id="deletePostingCategory"></a>
# **deletePostingCategory**
> deletePostingCategory(categoryId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PostingCategoryApi()
val categoryId : kotlin.String = categoryId_example // kotlin.String | 
try {
    apiInstance.deletePostingCategory(categoryId)
} catch (e: ClientException) {
    println("4xx response calling PostingCategoryApi#deletePostingCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostingCategoryApi#deletePostingCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **categoryId** | **kotlin.String**|  | |

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

<a id="listPostingCategories"></a>
# **listPostingCategories**
> kotlin.collections.List&lt;PostingCategory&gt; listPostingCategories()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PostingCategoryApi()
try {
    val result : kotlin.collections.List<PostingCategory> = apiInstance.listPostingCategories()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PostingCategoryApi#listPostingCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostingCategoryApi#listPostingCategories")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PostingCategory&gt;**](PostingCategory.md)

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

<a id="seedPostingCategories"></a>
# **seedPostingCategories**
> seedPostingCategories(skrVersion)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PostingCategoryApi()
val skrVersion : kotlin.String = skrVersion_example // kotlin.String | 
try {
    apiInstance.seedPostingCategories(skrVersion)
} catch (e: ClientException) {
    println("4xx response calling PostingCategoryApi#seedPostingCategories")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostingCategoryApi#seedPostingCategories")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **skrVersion** | **kotlin.String**|  | |

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

<a id="updatePostingCategory"></a>
# **updatePostingCategory**
> PostingCategory updatePostingCategory(categoryId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PostingCategoryApi()
val categoryId : kotlin.String = categoryId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PostingCategory = apiInstance.updatePostingCategory(categoryId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PostingCategoryApi#updatePostingCategory")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PostingCategoryApi#updatePostingCategory")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **categoryId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**PostingCategory**](PostingCategory.md)

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

