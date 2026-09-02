# ShopApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**shopEditorSave**](ShopApi.md#shopEditorSave) | **POST** /api/v1/shop/editor |  |


<a id="shopEditorSave"></a>
# **shopEditorSave**
> kotlin.Any shopEditorSave(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShopApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.shopEditorSave(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShopApi#shopEditorSave")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShopApi#shopEditorSave")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

