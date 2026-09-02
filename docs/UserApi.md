# UserApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**changePassword**](UserApi.md#changePassword) | **POST** /user/change-password | Change the current user&#39;s password (requires the current password). |
| [**createTeam**](UserApi.md#createTeam) | **POST** /user/teams | Create a new team within the current tenant |
| [**generateApiKey**](UserApi.md#generateApiKey) | **POST** /user/api-key | Generate a new API key for the current user |
| [**inviteUser**](UserApi.md#inviteUser) | **POST** /user/invite | Invite a user to the current tenant/organization |
| [**listTeams**](UserApi.md#listTeams) | **GET** /user/teams | List all teams in the current tenant |
| [**removeUserFromOrg**](UserApi.md#removeUserFromOrg) | **DELETE** /user/remove | Remove a user from the current organization |
| [**updateProfile**](UserApi.md#updateProfile) | **PUT** /user/profile | Update the current user&#39;s profile |
| [**userProfile**](UserApi.md#userProfile) | **GET** /user/profile | Get the current user&#39;s profile |
| [**userTenants**](UserApi.md#userTenants) | **GET** /user/tenants | List all tenants (organizations) the current user belongs to |


<a id="changePassword"></a>
# **changePassword**
> changePassword(changePasswordRequest)

Change the current user&#39;s password (requires the current password).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
val changePasswordRequest : ChangePasswordRequest =  // ChangePasswordRequest | 
try {
    apiInstance.changePassword(changePasswordRequest)
} catch (e: ClientException) {
    println("4xx response calling UserApi#changePassword")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#changePassword")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **changePasswordRequest** | [**ChangePasswordRequest**](ChangePasswordRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="createTeam"></a>
# **createTeam**
> ApiResponseTeam createTeam(teamCreate)

Create a new team within the current tenant

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
val teamCreate : TeamCreate =  // TeamCreate | 
try {
    val result : ApiResponseTeam = apiInstance.createTeam(teamCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#createTeam")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#createTeam")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **teamCreate** | [**TeamCreate**](TeamCreate.md)|  | |

### Return type

[**ApiResponseTeam**](ApiResponseTeam.md)

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

<a id="generateApiKey"></a>
# **generateApiKey**
> ApiResponseString generateApiKey()

Generate a new API key for the current user

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
try {
    val result : ApiResponseString = apiInstance.generateApiKey()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#generateApiKey")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#generateApiKey")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseString**](ApiResponseString.md)

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

<a id="inviteUser"></a>
# **inviteUser**
> inviteUser(inviteRequest)

Invite a user to the current tenant/organization

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
val inviteRequest : InviteRequest =  // InviteRequest | 
try {
    apiInstance.inviteUser(inviteRequest)
} catch (e: ClientException) {
    println("4xx response calling UserApi#inviteUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#inviteUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **inviteRequest** | [**InviteRequest**](InviteRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="listTeams"></a>
# **listTeams**
> ApiResponseVecTeam listTeams()

List all teams in the current tenant

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
try {
    val result : ApiResponseVecTeam = apiInstance.listTeams()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#listTeams")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#listTeams")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseVecTeam**](ApiResponseVecTeam.md)

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

<a id="removeUserFromOrg"></a>
# **removeUserFromOrg**
> removeUserFromOrg(removeUserRequest)

Remove a user from the current organization

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
val removeUserRequest : RemoveUserRequest =  // RemoveUserRequest | 
try {
    apiInstance.removeUserFromOrg(removeUserRequest)
} catch (e: ClientException) {
    println("4xx response calling UserApi#removeUserFromOrg")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#removeUserFromOrg")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **removeUserRequest** | [**RemoveUserRequest**](RemoveUserRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="updateProfile"></a>
# **updateProfile**
> updateProfile(updateProfileRequest)

Update the current user&#39;s profile

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
val updateProfileRequest : UpdateProfileRequest =  // UpdateProfileRequest | 
try {
    apiInstance.updateProfile(updateProfileRequest)
} catch (e: ClientException) {
    println("4xx response calling UserApi#updateProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#updateProfile")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **updateProfileRequest** | [**UpdateProfileRequest**](UpdateProfileRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: Not defined

<a id="userProfile"></a>
# **userProfile**
> ApiResponseUserProfile userProfile()

Get the current user&#39;s profile

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
try {
    val result : ApiResponseUserProfile = apiInstance.userProfile()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#userProfile")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#userProfile")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseUserProfile**](ApiResponseUserProfile.md)

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

<a id="userTenants"></a>
# **userTenants**
> ApiResponseVecUserTenantInfo userTenants()

List all tenants (organizations) the current user belongs to

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserApi()
try {
    val result : ApiResponseVecUserTenantInfo = apiInstance.userTenants()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserApi#userTenants")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserApi#userTenants")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseVecUserTenantInfo**](ApiResponseVecUserTenantInfo.md)

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

