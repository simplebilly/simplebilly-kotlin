# DeliveryDateApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createDeliveryDate**](DeliveryDateApi.md#createDeliveryDate) | **POST** /api/v1/delivery-dates |  |
| [**deleteDeliveryDate**](DeliveryDateApi.md#deleteDeliveryDate) | **DELETE** /api/v1/delivery-dates/{delivery_date_id} |  |
| [**getDeliveryDate**](DeliveryDateApi.md#getDeliveryDate) | **GET** /api/v1/delivery-dates/{delivery_date_id} |  |
| [**getDeliveryPerformance**](DeliveryDateApi.md#getDeliveryPerformance) | **GET** /api/v1/delivery-dates/performance | On-time performance summary: how many promised delivery dates were met within a period. |
| [**listDeliveryDates**](DeliveryDateApi.md#listDeliveryDates) | **GET** /api/v1/delivery-dates/ |  |
| [**updateDeliveryDate**](DeliveryDateApi.md#updateDeliveryDate) | **PUT** /api/v1/delivery-dates/{delivery_date_id} |  |
| [**updateDeliveryDateStatus**](DeliveryDateApi.md#updateDeliveryDateStatus) | **PUT** /api/v1/delivery-dates/{delivery_date_id}/status |  |


<a id="createDeliveryDate"></a>
# **createDeliveryDate**
> DeliveryDate createDeliveryDate(deliveryDateCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val deliveryDateCreate : DeliveryDateCreate =  // DeliveryDateCreate | 
try {
    val result : DeliveryDate = apiInstance.createDeliveryDate(deliveryDateCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#createDeliveryDate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#createDeliveryDate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryDateCreate** | [**DeliveryDateCreate**](DeliveryDateCreate.md)|  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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

<a id="deleteDeliveryDate"></a>
# **deleteDeliveryDate**
> deleteDeliveryDate(deliveryDateId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val deliveryDateId : kotlin.String = deliveryDateId_example // kotlin.String | 
try {
    apiInstance.deleteDeliveryDate(deliveryDateId)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#deleteDeliveryDate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#deleteDeliveryDate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryDateId** | **kotlin.String**|  | |

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

<a id="getDeliveryDate"></a>
# **getDeliveryDate**
> DeliveryDate getDeliveryDate(deliveryDateId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val deliveryDateId : kotlin.String = deliveryDateId_example // kotlin.String | 
try {
    val result : DeliveryDate = apiInstance.getDeliveryDate(deliveryDateId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#getDeliveryDate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#getDeliveryDate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryDateId** | **kotlin.String**|  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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

<a id="getDeliveryPerformance"></a>
# **getDeliveryPerformance**
> kotlin.Any getDeliveryPerformance(page, pageSize, orderNumber, status, from, to)

On-time performance summary: how many promised delivery dates were met within a period.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only dates on or after this date.
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only dates on or before this date.
try {
    val result : kotlin.Any = apiInstance.getDeliveryPerformance(page, pageSize, orderNumber, status, from, to)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#getDeliveryPerformance")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#getDeliveryPerformance")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderNumber** | **kotlin.String**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **from** | **java.time.LocalDate**| Only dates on or after this date. | [optional] |
| **to** | **java.time.LocalDate**| Only dates on or before this date. | [optional] |

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

<a id="listDeliveryDates"></a>
# **listDeliveryDates**
> kotlin.collections.List&lt;DeliveryDate&gt; listDeliveryDates(page, pageSize, orderNumber, status, from, to)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val status : kotlin.String = status_example // kotlin.String | 
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only dates on or after this date.
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | Only dates on or before this date.
try {
    val result : kotlin.collections.List<DeliveryDate> = apiInstance.listDeliveryDates(page, pageSize, orderNumber, status, from, to)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#listDeliveryDates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#listDeliveryDates")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **orderNumber** | **kotlin.String**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **from** | **java.time.LocalDate**| Only dates on or after this date. | [optional] |
| **to** | **java.time.LocalDate**| Only dates on or before this date. | [optional] |

### Return type

[**kotlin.collections.List&lt;DeliveryDate&gt;**](DeliveryDate.md)

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

<a id="updateDeliveryDate"></a>
# **updateDeliveryDate**
> DeliveryDate updateDeliveryDate(deliveryDateId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val deliveryDateId : kotlin.String = deliveryDateId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : DeliveryDate = apiInstance.updateDeliveryDate(deliveryDateId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#updateDeliveryDate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#updateDeliveryDate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryDateId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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

<a id="updateDeliveryDateStatus"></a>
# **updateDeliveryDateStatus**
> DeliveryDate updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryDateApi()
val deliveryDateId : kotlin.String = deliveryDateId_example // kotlin.String | 
val deliveryDateStatusUpdate : DeliveryDateStatusUpdate =  // DeliveryDateStatusUpdate | 
try {
    val result : DeliveryDate = apiInstance.updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryDateApi#updateDeliveryDateStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryDateApi#updateDeliveryDateStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryDateId** | **kotlin.String**|  | |
| **deliveryDateStatusUpdate** | [**DeliveryDateStatusUpdate**](DeliveryDateStatusUpdate.md)|  | |

### Return type

[**DeliveryDate**](DeliveryDate.md)

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

