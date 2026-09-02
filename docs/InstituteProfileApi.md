# InstituteProfileApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getInstituteProfile**](InstituteProfileApi.md#getInstituteProfile) | **GET** /api/v1/institute-profile | Current institute profile (created with defaults when missing). |
| [**updateInstituteProfile**](InstituteProfileApi.md#updateInstituteProfile) | **PUT** /api/v1/institute-profile | Update the institute profile (institute_type and/or kapitalmarktorientiert). |


<a id="getInstituteProfile"></a>
# **getInstituteProfile**
> InstituteProfile getInstituteProfile()

Current institute profile (created with defaults when missing).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InstituteProfileApi()
try {
    val result : InstituteProfile = apiInstance.getInstituteProfile()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InstituteProfileApi#getInstituteProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InstituteProfileApi#getInstituteProfile")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**InstituteProfile**](InstituteProfile.md)

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

<a id="updateInstituteProfile"></a>
# **updateInstituteProfile**
> InstituteProfile updateInstituteProfile(instituteProfileUpdate)

Update the institute profile (institute_type and/or kapitalmarktorientiert).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = InstituteProfileApi()
val instituteProfileUpdate : InstituteProfileUpdate =  // InstituteProfileUpdate | 
try {
    val result : InstituteProfile = apiInstance.updateInstituteProfile(instituteProfileUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling InstituteProfileApi#updateInstituteProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling InstituteProfileApi#updateInstituteProfile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **instituteProfileUpdate** | [**InstituteProfileUpdate**](InstituteProfileUpdate.md)|  | |

### Return type

[**InstituteProfile**](InstituteProfile.md)

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

