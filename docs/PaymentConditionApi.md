# PaymentConditionApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**listPaymentConditionsApi**](PaymentConditionApi.md#listPaymentConditionsApi) | **GET** /api/v1/payment-conditions |  |


<a id="listPaymentConditionsApi"></a>
# **listPaymentConditionsApi**
> kotlin.collections.List&lt;PaymentCondition&gt; listPaymentConditionsApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PaymentConditionApi()
try {
    val result : kotlin.collections.List<PaymentCondition> = apiInstance.listPaymentConditionsApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PaymentConditionApi#listPaymentConditionsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PaymentConditionApi#listPaymentConditionsApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PaymentCondition&gt;**](PaymentCondition.md)

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

