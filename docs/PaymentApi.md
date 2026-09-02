# PaymentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createPayment**](PaymentApi.md#createPayment) | **POST** /api/v1/payments |  |
| [**deletePayment**](PaymentApi.md#deletePayment) | **DELETE** /api/v1/payments/{id} |  |
| [**getPayment**](PaymentApi.md#getPayment) | **GET** /api/v1/payments/{id} |  |
| [**getPayments**](PaymentApi.md#getPayments) | **GET** /api/v1/payments/ |  |
| [**paymentRestore**](PaymentApi.md#paymentRestore) | **POST** /api/v1/payments/{id}/restore |  |
| [**updatePayment**](PaymentApi.md#updatePayment) | **PUT** /api/v1/payments/{id} |  |


<a id="createPayment"></a>
# **createPayment**
> Payment createPayment(paymentCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentApi()
val paymentCreate : PaymentCreate =  // PaymentCreate | 
try {
    val result : Payment = apiInstance.createPayment(paymentCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#createPayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#createPayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **paymentCreate** | [**PaymentCreate**](PaymentCreate.md)|  | |

### Return type

[**Payment**](Payment.md)

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

<a id="deletePayment"></a>
# **deletePayment**
> deletePayment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deletePayment(id)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#deletePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#deletePayment")
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

<a id="getPayment"></a>
# **getPayment**
> Payment getPayment(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Payment = apiInstance.getPayment(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#getPayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#getPayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Payment**](Payment.md)

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

<a id="getPayments"></a>
# **getPayments**
> kotlin.collections.List&lt;Payment&gt; getPayments(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Payment> = apiInstance.getPayments(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#getPayments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#getPayments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;Payment&gt;**](Payment.md)

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

<a id="paymentRestore"></a>
# **paymentRestore**
> Payment paymentRestore(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Payment = apiInstance.paymentRestore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#paymentRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#paymentRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Payment**](Payment.md)

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

<a id="updatePayment"></a>
# **updatePayment**
> Payment updatePayment(id, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Payment = apiInstance.updatePayment(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentApi#updatePayment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentApi#updatePayment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Payment**](Payment.md)

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

