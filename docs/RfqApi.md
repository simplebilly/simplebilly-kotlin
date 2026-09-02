# RfqApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**convertRfq**](RfqApi.md#convertRfq) | **POST** /api/v1/rfqs/{rfq_id}/convert | Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;. |
| [**createRfq**](RfqApi.md#createRfq) | **POST** /api/v1/rfqs |  |
| [**deleteRfq**](RfqApi.md#deleteRfq) | **DELETE** /api/v1/rfqs/{rfq_id} |  |
| [**getRfq**](RfqApi.md#getRfq) | **GET** /api/v1/rfqs/{rfq_id} |  |
| [**listRfqs**](RfqApi.md#listRfqs) | **GET** /api/v1/rfqs/ |  |
| [**updateRfq**](RfqApi.md#updateRfq) | **PUT** /api/v1/rfqs/{rfq_id} |  |
| [**updateRfqStatus**](RfqApi.md#updateRfqStatus) | **PUT** /api/v1/rfqs/{rfq_id}/status |  |


<a id="convertRfq"></a>
# **convertRfq**
> kotlin.Any convertRfq(rfqId)

Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val rfqId : kotlin.String = rfqId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.convertRfq(rfqId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#convertRfq")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#convertRfq")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rfqId** | **kotlin.String**|  | |

### Return type

[**kotlin.Any**](kotlin.Any.md)

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

<a id="createRfq"></a>
# **createRfq**
> Rfq createRfq(rfq)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val rfq : Rfq =  // Rfq | 
try {
    val result : Rfq = apiInstance.createRfq(rfq)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#createRfq")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#createRfq")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rfq** | [**Rfq**](Rfq.md)|  | |

### Return type

[**Rfq**](Rfq.md)

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

<a id="deleteRfq"></a>
# **deleteRfq**
> deleteRfq(rfqId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val rfqId : kotlin.String = rfqId_example // kotlin.String | 
try {
    apiInstance.deleteRfq(rfqId)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#deleteRfq")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#deleteRfq")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rfqId** | **kotlin.String**|  | |

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

<a id="getRfq"></a>
# **getRfq**
> Rfq getRfq(rfqId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val rfqId : kotlin.String = rfqId_example // kotlin.String | 
try {
    val result : Rfq = apiInstance.getRfq(rfqId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#getRfq")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#getRfq")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rfqId** | **kotlin.String**|  | |

### Return type

[**Rfq**](Rfq.md)

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

<a id="listRfqs"></a>
# **listRfqs**
> kotlin.collections.List&lt;Rfq&gt; listRfqs(page, pageSize, status, supplierName)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val supplierName : kotlin.String = supplierName_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Rfq> = apiInstance.listRfqs(page, pageSize, status, supplierName)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#listRfqs")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#listRfqs")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **supplierName** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Rfq&gt;**](Rfq.md)

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

<a id="updateRfq"></a>
# **updateRfq**
> Rfq updateRfq(rfqId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val rfqId : kotlin.String = rfqId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Rfq = apiInstance.updateRfq(rfqId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#updateRfq")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#updateRfq")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rfqId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Rfq**](Rfq.md)

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

<a id="updateRfqStatus"></a>
# **updateRfqStatus**
> Rfq updateRfqStatus(rfqId, rfqStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = RfqApi()
val rfqId : kotlin.String = rfqId_example // kotlin.String | 
val rfqStatusUpdate : RfqStatusUpdate =  // RfqStatusUpdate | 
try {
    val result : Rfq = apiInstance.updateRfqStatus(rfqId, rfqStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling RfqApi#updateRfqStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling RfqApi#updateRfqStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **rfqId** | **kotlin.String**|  | |
| **rfqStatusUpdate** | [**RfqStatusUpdate**](RfqStatusUpdate.md)|  | |

### Return type

[**Rfq**](Rfq.md)

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

