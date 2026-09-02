# CustomerGroupApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**addGroupMembers**](CustomerGroupApi.md#addGroupMembers) | **POST** /api/v1/customer-groups/{customer_group_id}/members |  |
| [**createCustomerGroup**](CustomerGroupApi.md#createCustomerGroup) | **POST** /api/v1/customer-groups |  |
| [**deleteCustomerGroup**](CustomerGroupApi.md#deleteCustomerGroup) | **DELETE** /api/v1/customer-groups/{customer_group_id} |  |
| [**getCustomerGroup**](CustomerGroupApi.md#getCustomerGroup) | **GET** /api/v1/customer-groups/{customer_group_id} |  |
| [**listCustomerGroups**](CustomerGroupApi.md#listCustomerGroups) | **GET** /api/v1/customer-groups/ |  |
| [**updateCustomerGroup**](CustomerGroupApi.md#updateCustomerGroup) | **PUT** /api/v1/customer-groups/{customer_group_id} |  |


<a id="addGroupMembers"></a>
# **addGroupMembers**
> CustomerGroup addGroupMembers(customerGroupId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerGroupApi()
val customerGroupId : kotlin.String = customerGroupId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : CustomerGroup = apiInstance.addGroupMembers(customerGroupId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerGroupApi#addGroupMembers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerGroupApi#addGroupMembers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerGroupId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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

<a id="createCustomerGroup"></a>
# **createCustomerGroup**
> CustomerGroup createCustomerGroup(customerGroupCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerGroupApi()
val customerGroupCreate : CustomerGroupCreate =  // CustomerGroupCreate | 
try {
    val result : CustomerGroup = apiInstance.createCustomerGroup(customerGroupCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerGroupApi#createCustomerGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerGroupApi#createCustomerGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerGroupCreate** | [**CustomerGroupCreate**](CustomerGroupCreate.md)|  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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

<a id="deleteCustomerGroup"></a>
# **deleteCustomerGroup**
> deleteCustomerGroup(customerGroupId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerGroupApi()
val customerGroupId : kotlin.String = customerGroupId_example // kotlin.String | 
try {
    apiInstance.deleteCustomerGroup(customerGroupId)
} catch (e: ClientException) {
    println("4xx response calling CustomerGroupApi#deleteCustomerGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerGroupApi#deleteCustomerGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerGroupId** | **kotlin.String**|  | |

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

<a id="getCustomerGroup"></a>
# **getCustomerGroup**
> CustomerGroup getCustomerGroup(customerGroupId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerGroupApi()
val customerGroupId : kotlin.String = customerGroupId_example // kotlin.String | 
try {
    val result : CustomerGroup = apiInstance.getCustomerGroup(customerGroupId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerGroupApi#getCustomerGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerGroupApi#getCustomerGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerGroupId** | **kotlin.String**|  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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

<a id="listCustomerGroups"></a>
# **listCustomerGroups**
> kotlin.collections.List&lt;CustomerGroup&gt; listCustomerGroups(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerGroupApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<CustomerGroup> = apiInstance.listCustomerGroups(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerGroupApi#listCustomerGroups")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerGroupApi#listCustomerGroups")
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

[**kotlin.collections.List&lt;CustomerGroup&gt;**](CustomerGroup.md)

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

<a id="updateCustomerGroup"></a>
# **updateCustomerGroup**
> CustomerGroup updateCustomerGroup(customerGroupId, customerGroupUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CustomerGroupApi()
val customerGroupId : kotlin.String = customerGroupId_example // kotlin.String | 
val customerGroupUpdate : CustomerGroupUpdate =  // CustomerGroupUpdate | 
try {
    val result : CustomerGroup = apiInstance.updateCustomerGroup(customerGroupId, customerGroupUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CustomerGroupApi#updateCustomerGroup")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CustomerGroupApi#updateCustomerGroup")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerGroupId** | **kotlin.String**|  | |
| **customerGroupUpdate** | [**CustomerGroupUpdate**](CustomerGroupUpdate.md)|  | |

### Return type

[**CustomerGroup**](CustomerGroup.md)

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

