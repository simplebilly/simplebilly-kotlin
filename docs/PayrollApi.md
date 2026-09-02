# PayrollApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**payrollApprove**](PayrollApi.md#payrollApprove) | **POST** /api/v1/payroll/{id}/approve |  |
| [**payrollAutopay**](PayrollApi.md#payrollAutopay) | **POST** /api/v1/payroll/{id}/autopay |  |
| [**payrollCalculate**](PayrollApi.md#payrollCalculate) | **POST** /api/v1/payroll/{id}/calculate |  |
| [**payrollCreate**](PayrollApi.md#payrollCreate) | **POST** /api/v1/payroll |  |
| [**payrollDelete**](PayrollApi.md#payrollDelete) | **DELETE** /api/v1/payroll/{id} |  |
| [**payrollElsterExport**](PayrollApi.md#payrollElsterExport) | **POST** /api/v1/payroll/{id}/elster-export |  |
| [**payrollEmail**](PayrollApi.md#payrollEmail) | **POST** /api/v1/payroll/{id}/email |  |
| [**payrollEntryPdf**](PayrollApi.md#payrollEntryPdf) | **GET** /api/v1/payroll/{id}/entries/{entry_id}/pdf |  |
| [**payrollGet**](PayrollApi.md#payrollGet) | **GET** /api/v1/payroll/{id} |  |
| [**payrollList**](PayrollApi.md#payrollList) | **GET** /api/v1/payroll |  |
| [**payrollPay**](PayrollApi.md#payrollPay) | **POST** /api/v1/payroll/{id}/pay |  |
| [**payrollPdf**](PayrollApi.md#payrollPdf) | **GET** /api/v1/payroll/{id}/pdf |  |
| [**payrollSummary**](PayrollApi.md#payrollSummary) | **GET** /api/v1/payroll/summary/{year} |  |
| [**payrollSvMeldungen**](PayrollApi.md#payrollSvMeldungen) | **POST** /api/v1/payroll/{id}/sv-meldungen |  |


<a id="payrollApprove"></a>
# **payrollApprove**
> PayrollRunApi payrollApprove(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : PayrollRunApi = apiInstance.payrollApprove(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollApprove")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollApprove")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

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

<a id="payrollAutopay"></a>
# **payrollAutopay**
> kotlin.Any payrollAutopay(id, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : kotlin.String = id_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.payrollAutopay(id, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollAutopay")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollAutopay")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | [optional] |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="payrollCalculate"></a>
# **payrollCalculate**
> PayrollRunApi payrollCalculate(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : PayrollRunApi = apiInstance.payrollCalculate(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollCalculate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollCalculate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

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

<a id="payrollCreate"></a>
# **payrollCreate**
> PayrollRunApi payrollCreate(payrollCreatePayload)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val payrollCreatePayload : PayrollCreatePayload =  // PayrollCreatePayload | 
try {
    val result : PayrollRunApi = apiInstance.payrollCreate(payrollCreatePayload)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollCreate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollCreate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **payrollCreatePayload** | [**PayrollCreatePayload**](PayrollCreatePayload.md)|  | |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

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

<a id="payrollDelete"></a>
# **payrollDelete**
> payrollDelete(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.payrollDelete(id)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollDelete")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollDelete")
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
 - **Accept**: Not defined

<a id="payrollElsterExport"></a>
# **payrollElsterExport**
> payrollElsterExport(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.payrollElsterExport(id)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollElsterExport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollElsterExport")
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
 - **Accept**: Not defined

<a id="payrollEmail"></a>
# **payrollEmail**
> kotlin.Any payrollEmail(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.payrollEmail(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollEmail")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollEmail")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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

<a id="payrollEntryPdf"></a>
# **payrollEntryPdf**
> payrollEntryPdf(id, entryId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : kotlin.String = id_example // kotlin.String | 
val entryId : kotlin.String = entryId_example // kotlin.String | 
try {
    apiInstance.payrollEntryPdf(id, entryId)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollEntryPdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollEntryPdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |
| **entryId** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="payrollGet"></a>
# **payrollGet**
> PayrollRunApi payrollGet(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : PayrollRunApi = apiInstance.payrollGet(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollGet")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollGet")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

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

<a id="payrollList"></a>
# **payrollList**
> kotlin.collections.List&lt;PayrollRunApi&gt; payrollList(year, status)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val status : kotlin.String = status_example // kotlin.String | 
try {
    val result : kotlin.collections.List<PayrollRunApi> = apiInstance.payrollList(year, status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollList")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollList")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **status** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;PayrollRunApi&gt;**](PayrollRunApi.md)

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

<a id="payrollPay"></a>
# **payrollPay**
> PayrollRunApi payrollPay(id, payrollPayPayload)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val payrollPayPayload : PayrollPayPayload =  // PayrollPayPayload | 
try {
    val result : PayrollRunApi = apiInstance.payrollPay(id, payrollPayPayload)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollPay")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollPay")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **payrollPayPayload** | [**PayrollPayPayload**](PayrollPayPayload.md)|  | |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

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

<a id="payrollPdf"></a>
# **payrollPdf**
> payrollPdf(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : kotlin.String = id_example // kotlin.String | 
try {
    apiInstance.payrollPdf(id)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollPdf")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollPdf")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **kotlin.String**|  | |

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
 - **Accept**: Not defined

<a id="payrollSummary"></a>
# **payrollSummary**
> YearlyPayrollSummary payrollSummary(year)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val year : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : YearlyPayrollSummary = apiInstance.payrollSummary(year)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollSummary")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollSummary")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |

### Return type

[**YearlyPayrollSummary**](YearlyPayrollSummary.md)

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

<a id="payrollSvMeldungen"></a>
# **payrollSvMeldungen**
> kotlin.Any payrollSvMeldungen(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PayrollApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.Any = apiInstance.payrollSvMeldungen(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PayrollApi#payrollSvMeldungen")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PayrollApi#payrollSvMeldungen")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

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

