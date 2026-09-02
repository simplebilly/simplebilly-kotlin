# VoucherApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createVoucher**](VoucherApi.md#createVoucher) | **POST** /api/v1/vouchers |  |
| [**deleteVoucher**](VoucherApi.md#deleteVoucher) | **DELETE** /api/v1/vouchers/{voucher_id} |  |
| [**getVoucher**](VoucherApi.md#getVoucher) | **GET** /api/v1/vouchers/{voucher_id} |  |
| [**listVouchers**](VoucherApi.md#listVouchers) | **GET** /api/v1/vouchers/ |  |
| [**updateVoucher**](VoucherApi.md#updateVoucher) | **PUT** /api/v1/vouchers/{voucher_id} |  |
| [**voucherRestore**](VoucherApi.md#voucherRestore) | **POST** /api/v1/vouchers/{voucher_id}/restore |  |


<a id="createVoucher"></a>
# **createVoucher**
> Voucher createVoucher(voucherCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = VoucherApi()
val voucherCreate : VoucherCreate =  // VoucherCreate | 
try {
    val result : Voucher = apiInstance.createVoucher(voucherCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VoucherApi#createVoucher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VoucherApi#createVoucher")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **voucherCreate** | [**VoucherCreate**](VoucherCreate.md)|  | |

### Return type

[**Voucher**](Voucher.md)

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

<a id="deleteVoucher"></a>
# **deleteVoucher**
> deleteVoucher(voucherId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = VoucherApi()
val voucherId : kotlin.String = voucherId_example // kotlin.String | 
try {
    apiInstance.deleteVoucher(voucherId)
} catch (e: ClientException) {
    println("4xx response calling VoucherApi#deleteVoucher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VoucherApi#deleteVoucher")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **voucherId** | **kotlin.String**|  | |

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

<a id="getVoucher"></a>
# **getVoucher**
> Voucher getVoucher(voucherId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = VoucherApi()
val voucherId : kotlin.String = voucherId_example // kotlin.String | 
try {
    val result : Voucher = apiInstance.getVoucher(voucherId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VoucherApi#getVoucher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VoucherApi#getVoucher")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **voucherId** | **kotlin.String**|  | |

### Return type

[**Voucher**](Voucher.md)

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

<a id="listVouchers"></a>
# **listVouchers**
> kotlin.collections.List&lt;Voucher&gt; listVouchers(page, pageSize, voucherType, voucherStatus, contactName, dateFrom, dateTo)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = VoucherApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val voucherType : kotlin.String = voucherType_example // kotlin.String | 
val voucherStatus : kotlin.String = voucherStatus_example // kotlin.String | 
val contactName : kotlin.String = contactName_example // kotlin.String | 
val dateFrom : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val dateTo : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
try {
    val result : kotlin.collections.List<Voucher> = apiInstance.listVouchers(page, pageSize, voucherType, voucherStatus, contactName, dateFrom, dateTo)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VoucherApi#listVouchers")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VoucherApi#listVouchers")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **voucherType** | **kotlin.String**|  | [optional] |
| **voucherStatus** | **kotlin.String**|  | [optional] |
| **contactName** | **kotlin.String**|  | [optional] |
| **dateFrom** | **java.time.LocalDate**|  | [optional] |
| **dateTo** | **java.time.LocalDate**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Voucher&gt;**](Voucher.md)

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

<a id="updateVoucher"></a>
# **updateVoucher**
> Voucher updateVoucher(voucherId, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = VoucherApi()
val voucherId : kotlin.String = voucherId_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : Voucher = apiInstance.updateVoucher(voucherId, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VoucherApi#updateVoucher")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VoucherApi#updateVoucher")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **voucherId** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

### Return type

[**Voucher**](Voucher.md)

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

<a id="voucherRestore"></a>
# **voucherRestore**
> Voucher voucherRestore(voucherId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = VoucherApi()
val voucherId : kotlin.String = voucherId_example // kotlin.String | 
try {
    val result : Voucher = apiInstance.voucherRestore(voucherId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling VoucherApi#voucherRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling VoucherApi#voucherRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **voucherId** | **kotlin.String**|  | |

### Return type

[**Voucher**](Voucher.md)

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

