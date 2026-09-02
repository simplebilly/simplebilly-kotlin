# TenantSettingsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getTenantSettings**](TenantSettingsApi.md#getTenantSettings) | **GET** /api/v1/settings/tenant |  |
| [**updateTenantSettings**](TenantSettingsApi.md#updateTenantSettings) | **PUT** /api/v1/settings/tenant |  |


<a id="getTenantSettings"></a>
# **getTenantSettings**
> TenantSettings getTenantSettings()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TenantSettingsApi()
try {
    val result : TenantSettings = apiInstance.getTenantSettings()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TenantSettingsApi#getTenantSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TenantSettingsApi#getTenantSettings")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**TenantSettings**](TenantSettings.md)

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

<a id="updateTenantSettings"></a>
# **updateTenantSettings**
> TenantSettings updateTenantSettings(updateTenantSettings)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TenantSettingsApi()
val updateTenantSettings : UpdateTenantSettings =  // UpdateTenantSettings | 
try {
    val result : TenantSettings = apiInstance.updateTenantSettings(updateTenantSettings)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TenantSettingsApi#updateTenantSettings")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TenantSettingsApi#updateTenantSettings")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateTenantSettings** | [**UpdateTenantSettings**](UpdateTenantSettings.md)|  | |

### Return type

[**TenantSettings**](TenantSettings.md)

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

