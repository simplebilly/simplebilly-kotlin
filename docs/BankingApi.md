# BankingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**bankLookupApi**](BankingApi.md#bankLookupApi) | **GET** /api/v1/bookkeeping/banking/lookup |  |
| [**bankTransactionsApi**](BankingApi.md#bankTransactionsApi) | **GET** /api/v1/bookkeeping/banking/transactions |  |
| [**hebesatzLookupApi**](BankingApi.md#hebesatzLookupApi) | **GET** /api/v1/bookkeeping/hebesatz |  |


<a id="bankLookupApi"></a>
# **bankLookupApi**
> BankLookup bankLookupApi(iban)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BankingApi()
val iban : kotlin.String = iban_example // kotlin.String | 
try {
    val result : BankLookup = apiInstance.bankLookupApi(iban)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BankingApi#bankLookupApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BankingApi#bankLookupApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **iban** | **kotlin.String**|  | |

### Return type

[**BankLookup**](BankLookup.md)

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

<a id="bankTransactionsApi"></a>
# **bankTransactionsApi**
> bankTransactionsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BankingApi()
try {
    apiInstance.bankTransactionsApi()
} catch (e: ClientException) {
    println("4xx response calling BankingApi#bankTransactionsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BankingApi#bankTransactionsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="hebesatzLookupApi"></a>
# **hebesatzLookupApi**
> kotlin.collections.List&lt;HebesatzLookup&gt; hebesatzLookupApi(gemeindeschluessel, plz, name, stichtag, countryCode)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BankingApi()
val gemeindeschluessel : kotlin.String = gemeindeschluessel_example // kotlin.String | 
val plz : kotlin.String = plz_example // kotlin.String | 
val name : kotlin.String = name_example // kotlin.String | 
val stichtag : kotlin.String = stichtag_example // kotlin.String | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from <= date <= valid_to.
val countryCode : kotlin.String = countryCode_example // kotlin.String | 
try {
    val result : kotlin.collections.List<HebesatzLookup> = apiInstance.hebesatzLookupApi(gemeindeschluessel, plz, name, stichtag, countryCode)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BankingApi#hebesatzLookupApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BankingApi#hebesatzLookupApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **gemeindeschluessel** | **kotlin.String**|  | [optional] |
| **plz** | **kotlin.String**|  | [optional] |
| **name** | **kotlin.String**|  | [optional] |
| **stichtag** | **kotlin.String**| Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from &lt;&#x3D; date &lt;&#x3D; valid_to. | [optional] |
| **countryCode** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;HebesatzLookup&gt;**](HebesatzLookup.md)

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

