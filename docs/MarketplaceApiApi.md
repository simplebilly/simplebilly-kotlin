# MarketplaceApiApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createConnectionApi**](MarketplaceApiApi.md#createConnectionApi) | **POST** /api/v1/marketplace/connections | Create a new connection (for API-key based platforms) |
| [**deleteConnectionApi**](MarketplaceApiApi.md#deleteConnectionApi) | **DELETE** /api/v1/marketplace/connections/{connection_id} | Soft-delete a connection |
| [**getConnectionApi**](MarketplaceApiApi.md#getConnectionApi) | **GET** /api/v1/marketplace/connections/{connection_id} | Get a single connection |
| [**getSyncDirectionApi**](MarketplaceApiApi.md#getSyncDirectionApi) | **GET** /api/v1/marketplace/connections/{connection_id}/directions | Get current sync direction configuration for a connection |
| [**getSyncLogsApi**](MarketplaceApiApi.md#getSyncLogsApi) | **GET** /api/v1/marketplace/connections/{connection_id}/logs | Get sync logs for a connection |
| [**listConnectionsApi**](MarketplaceApiApi.md#listConnectionsApi) | **GET** /api/v1/marketplace/connections | List connections for the current tenant |
| [**listPlatformsApi**](MarketplaceApiApi.md#listPlatformsApi) | **GET** /api/v1/marketplace/platforms | List all supported platforms |
| [**oauthAuthorizeApi**](MarketplaceApiApi.md#oauthAuthorizeApi) | **POST** /api/v1/marketplace/oauth/authorize | OAuth: initiate authorization flow |
| [**oauthCallbackApi**](MarketplaceApiApi.md#oauthCallbackApi) | **POST** /api/v1/marketplace/oauth/callback | OAuth: handle callback after authorization |
| [**triggerSyncApi**](MarketplaceApiApi.md#triggerSyncApi) | **POST** /api/v1/marketplace/connections/{connection_id}/sync | Trigger sync for a connection |
| [**updateConnectionApi**](MarketplaceApiApi.md#updateConnectionApi) | **PUT** /api/v1/marketplace/connections/{connection_id} | Update a connection |
| [**updateSyncDirectionApi**](MarketplaceApiApi.md#updateSyncDirectionApi) | **PUT** /api/v1/marketplace/connections/{connection_id}/directions | Update per-entity sync direction configuration for a connection |
| [**webhookReceiverApi**](MarketplaceApiApi.md#webhookReceiverApi) | **POST** /api/v1/marketplace/webhook/{platform}/{connection_id} | Webhook receiver |


<a id="createConnectionApi"></a>
# **createConnectionApi**
> MarketplaceConnection createConnectionApi(createConnectionRequest)

Create a new connection (for API-key based platforms)

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val createConnectionRequest : CreateConnectionRequest =  // CreateConnectionRequest | 
try {
    val result : MarketplaceConnection = apiInstance.createConnectionApi(createConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#createConnectionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#createConnectionApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createConnectionRequest** | [**CreateConnectionRequest**](CreateConnectionRequest.md)|  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

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

<a id="deleteConnectionApi"></a>
# **deleteConnectionApi**
> deleteConnectionApi(connectionId)

Soft-delete a connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
try {
    apiInstance.deleteConnectionApi(connectionId)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#deleteConnectionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#deleteConnectionApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |

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

<a id="getConnectionApi"></a>
# **getConnectionApi**
> MarketplaceConnection getConnectionApi(connectionId)

Get a single connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
try {
    val result : MarketplaceConnection = apiInstance.getConnectionApi(connectionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#getConnectionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#getConnectionApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

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

<a id="getSyncDirectionApi"></a>
# **getSyncDirectionApi**
> getSyncDirectionApi(connectionId)

Get current sync direction configuration for a connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
try {
    apiInstance.getSyncDirectionApi(connectionId)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#getSyncDirectionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#getSyncDirectionApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |

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

<a id="getSyncLogsApi"></a>
# **getSyncLogsApi**
> kotlin.collections.List&lt;SyncLog&gt; getSyncLogsApi(connectionId)

Get sync logs for a connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<SyncLog> = apiInstance.getSyncLogsApi(connectionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#getSyncLogsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#getSyncLogsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;SyncLog&gt;**](SyncLog.md)

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

<a id="listConnectionsApi"></a>
# **listConnectionsApi**
> kotlin.collections.List&lt;MarketplaceConnection&gt; listConnectionsApi()

List connections for the current tenant

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
try {
    val result : kotlin.collections.List<MarketplaceConnection> = apiInstance.listConnectionsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#listConnectionsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#listConnectionsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;MarketplaceConnection&gt;**](MarketplaceConnection.md)

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

<a id="listPlatformsApi"></a>
# **listPlatformsApi**
> kotlin.collections.List&lt;PlatformInfo&gt; listPlatformsApi()

List all supported platforms

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
try {
    val result : kotlin.collections.List<PlatformInfo> = apiInstance.listPlatformsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#listPlatformsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#listPlatformsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PlatformInfo&gt;**](PlatformInfo.md)

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

<a id="oauthAuthorizeApi"></a>
# **oauthAuthorizeApi**
> OAuthAuthorizeResponse oauthAuthorizeApi(oauthAuthorizeRequest)

OAuth: initiate authorization flow

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val oauthAuthorizeRequest : OAuthAuthorizeRequest =  // OAuthAuthorizeRequest | 
try {
    val result : OAuthAuthorizeResponse = apiInstance.oauthAuthorizeApi(oauthAuthorizeRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#oauthAuthorizeApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#oauthAuthorizeApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **oauthAuthorizeRequest** | [**OAuthAuthorizeRequest**](OAuthAuthorizeRequest.md)|  | |

### Return type

[**OAuthAuthorizeResponse**](OAuthAuthorizeResponse.md)

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

<a id="oauthCallbackApi"></a>
# **oauthCallbackApi**
> MarketplaceConnection oauthCallbackApi(oauthCallbackRequest)

OAuth: handle callback after authorization

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val oauthCallbackRequest : OAuthCallbackRequest =  // OAuthCallbackRequest | 
try {
    val result : MarketplaceConnection = apiInstance.oauthCallbackApi(oauthCallbackRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#oauthCallbackApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#oauthCallbackApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **oauthCallbackRequest** | [**OAuthCallbackRequest**](OAuthCallbackRequest.md)|  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

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

<a id="triggerSyncApi"></a>
# **triggerSyncApi**
> SyncSummary triggerSyncApi(connectionId, syncType, direction)

Trigger sync for a connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
val syncType : kotlin.String = syncType_example // kotlin.String | 
val direction : kotlin.String = direction_example // kotlin.String | 
try {
    val result : SyncSummary = apiInstance.triggerSyncApi(connectionId, syncType, direction)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#triggerSyncApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#triggerSyncApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |
| **syncType** | **kotlin.String**|  | [optional] |
| **direction** | **kotlin.String**|  | [optional] |

### Return type

[**SyncSummary**](SyncSummary.md)

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

<a id="updateConnectionApi"></a>
# **updateConnectionApi**
> MarketplaceConnection updateConnectionApi(connectionId, updateConnectionRequest)

Update a connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
val updateConnectionRequest : UpdateConnectionRequest =  // UpdateConnectionRequest | 
try {
    val result : MarketplaceConnection = apiInstance.updateConnectionApi(connectionId, updateConnectionRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#updateConnectionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#updateConnectionApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |
| **updateConnectionRequest** | [**UpdateConnectionRequest**](UpdateConnectionRequest.md)|  | |

### Return type

[**MarketplaceConnection**](MarketplaceConnection.md)

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

<a id="updateSyncDirectionApi"></a>
# **updateSyncDirectionApi**
> updateSyncDirectionApi(connectionId, updateSyncDirectionRequest)

Update per-entity sync direction configuration for a connection

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
val updateSyncDirectionRequest : UpdateSyncDirectionRequest =  // UpdateSyncDirectionRequest | 
try {
    apiInstance.updateSyncDirectionApi(connectionId, updateSyncDirectionRequest)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#updateSyncDirectionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#updateSyncDirectionApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **connectionId** | **kotlin.String**|  | |
| **updateSyncDirectionRequest** | [**UpdateSyncDirectionRequest**](UpdateSyncDirectionRequest.md)|  | |

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

<a id="webhookReceiverApi"></a>
# **webhookReceiverApi**
> webhookReceiverApi(platform, connectionId)

Webhook receiver

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = MarketplaceApiApi()
val platform : kotlin.String = platform_example // kotlin.String | 
val connectionId : kotlin.String = connectionId_example // kotlin.String | 
try {
    apiInstance.webhookReceiverApi(platform, connectionId)
} catch (e: ClientException) {
    println("4xx response calling MarketplaceApiApi#webhookReceiverApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling MarketplaceApiApi#webhookReceiverApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **platform** | **kotlin.String**|  | |
| **connectionId** | **kotlin.String**|  | |

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

