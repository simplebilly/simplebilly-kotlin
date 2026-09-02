# EmissionsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createEmissionEntryApi**](EmissionsApi.md#createEmissionEntryApi) | **POST** /api/v1/bookkeeping/emissions/entries |  |
| [**createEmissionTargetApi**](EmissionsApi.md#createEmissionTargetApi) | **POST** /api/v1/bookkeeping/emissions/targets |  |
| [**deleteEmissionEntryApi**](EmissionsApi.md#deleteEmissionEntryApi) | **DELETE** /api/v1/bookkeeping/emissions/entries/{id} |  |
| [**deleteEmissionTargetApi**](EmissionsApi.md#deleteEmissionTargetApi) | **DELETE** /api/v1/bookkeeping/emissions/targets/{id} |  |
| [**emissionsEntriesApi**](EmissionsApi.md#emissionsEntriesApi) | **GET** /api/v1/bookkeeping/emissions/entries |  |
| [**emissionsExportApi**](EmissionsApi.md#emissionsExportApi) | **GET** /api/v1/bookkeeping/emissions/export |  |
| [**emissionsFactorsApi**](EmissionsApi.md#emissionsFactorsApi) | **GET** /api/v1/bookkeeping/emissions/factors |  |
| [**emissionsReportApi**](EmissionsApi.md#emissionsReportApi) | **GET** /api/v1/bookkeeping/emissions/report |  |
| [**emissionsTargetsApi**](EmissionsApi.md#emissionsTargetsApi) | **GET** /api/v1/bookkeeping/emissions/targets |  |


<a id="createEmissionEntryApi"></a>
# **createEmissionEntryApi**
> EmissionEntry createEmissionEntryApi(createEmissionEntry)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val createEmissionEntry : CreateEmissionEntry =  // CreateEmissionEntry | 
try {
    val result : EmissionEntry = apiInstance.createEmissionEntryApi(createEmissionEntry)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#createEmissionEntryApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#createEmissionEntryApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createEmissionEntry** | [**CreateEmissionEntry**](CreateEmissionEntry.md)|  | |

### Return type

[**EmissionEntry**](EmissionEntry.md)

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

<a id="createEmissionTargetApi"></a>
# **createEmissionTargetApi**
> EmissionTarget createEmissionTargetApi(createEmissionTarget)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val createEmissionTarget : CreateEmissionTarget =  // CreateEmissionTarget | 
try {
    val result : EmissionTarget = apiInstance.createEmissionTargetApi(createEmissionTarget)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#createEmissionTargetApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#createEmissionTargetApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **createEmissionTarget** | [**CreateEmissionTarget**](CreateEmissionTarget.md)|  | |

### Return type

[**EmissionTarget**](EmissionTarget.md)

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

<a id="deleteEmissionEntryApi"></a>
# **deleteEmissionEntryApi**
> deleteEmissionEntryApi(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteEmissionEntryApi(id)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#deleteEmissionEntryApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#deleteEmissionEntryApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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
 - **Accept**: application/json

<a id="deleteEmissionTargetApi"></a>
# **deleteEmissionTargetApi**
> deleteEmissionTargetApi(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteEmissionTargetApi(id)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#deleteEmissionTargetApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#deleteEmissionTargetApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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
 - **Accept**: application/json

<a id="emissionsEntriesApi"></a>
# **emissionsEntriesApi**
> kotlin.collections.List&lt;EmissionEntry&gt; emissionsEntriesApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : kotlin.collections.List<EmissionEntry> = apiInstance.emissionsEntriesApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#emissionsEntriesApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#emissionsEntriesApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**kotlin.collections.List&lt;EmissionEntry&gt;**](EmissionEntry.md)

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

<a id="emissionsExportApi"></a>
# **emissionsExportApi**
> EmissionsExportResponse emissionsExportApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EmissionsExportResponse = apiInstance.emissionsExportApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#emissionsExportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#emissionsExportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**EmissionsExportResponse**](EmissionsExportResponse.md)

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

<a id="emissionsFactorsApi"></a>
# **emissionsFactorsApi**
> kotlin.collections.List&lt;EmissionFactorResponse&gt; emissionsFactorsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
try {
    val result : kotlin.collections.List<EmissionFactorResponse> = apiInstance.emissionsFactorsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#emissionsFactorsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#emissionsFactorsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;EmissionFactorResponse&gt;**](EmissionFactorResponse.md)

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

<a id="emissionsReportApi"></a>
# **emissionsReportApi**
> EmissionsReport emissionsReportApi(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : EmissionsReport = apiInstance.emissionsReportApi(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#emissionsReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#emissionsReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**EmissionsReport**](EmissionsReport.md)

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

<a id="emissionsTargetsApi"></a>
# **emissionsTargetsApi**
> kotlin.collections.List&lt;EmissionTarget&gt; emissionsTargetsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmissionsApi()
try {
    val result : kotlin.collections.List<EmissionTarget> = apiInstance.emissionsTargetsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmissionsApi#emissionsTargetsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmissionsApi#emissionsTargetsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;EmissionTarget&gt;**](EmissionTarget.md)

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

