# ShippingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getCredentialsApi**](ShippingApi.md#getCredentialsApi) | **GET** /api/v1/shipping/credentials |  |
| [**getRatesApi**](ShippingApi.md#getRatesApi) | **POST** /api/v1/shipping/rates |  |
| [**listProvidersApi**](ShippingApi.md#listProvidersApi) | **GET** /api/v1/shipping/providers |  |
| [**saveCredentialsApi**](ShippingApi.md#saveCredentialsApi) | **PUT** /api/v1/shipping/credentials |  |


<a id="getCredentialsApi"></a>
# **getCredentialsApi**
> ShippingCredentials getCredentialsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingApi()
try {
    val result : ShippingCredentials = apiInstance.getCredentialsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingApi#getCredentialsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingApi#getCredentialsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ShippingCredentials**](ShippingCredentials.md)

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

<a id="getRatesApi"></a>
# **getRatesApi**
> RateResponse getRatesApi(rateRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingApi()
val rateRequest : RateRequest =  // RateRequest | 
try {
    val result : RateResponse = apiInstance.getRatesApi(rateRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingApi#getRatesApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingApi#getRatesApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rateRequest** | [**RateRequest**](RateRequest.md)|  | |

### Return type

[**RateResponse**](RateResponse.md)

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

<a id="listProvidersApi"></a>
# **listProvidersApi**
> kotlin.collections.List&lt;ProviderInfo&gt; listProvidersApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingApi()
try {
    val result : kotlin.collections.List<ProviderInfo> = apiInstance.listProvidersApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingApi#listProvidersApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingApi#listProvidersApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;ProviderInfo&gt;**](ProviderInfo.md)

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

<a id="saveCredentialsApi"></a>
# **saveCredentialsApi**
> ShippingCredentials saveCredentialsApi(shippingCredentials)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShippingApi()
val shippingCredentials : ShippingCredentials =  // ShippingCredentials | 
try {
    val result : ShippingCredentials = apiInstance.saveCredentialsApi(shippingCredentials)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShippingApi#saveCredentialsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShippingApi#saveCredentialsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shippingCredentials** | [**ShippingCredentials**](ShippingCredentials.md)|  | |

### Return type

[**ShippingCredentials**](ShippingCredentials.md)

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

