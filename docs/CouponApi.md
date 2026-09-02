# CouponApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**couponRestore**](CouponApi.md#couponRestore) | **POST** /api/v1/coupons/{coupon_id}/restore |  |
| [**createCoupon**](CouponApi.md#createCoupon) | **POST** /api/v1/coupons |  |
| [**deleteCoupon**](CouponApi.md#deleteCoupon) | **DELETE** /api/v1/coupons/{coupon_id} |  |
| [**getCoupon**](CouponApi.md#getCoupon) | **GET** /api/v1/coupons/{coupon_id} |  |
| [**listCoupons**](CouponApi.md#listCoupons) | **GET** /api/v1/coupons/ |  |
| [**updateCoupon**](CouponApi.md#updateCoupon) | **PUT** /api/v1/coupons/{coupon_id} |  |


<a id="couponRestore"></a>
# **couponRestore**
> Coupon couponRestore(couponId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CouponApi()
val couponId : kotlin.String = couponId_example // kotlin.String | 
try {
    val result : Coupon = apiInstance.couponRestore(couponId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CouponApi#couponRestore")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CouponApi#couponRestore")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **couponId** | **kotlin.String**|  | |

### Return type

[**Coupon**](Coupon.md)

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

<a id="createCoupon"></a>
# **createCoupon**
> Coupon createCoupon(couponCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CouponApi()
val couponCreate : CouponCreate =  // CouponCreate | 
try {
    val result : Coupon = apiInstance.createCoupon(couponCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CouponApi#createCoupon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CouponApi#createCoupon")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **couponCreate** | [**CouponCreate**](CouponCreate.md)|  | |

### Return type

[**Coupon**](Coupon.md)

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

<a id="deleteCoupon"></a>
# **deleteCoupon**
> deleteCoupon(couponId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CouponApi()
val couponId : kotlin.String = couponId_example // kotlin.String | 
try {
    apiInstance.deleteCoupon(couponId)
} catch (e: ClientException) {
    println("4xx response calling CouponApi#deleteCoupon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CouponApi#deleteCoupon")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **couponId** | **kotlin.String**|  | |

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

<a id="getCoupon"></a>
# **getCoupon**
> Coupon getCoupon(couponId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CouponApi()
val couponId : kotlin.String = couponId_example // kotlin.String | 
try {
    val result : Coupon = apiInstance.getCoupon(couponId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CouponApi#getCoupon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CouponApi#getCoupon")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **couponId** | **kotlin.String**|  | |

### Return type

[**Coupon**](Coupon.md)

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

<a id="listCoupons"></a>
# **listCoupons**
> kotlin.collections.List&lt;Coupon&gt; listCoupons(page, pageSize, isActive, code, discountType)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CouponApi()
val page : kotlin.Int = 56 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val isActive : kotlin.Boolean = true // kotlin.Boolean | 
val code : kotlin.String = code_example // kotlin.String | 
val discountType : kotlin.String = discountType_example // kotlin.String | 
try {
    val result : kotlin.collections.List<Coupon> = apiInstance.listCoupons(page, pageSize, isActive, code, discountType)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CouponApi#listCoupons")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CouponApi#listCoupons")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **isActive** | **kotlin.Boolean**|  | [optional] |
| **code** | **kotlin.String**|  | [optional] |
| **discountType** | **kotlin.String**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;Coupon&gt;**](Coupon.md)

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

<a id="updateCoupon"></a>
# **updateCoupon**
> Coupon updateCoupon(couponId, couponUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = CouponApi()
val couponId : kotlin.String = couponId_example // kotlin.String | 
val couponUpdate : CouponUpdate =  // CouponUpdate | 
try {
    val result : Coupon = apiInstance.updateCoupon(couponId, couponUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling CouponApi#updateCoupon")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling CouponApi#updateCoupon")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **couponId** | **kotlin.String**|  | |
| **couponUpdate** | [**CouponUpdate**](CouponUpdate.md)|  | |

### Return type

[**Coupon**](Coupon.md)

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

