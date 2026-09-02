# EmployeeApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createEmployee**](EmployeeApi.md#createEmployee) | **POST** /api/v1/employees |  |
| [**deleteEmployee**](EmployeeApi.md#deleteEmployee) | **DELETE** /api/v1/employees/{id} |  |
| [**employeeRestore**](EmployeeApi.md#employeeRestore) | **POST** /api/v1/employees/{id}/restore |  |
| [**getEmployee**](EmployeeApi.md#getEmployee) | **GET** /api/v1/employees/{id} |  |
| [**getEmployeePayrollSummary**](EmployeeApi.md#getEmployeePayrollSummary) | **GET** /api/v1/employees/{id}/payroll-summary |  |
| [**getEmployees**](EmployeeApi.md#getEmployees) | **GET** /api/v1/employees/ |  |
| [**updateEmployee**](EmployeeApi.md#updateEmployee) | **PUT** /api/v1/employees/{id} |  |


<a id="createEmployee"></a>
# **createEmployee**
> Employee createEmployee(employeeCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val employeeCreate : EmployeeCreate =  // EmployeeCreate | 
try {
    val result : Employee = apiInstance.createEmployee(employeeCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#createEmployee")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#createEmployee")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **employeeCreate** | [**EmployeeCreate**](EmployeeCreate.md)|  | |

### Return type

[**Employee**](Employee.md)

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

<a id="deleteEmployee"></a>
# **deleteEmployee**
> deleteEmployee(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteEmployee(id)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#deleteEmployee")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#deleteEmployee")
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

<a id="employeeRestore"></a>
# **employeeRestore**
> Employee employeeRestore(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Employee = apiInstance.employeeRestore(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#employeeRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#employeeRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Employee**](Employee.md)

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

<a id="getEmployee"></a>
# **getEmployee**
> Employee getEmployee(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : Employee = apiInstance.getEmployee(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#getEmployee")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#getEmployee")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**Employee**](Employee.md)

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

<a id="getEmployeePayrollSummary"></a>
# **getEmployeePayrollSummary**
> PayrollSummary getEmployeePayrollSummary(id, year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val year : kotlin.Int = 56 // kotlin.Int | Fiscal year for the breakdown; defaults to the current year.
try {
    val result : PayrollSummary = apiInstance.getEmployeePayrollSummary(id, year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#getEmployeePayrollSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#getEmployeePayrollSummary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **year** | **kotlin.Int**| Fiscal year for the breakdown; defaults to the current year. | [optional] |

### Return type

[**PayrollSummary**](PayrollSummary.md)

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

<a id="getEmployees"></a>
# **getEmployees**
> kotlin.collections.List&lt;Employee&gt; getEmployees(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Employee> = apiInstance.getEmployees(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#getEmployees")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#getEmployees")
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

[**kotlin.collections.List&lt;Employee&gt;**](Employee.md)

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

<a id="updateEmployee"></a>
# **updateEmployee**
> Employee updateEmployee(id, employeeUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = EmployeeApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val employeeUpdate : EmployeeUpdate =  // EmployeeUpdate | 
try {
    val result : Employee = apiInstance.updateEmployee(id, employeeUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling EmployeeApi#updateEmployee")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling EmployeeApi#updateEmployee")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **employeeUpdate** | [**EmployeeUpdate**](EmployeeUpdate.md)|  | |

### Return type

[**Employee**](Employee.md)

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

