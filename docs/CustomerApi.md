# CustomerApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createCustomer**](CustomerApi.md#createCustomer) | **POST** /api/v1/customers |  |
| [**customerRestore**](CustomerApi.md#customerRestore) | **POST** /api/v1/customers/{customer_id}/restore |  |
| [**deleteCustomer**](CustomerApi.md#deleteCustomer) | **DELETE** /api/v1/customers/{customer_id} |  |
| [**getCustomer**](CustomerApi.md#getCustomer) | **GET** /api/v1/customers/{customer_id} |  |
| [**getCustomers**](CustomerApi.md#getCustomers) | **GET** /api/v1/customers/ |  |
| [**updateCustomer**](CustomerApi.md#updateCustomer) | **PUT** /api/v1/customers/{customer_id} |  |


<a id="createCustomer"></a>
# **createCustomer**
> Customer createCustomer(customerCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerApi()
val customerCreate : CustomerCreate =  // CustomerCreate | 
try {
    val result : Customer = apiInstance.createCustomer(customerCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerApi#createCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerApi#createCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerCreate** | [**CustomerCreate**](CustomerCreate.md)|  | |

### Return type

[**Customer**](Customer.md)

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

<a id="customerRestore"></a>
# **customerRestore**
> Customer customerRestore(customerId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerApi()
val customerId : kotlin.String = customerId_example // kotlin.String | 
try {
    val result : Customer = apiInstance.customerRestore(customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerApi#customerRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerApi#customerRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**|  | |

### Return type

[**Customer**](Customer.md)

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

<a id="deleteCustomer"></a>
# **deleteCustomer**
> deleteCustomer(customerId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerApi()
val customerId : kotlin.String = customerId_example // kotlin.String | 
try {
    apiInstance.deleteCustomer(customerId)
} catch (e: ClientException) {
    println("4xx response calling CustomerApi#deleteCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerApi#deleteCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**|  | |

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

<a id="getCustomer"></a>
# **getCustomer**
> Customer getCustomer(customerId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerApi()
val customerId : kotlin.String = customerId_example // kotlin.String | 
try {
    val result : Customer = apiInstance.getCustomer(customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerApi#getCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerApi#getCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**|  | |

### Return type

[**Customer**](Customer.md)

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

<a id="getCustomers"></a>
# **getCustomers**
> kotlin.collections.List&lt;Customer&gt; getCustomers(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Customer> = apiInstance.getCustomers(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerApi#getCustomers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerApi#getCustomers")
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

[**kotlin.collections.List&lt;Customer&gt;**](Customer.md)

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

<a id="updateCustomer"></a>
# **updateCustomer**
> Customer updateCustomer(customerId, customerUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerApi()
val customerId : kotlin.String = customerId_example // kotlin.String | 
val customerUpdate : CustomerUpdate =  // CustomerUpdate | 
try {
    val result : Customer = apiInstance.updateCustomer(customerId, customerUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerApi#updateCustomer")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerApi#updateCustomer")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**|  | |
| **customerUpdate** | [**CustomerUpdate**](CustomerUpdate.md)|  | |

### Return type

[**Customer**](Customer.md)

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

