# DeliveryAppointmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createDeliveryAppointment**](DeliveryAppointmentApi.md#createDeliveryAppointment) | **POST** /api/v1/delivery-appointments |  |
| [**deleteDeliveryAppointment**](DeliveryAppointmentApi.md#deleteDeliveryAppointment) | **DELETE** /api/v1/delivery-appointments/{appointment_id} |  |
| [**getDeliveryAppointment**](DeliveryAppointmentApi.md#getDeliveryAppointment) | **GET** /api/v1/delivery-appointments/{appointment_id} |  |
| [**getPublicDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#getPublicDeliveryAppointmentStatus) | **GET** /api/v1/public/delivery-appointments/status | Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match. |
| [**listDeliveryAppointments**](DeliveryAppointmentApi.md#listDeliveryAppointments) | **GET** /api/v1/delivery-appointments |  |
| [**requestPublicDeliveryAppointment**](DeliveryAppointmentApi.md#requestPublicDeliveryAppointment) | **POST** /api/v1/public/delivery-appointments/request | Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request. |
| [**updateDeliveryAppointment**](DeliveryAppointmentApi.md#updateDeliveryAppointment) | **PUT** /api/v1/delivery-appointments/{appointment_id} |  |
| [**updateDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#updateDeliveryAppointmentStatus) | **PUT** /api/v1/delivery-appointments/{appointment_id}/status |  |


<a id="createDeliveryAppointment"></a>
# **createDeliveryAppointment**
> DeliveryAppointment createDeliveryAppointment(deliveryAppointmentCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val deliveryAppointmentCreate : DeliveryAppointmentCreate =  // DeliveryAppointmentCreate | 
try {
    val result : DeliveryAppointment = apiInstance.createDeliveryAppointment(deliveryAppointmentCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#createDeliveryAppointment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#createDeliveryAppointment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **deliveryAppointmentCreate** | [**DeliveryAppointmentCreate**](DeliveryAppointmentCreate.md)|  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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

<a id="deleteDeliveryAppointment"></a>
# **deleteDeliveryAppointment**
> deleteDeliveryAppointment(appointmentId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val appointmentId : kotlin.String = appointmentId_example // kotlin.String | 
try {
    apiInstance.deleteDeliveryAppointment(appointmentId)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#deleteDeliveryAppointment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#deleteDeliveryAppointment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **appointmentId** | **kotlin.String**|  | |

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

<a id="getDeliveryAppointment"></a>
# **getDeliveryAppointment**
> DeliveryAppointment getDeliveryAppointment(appointmentId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val appointmentId : kotlin.String = appointmentId_example // kotlin.String | 
try {
    val result : DeliveryAppointment = apiInstance.getDeliveryAppointment(appointmentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#getDeliveryAppointment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#getDeliveryAppointment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **appointmentId** | **kotlin.String**|  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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

<a id="getPublicDeliveryAppointmentStatus"></a>
# **getPublicDeliveryAppointmentStatus**
> PublicDeliveryAppointmentStatusResponse getPublicDeliveryAppointmentStatus(appointmentId, email, token)

Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val appointmentId : kotlin.String = appointmentId_example // kotlin.String | 
val email : kotlin.String = email_example // kotlin.String | 
val token : kotlin.String = token_example // kotlin.String | 
try {
    val result : PublicDeliveryAppointmentStatusResponse = apiInstance.getPublicDeliveryAppointmentStatus(appointmentId, email, token)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#getPublicDeliveryAppointmentStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#getPublicDeliveryAppointmentStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **appointmentId** | **kotlin.String**|  | |
| **email** | **kotlin.String**|  | |
| **token** | **kotlin.String**|  | |

### Return type

[**PublicDeliveryAppointmentStatusResponse**](PublicDeliveryAppointmentStatusResponse.md)

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

<a id="listDeliveryAppointments"></a>
# **listDeliveryAppointments**
> kotlin.collections.List&lt;DeliveryAppointment&gt; listDeliveryAppointments(page, pageSize, status, warehouseId, from, to)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
val warehouseId : kotlin.String = warehouseId_example // kotlin.String | 
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
try {
    val result : kotlin.collections.List<DeliveryAppointment> = apiInstance.listDeliveryAppointments(page, pageSize, status, warehouseId, from, to)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#listDeliveryAppointments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#listDeliveryAppointments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |
| **warehouseId** | **kotlin.String**|  | [optional] |
| **from** | **java.time.LocalDate**|  | [optional] |
| **to** | **java.time.LocalDate**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;DeliveryAppointment&gt;**](DeliveryAppointment.md)

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

<a id="requestPublicDeliveryAppointment"></a>
# **requestPublicDeliveryAppointment**
> PublicDeliveryAppointmentResponse requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest)

Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val publicDeliveryAppointmentRequest : PublicDeliveryAppointmentRequest =  // PublicDeliveryAppointmentRequest | 
try {
    val result : PublicDeliveryAppointmentResponse = apiInstance.requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#requestPublicDeliveryAppointment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#requestPublicDeliveryAppointment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **publicDeliveryAppointmentRequest** | [**PublicDeliveryAppointmentRequest**](PublicDeliveryAppointmentRequest.md)|  | |

### Return type

[**PublicDeliveryAppointmentResponse**](PublicDeliveryAppointmentResponse.md)

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

<a id="updateDeliveryAppointment"></a>
# **updateDeliveryAppointment**
> DeliveryAppointment updateDeliveryAppointment(appointmentId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val appointmentId : kotlin.String = appointmentId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : DeliveryAppointment = apiInstance.updateDeliveryAppointment(appointmentId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#updateDeliveryAppointment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#updateDeliveryAppointment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **appointmentId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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

<a id="updateDeliveryAppointmentStatus"></a>
# **updateDeliveryAppointmentStatus**
> DeliveryAppointment updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = DeliveryAppointmentApi()
val appointmentId : kotlin.String = appointmentId_example // kotlin.String | 
val appointmentStatusUpdate : AppointmentStatusUpdate =  // AppointmentStatusUpdate | 
try {
    val result : DeliveryAppointment = apiInstance.updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling DeliveryAppointmentApi#updateDeliveryAppointmentStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling DeliveryAppointmentApi#updateDeliveryAppointmentStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **appointmentId** | **kotlin.String**|  | |
| **appointmentStatusUpdate** | [**AppointmentStatusUpdate**](AppointmentStatusUpdate.md)|  | |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

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

