# PackingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**completePacking**](PackingApi.md#completePacking) | **POST** /api/v1/packing/{order_number}/complete | Mark packing as complete and transition order to shipped |
| [**getPackingQueue**](PackingApi.md#getPackingQueue) | **GET** /api/v1/packing/queue | Get the packing queue - orders ready for packing |
| [**printDeliveryNote**](PackingApi.md#printDeliveryNote) | **POST** /api/v1/packing/{order_number}/print-delivery-note | Print delivery note (Lieferschein) for an order |
| [**printLabel**](PackingApi.md#printLabel) | **POST** /api/v1/packing/{order_number}/print-label | Print shipping label for an order |
| [**recordPackingVideo**](PackingApi.md#recordPackingVideo) | **POST** /api/v1/packing/{order_number}/record-video | Record video of packing process |


<a id="completePacking"></a>
# **completePacking**
> PackingCompleteResponse completePacking(orderNumber, packingCompleteRequest)

Mark packing as complete and transition order to shipped

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PackingApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val packingCompleteRequest : PackingCompleteRequest =  // PackingCompleteRequest | 
try {
    val result : PackingCompleteResponse = apiInstance.completePacking(orderNumber, packingCompleteRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PackingApi#completePacking")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PackingApi#completePacking")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |
| **packingCompleteRequest** | [**PackingCompleteRequest**](PackingCompleteRequest.md)|  | |

### Return type

[**PackingCompleteResponse**](PackingCompleteResponse.md)

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

<a id="getPackingQueue"></a>
# **getPackingQueue**
> PackingQueue getPackingQueue(page, pageSize, search)

Get the packing queue - orders ready for packing

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PackingApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : PackingQueue = apiInstance.getPackingQueue(page, pageSize, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PackingApi#getPackingQueue")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PackingApi#getPackingQueue")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**PackingQueue**](PackingQueue.md)

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

<a id="printDeliveryNote"></a>
# **printDeliveryNote**
> PrintDeliveryNoteResponse printDeliveryNote(orderNumber)

Print delivery note (Lieferschein) for an order

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PackingApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : PrintDeliveryNoteResponse = apiInstance.printDeliveryNote(orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PackingApi#printDeliveryNote")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PackingApi#printDeliveryNote")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |

### Return type

[**PrintDeliveryNoteResponse**](PrintDeliveryNoteResponse.md)

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

<a id="printLabel"></a>
# **printLabel**
> PrintLabelResponse printLabel(orderNumber)

Print shipping label for an order

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PackingApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : PrintLabelResponse = apiInstance.printLabel(orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PackingApi#printLabel")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PackingApi#printLabel")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |

### Return type

[**PrintLabelResponse**](PrintLabelResponse.md)

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

<a id="recordPackingVideo"></a>
# **recordPackingVideo**
> PackingVideoResponse recordPackingVideo(orderNumber, body)

Record video of packing process

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PackingApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : PackingVideoResponse = apiInstance.recordPackingVideo(orderNumber, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PackingApi#recordPackingVideo")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PackingApi#recordPackingVideo")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**PackingVideoResponse**](PackingVideoResponse.md)

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

