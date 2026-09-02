# InventoryValueApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getInventoryValueApi**](InventoryValueApi.md#getInventoryValueApi) | **GET** /api/v1/bookkeeping/inventory-value |  |
| [**recordInventoryValueApi**](InventoryValueApi.md#recordInventoryValueApi) | **POST** /api/v1/bookkeeping/inventory-value/record |  |


<a id="getInventoryValueApi"></a>
# **getInventoryValueApi**
> CurrentInventoryValue getInventoryValueApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryValueApi()
try {
    val result : CurrentInventoryValue = apiInstance.getInventoryValueApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryValueApi#getInventoryValueApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryValueApi#getInventoryValueApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**CurrentInventoryValue**](CurrentInventoryValue.md)

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

<a id="recordInventoryValueApi"></a>
# **recordInventoryValueApi**
> InventoryValuePoint recordInventoryValueApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InventoryValueApi()
try {
    val result : InventoryValuePoint = apiInstance.recordInventoryValueApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InventoryValueApi#recordInventoryValueApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InventoryValueApi#recordInventoryValueApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InventoryValuePoint**](InventoryValuePoint.md)

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

