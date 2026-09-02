# CreateSepaDirectDebitApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createSepaDirectDebitApi**](CreateSepaDirectDebitApi.md#createSepaDirectDebitApi) | **POST** /api/v1/bookkeeping/sepa-direct-debit |  |


<a id="createSepaDirectDebitApi"></a>
# **createSepaDirectDebitApi**
> SepaDirectDebitResponse createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, creditorBic, debtorBic, description)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CreateSepaDirectDebitApi()
val creditorName : kotlin.String = creditorName_example // kotlin.String | 
val creditorIban : kotlin.String = creditorIban_example // kotlin.String | 
val creditorId : kotlin.String = creditorId_example // kotlin.String | 
val mandateId : kotlin.String = mandateId_example // kotlin.String | 
val mandateDate : kotlin.String = mandateDate_example // kotlin.String | 
val debtorName : kotlin.String = debtorName_example // kotlin.String | 
val debtorIban : kotlin.String = debtorIban_example // kotlin.String | 
val amount : kotlin.String = amount_example // kotlin.String | 
val collectionDate : kotlin.String = collectionDate_example // kotlin.String | 
val creditorBic : kotlin.String = creditorBic_example // kotlin.String | 
val debtorBic : kotlin.String = debtorBic_example // kotlin.String | 
val description : kotlin.String = description_example // kotlin.String | 
try {
    val result : SepaDirectDebitResponse = apiInstance.createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, creditorBic, debtorBic, description)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CreateSepaDirectDebitApi#createSepaDirectDebitApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CreateSepaDirectDebitApi#createSepaDirectDebitApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **creditorName** | **kotlin.String**|  | |
| **creditorIban** | **kotlin.String**|  | |
| **creditorId** | **kotlin.String**|  | |
| **mandateId** | **kotlin.String**|  | |
| **mandateDate** | **kotlin.String**|  | |
| **debtorName** | **kotlin.String**|  | |
| **debtorIban** | **kotlin.String**|  | |
| **amount** | **kotlin.String**|  | |
| **collectionDate** | **kotlin.String**|  | |
| **creditorBic** | **kotlin.String**|  | [optional] |
| **debtorBic** | **kotlin.String**|  | [optional] |
| **description** | **kotlin.String**|  | [optional] |

### Return type

[**SepaDirectDebitResponse**](SepaDirectDebitResponse.md)

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

