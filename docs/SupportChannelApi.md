# SupportChannelApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createChannelApi**](SupportChannelApi.md#createChannelApi) | **POST** /api/v1/support/channels |  |
| [**deleteChannelApi**](SupportChannelApi.md#deleteChannelApi) | **DELETE** /api/v1/support/channels/{channel_id} |  |
| [**listChannelsApi**](SupportChannelApi.md#listChannelsApi) | **GET** /api/v1/support/channels |  |
| [**updateChannelApi**](SupportChannelApi.md#updateChannelApi) | **PUT** /api/v1/support/channels/{channel_id} |  |


<a id="createChannelApi"></a>
# **createChannelApi**
> SupportChannel createChannelApi(createChannelDto)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportChannelApi()
val createChannelDto : CreateChannelDto =  // CreateChannelDto | 
try {
    val result : SupportChannel = apiInstance.createChannelApi(createChannelDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportChannelApi#createChannelApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportChannelApi#createChannelApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createChannelDto** | [**CreateChannelDto**](CreateChannelDto.md)|  | |

### Return type

[**SupportChannel**](SupportChannel.md)

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

<a id="deleteChannelApi"></a>
# **deleteChannelApi**
> deleteChannelApi(channelId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportChannelApi()
val channelId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteChannelApi(channelId)
} catch (e: ClientException) {
    println("4xx response calling SupportChannelApi#deleteChannelApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportChannelApi#deleteChannelApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **channelId** | **java.util.UUID**|  | |

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

<a id="listChannelsApi"></a>
# **listChannelsApi**
> kotlin.collections.List&lt;SupportChannel&gt; listChannelsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportChannelApi()
try {
    val result : kotlin.collections.List<SupportChannel> = apiInstance.listChannelsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportChannelApi#listChannelsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportChannelApi#listChannelsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;SupportChannel&gt;**](SupportChannel.md)

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

<a id="updateChannelApi"></a>
# **updateChannelApi**
> SupportChannel updateChannelApi(channelId, updateChannelDto)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupportChannelApi()
val channelId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val updateChannelDto : UpdateChannelDto =  // UpdateChannelDto | 
try {
    val result : SupportChannel = apiInstance.updateChannelApi(channelId, updateChannelDto)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupportChannelApi#updateChannelApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupportChannelApi#updateChannelApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **channelId** | **java.util.UUID**|  | |
| **updateChannelDto** | [**UpdateChannelDto**](UpdateChannelDto.md)|  | |

### Return type

[**SupportChannel**](SupportChannel.md)

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

