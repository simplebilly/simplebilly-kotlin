# UserManagementApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getUser**](UserManagementApi.md#getUser) | **GET** /api/v1/users/{user_id} |  |
| [**listUsers**](UserManagementApi.md#listUsers) | **GET** /api/v1/users |  |
| [**removeUser**](UserManagementApi.md#removeUser) | **DELETE** /api/v1/users/{user_id} |  |
| [**updateUserPermissions**](UserManagementApi.md#updateUserPermissions) | **PUT** /api/v1/users/{user_id}/permissions |  |
| [**updateUserRole**](UserManagementApi.md#updateUserRole) | **PUT** /api/v1/users/{user_id}/role |  |


<a id="getUser"></a>
# **getUser**
> TenantUser getUser(userId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserManagementApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : TenantUser = apiInstance.getUser(userId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserManagementApi#getUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserManagementApi#getUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |

### Return type

[**TenantUser**](TenantUser.md)

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

<a id="listUsers"></a>
# **listUsers**
> kotlin.collections.List&lt;TenantUser&gt; listUsers()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserManagementApi()
try {
    val result : kotlin.collections.List<TenantUser> = apiInstance.listUsers()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling UserManagementApi#listUsers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserManagementApi#listUsers")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;TenantUser&gt;**](TenantUser.md)

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

<a id="removeUser"></a>
# **removeUser**
> removeUser(userId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserManagementApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.removeUser(userId)
} catch (e: ClientException) {
    println("4xx response calling UserManagementApi#removeUser")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserManagementApi#removeUser")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |

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
 - **Accept**: Not defined

<a id="updateUserPermissions"></a>
# **updateUserPermissions**
> updateUserPermissions(userId, updatePermissionsPayload)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserManagementApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val updatePermissionsPayload : UpdatePermissionsPayload =  // UpdatePermissionsPayload | 
try {
    apiInstance.updateUserPermissions(userId, updatePermissionsPayload)
} catch (e: ClientException) {
    println("4xx response calling UserManagementApi#updateUserPermissions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserManagementApi#updateUserPermissions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |
| **updatePermissionsPayload** | [**UpdatePermissionsPayload**](UpdatePermissionsPayload.md)|  | |

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

<a id="updateUserRole"></a>
# **updateUserRole**
> updateUserRole(userId, updateRolePayload)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = UserManagementApi()
val userId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val updateRolePayload : UpdateRolePayload =  // UpdateRolePayload | 
try {
    apiInstance.updateUserRole(userId, updateRolePayload)
} catch (e: ClientException) {
    println("4xx response calling UserManagementApi#updateUserRole")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling UserManagementApi#updateUserRole")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **userId** | **java.util.UUID**|  | |
| **updateRolePayload** | [**UpdateRolePayload**](UpdateRolePayload.md)|  | |

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

