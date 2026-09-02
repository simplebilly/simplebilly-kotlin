# BookkeepingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**allocatePaymentApi**](BookkeepingApi.md#allocatePaymentApi) | **POST** /api/v1/payments/allocate | Allocate a payment to an invoice |
| [**bwaReportApi**](BookkeepingApi.md#bwaReportApi) | **GET** /api/v1/bookkeeping/bwa | Get BWA (Betriebswirtschaftliche Auswertung) report |
| [**elsterStatusApi**](BookkeepingApi.md#elsterStatusApi) | **GET** /api/v1/bookkeeping/elster/status |  |
| [**elsterValidateApi**](BookkeepingApi.md#elsterValidateApi) | **POST** /api/v1/bookkeeping/ustva/elster-validate |  |
| [**elsterXmlApi**](BookkeepingApi.md#elsterXmlApi) | **GET** /api/v1/bookkeeping/ustva/elster-xml |  |
| [**getCashflow**](BookkeepingApi.md#getCashflow) | **GET** /api/v1/bookkeeping/cashflow | GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period. |
| [**getLiquidity**](BookkeepingApi.md#getLiquidity) | **GET** /api/v1/bookkeeping/liquidity | GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios. |
| [**getOpenInvoicesApi**](BookkeepingApi.md#getOpenInvoicesApi) | **GET** /api/v1/payments/open-invoices/{customer_id} | Get open invoices for a customer |
| [**getVerfahrensdokumentation**](BookkeepingApi.md#getVerfahrensdokumentation) | **GET** /api/v1/bookkeeping/verfahrensdokumentation | GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules. |
| [**runDunningApi**](BookkeepingApi.md#runDunningApi) | **POST** /api/v1/bookkeeping/dunning |  |


<a id="allocatePaymentApi"></a>
# **allocatePaymentApi**
> allocatePaymentApi(allocatePaymentRequest)

Allocate a payment to an invoice

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
val allocatePaymentRequest : AllocatePaymentRequest =  // AllocatePaymentRequest | 
try {
    apiInstance.allocatePaymentApi(allocatePaymentRequest)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#allocatePaymentApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#allocatePaymentApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **allocatePaymentRequest** | [**AllocatePaymentRequest**](AllocatePaymentRequest.md)|  | |

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

 - **Content-Type**: application/json
 - **Accept**: application/json

<a id="bwaReportApi"></a>
# **bwaReportApi**
> BWAReport bwaReportApi(year, month)

Get BWA (Betriebswirtschaftliche Auswertung) report

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BWAReport = apiInstance.bwaReportApi(year, month)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#bwaReportApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#bwaReportApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **month** | **kotlin.Int**|  | [optional] |

### Return type

[**BWAReport**](BWAReport.md)

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

<a id="elsterStatusApi"></a>
# **elsterStatusApi**
> ElsterStatus elsterStatusApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
try {
    val result : ElsterStatus = apiInstance.elsterStatusApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#elsterStatusApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#elsterStatusApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ElsterStatus**](ElsterStatus.md)

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

<a id="elsterValidateApi"></a>
# **elsterValidateApi**
> elsterValidateApi(zeitraum)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
val zeitraum : kotlin.String = zeitraum_example // kotlin.String | 
try {
    apiInstance.elsterValidateApi(zeitraum)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#elsterValidateApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#elsterValidateApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zeitraum** | **kotlin.String**|  | |

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

<a id="elsterXmlApi"></a>
# **elsterXmlApi**
> elsterXmlApi(zeitraum)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
val zeitraum : kotlin.String = zeitraum_example // kotlin.String | 
try {
    apiInstance.elsterXmlApi(zeitraum)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#elsterXmlApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#elsterXmlApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **zeitraum** | **kotlin.String**|  | |

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

<a id="getCashflow"></a>
# **getCashflow**
> CashflowReport getCashflow(year, month)

GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : CashflowReport = apiInstance.getCashflow(year, month)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#getCashflow")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#getCashflow")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | [optional] |
| **month** | **kotlin.Int**|  | [optional] |

### Return type

[**CashflowReport**](CashflowReport.md)

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

<a id="getLiquidity"></a>
# **getLiquidity**
> LiquidityPosition getLiquidity()

GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
try {
    val result : LiquidityPosition = apiInstance.getLiquidity()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#getLiquidity")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#getLiquidity")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**LiquidityPosition**](LiquidityPosition.md)

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

<a id="getOpenInvoicesApi"></a>
# **getOpenInvoicesApi**
> kotlin.collections.List&lt;Invoice&gt; getOpenInvoicesApi(customerId)

Get open invoices for a customer

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
val customerId : kotlin.String = customerId_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Invoice> = apiInstance.getOpenInvoicesApi(customerId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#getOpenInvoicesApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#getOpenInvoicesApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **customerId** | **kotlin.String**|  | |

### Return type

[**kotlin.collections.List&lt;Invoice&gt;**](Invoice.md)

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

<a id="getVerfahrensdokumentation"></a>
# **getVerfahrensdokumentation**
> Verfahrensdokumentation getVerfahrensdokumentation()

GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
try {
    val result : Verfahrensdokumentation = apiInstance.getVerfahrensdokumentation()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#getVerfahrensdokumentation")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#getVerfahrensdokumentation")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**Verfahrensdokumentation**](Verfahrensdokumentation.md)

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

<a id="runDunningApi"></a>
# **runDunningApi**
> DunningResult runDunningApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BookkeepingApi()
try {
    val result : DunningResult = apiInstance.runDunningApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BookkeepingApi#runDunningApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BookkeepingApi#runDunningApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**DunningResult**](DunningResult.md)

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

