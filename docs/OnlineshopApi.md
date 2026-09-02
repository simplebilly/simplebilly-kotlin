# OnlineshopApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getSmtpConfigApi**](OnlineshopApi.md#getSmtpConfigApi) | **GET** /api/v1/settings/smtp |  |
| [**saveSmtpConfigApi**](OnlineshopApi.md#saveSmtpConfigApi) | **PUT** /api/v1/settings/smtp |  |


<a id="getSmtpConfigApi"></a>
# **getSmtpConfigApi**
> SmtpConfig getSmtpConfigApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OnlineshopApi()
try {
    val result : SmtpConfig = apiInstance.getSmtpConfigApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnlineshopApi#getSmtpConfigApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnlineshopApi#getSmtpConfigApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**SmtpConfig**](SmtpConfig.md)

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

<a id="saveSmtpConfigApi"></a>
# **saveSmtpConfigApi**
> SmtpConfig saveSmtpConfigApi(smtpConfig)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = OnlineshopApi()
val smtpConfig : SmtpConfig =  // SmtpConfig | 
try {
    val result : SmtpConfig = apiInstance.saveSmtpConfigApi(smtpConfig)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling OnlineshopApi#saveSmtpConfigApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling OnlineshopApi#saveSmtpConfigApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **smtpConfig** | [**SmtpConfig**](SmtpConfig.md)|  | [optional] |

### Return type

[**SmtpConfig**](SmtpConfig.md)

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

