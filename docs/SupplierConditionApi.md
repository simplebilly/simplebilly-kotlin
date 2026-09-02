# SupplierConditionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createSupplierCondition**](SupplierConditionApi.md#createSupplierCondition) | **POST** /api/v1/supplier-conditions |  |
| [**deleteSupplierCondition**](SupplierConditionApi.md#deleteSupplierCondition) | **DELETE** /api/v1/supplier-conditions/{supplier_condition_id} |  |
| [**getSupplierCondition**](SupplierConditionApi.md#getSupplierCondition) | **GET** /api/v1/supplier-conditions/{supplier_condition_id} |  |
| [**listSupplierConditions**](SupplierConditionApi.md#listSupplierConditions) | **GET** /api/v1/supplier-conditions/ |  |
| [**updateSupplierCondition**](SupplierConditionApi.md#updateSupplierCondition) | **PUT** /api/v1/supplier-conditions/{supplier_condition_id} |  |


<a id="createSupplierCondition"></a>
# **createSupplierCondition**
> SupplierCondition createSupplierCondition(supplierConditionCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierConditionApi()
val supplierConditionCreate : SupplierConditionCreate =  // SupplierConditionCreate | 
try {
    val result : SupplierCondition = apiInstance.createSupplierCondition(supplierConditionCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierConditionApi#createSupplierCondition")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierConditionApi#createSupplierCondition")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierConditionCreate** | [**SupplierConditionCreate**](SupplierConditionCreate.md)|  | |

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

<a id="deleteSupplierCondition"></a>
# **deleteSupplierCondition**
> deleteSupplierCondition(supplierConditionId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierConditionApi()
val supplierConditionId : kotlin.String = supplierConditionId_example // kotlin.String | 
try {
    apiInstance.deleteSupplierCondition(supplierConditionId)
} catch (e: ClientException) {
    println("4xx response calling SupplierConditionApi#deleteSupplierCondition")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierConditionApi#deleteSupplierCondition")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierConditionId** | **kotlin.String**|  | |

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

<a id="getSupplierCondition"></a>
# **getSupplierCondition**
> SupplierCondition getSupplierCondition(supplierConditionId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierConditionApi()
val supplierConditionId : kotlin.String = supplierConditionId_example // kotlin.String | 
try {
    val result : SupplierCondition = apiInstance.getSupplierCondition(supplierConditionId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierConditionApi#getSupplierCondition")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierConditionApi#getSupplierCondition")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierConditionId** | **kotlin.String**|  | |

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

<a id="listSupplierConditions"></a>
# **listSupplierConditions**
> kotlin.collections.List&lt;SupplierCondition&gt; listSupplierConditions(page, pageSize, supplierContactId, search)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierConditionApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val supplierContactId : kotlin.String = supplierContactId_example // kotlin.String | 
val search : kotlin.String = search_example // kotlin.String | 
try {
    val result : kotlin.collections.List<SupplierCondition> = apiInstance.listSupplierConditions(page, pageSize, supplierContactId, search)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierConditionApi#listSupplierConditions")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierConditionApi#listSupplierConditions")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **supplierContactId** | **kotlin.String**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;SupplierCondition&gt;**](SupplierCondition.md)

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

<a id="updateSupplierCondition"></a>
# **updateSupplierCondition**
> SupplierCondition updateSupplierCondition(supplierConditionId, supplierConditionUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = SupplierConditionApi()
val supplierConditionId : kotlin.String = supplierConditionId_example // kotlin.String | 
val supplierConditionUpdate : SupplierConditionUpdate =  // SupplierConditionUpdate | 
try {
    val result : SupplierCondition = apiInstance.updateSupplierCondition(supplierConditionId, supplierConditionUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling SupplierConditionApi#updateSupplierCondition")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling SupplierConditionApi#updateSupplierCondition")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **supplierConditionId** | **kotlin.String**|  | |
| **supplierConditionUpdate** | [**SupplierConditionUpdate**](SupplierConditionUpdate.md)|  | |

### Return type

[**SupplierCondition**](SupplierCondition.md)

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

