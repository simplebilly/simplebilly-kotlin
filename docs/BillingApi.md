# BillingApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**getPlans**](BillingApi.md#getPlans) | **GET** /api/v1/plans | All canonical plans (free/starter/business/enterprise) — the single source of truth lives in &#x60;crate::saasy::plans&#x60;, matching marketing. |
| [**getQuotaApi**](BillingApi.md#getQuotaApi) | **GET** /api/v1/quota | Effective limits + current usage for the calling tenant. |
| [**getSubscriptionApi**](BillingApi.md#getSubscriptionApi) | **GET** /api/v1/subscription |  |
| [**getUsageApi**](BillingApi.md#getUsageApi) | **GET** /api/v1/usage |  |
| [**paddleSubscriptionWebhook**](BillingApi.md#paddleSubscriptionWebhook) | **POST** /api/webhooks/paddle/subscription | Paddle Billing subscription webhook. Verifies the &#x60;Paddle-Signature&#x60; header (HMAC-SHA256 over &#x60;\&quot;{ts}:{raw_body}\&quot;&#x60; with the webhook secret), then updates &#x60;billing_info&#x60; and &#x60;tenants.plan&#x60; for the tenant identified by the subscription &#x60;custom_data&#x60; (JSON &#x60;{\&quot;tenant_id\&quot;: \&quot;...\&quot;}&#x60; or a bare tenant UUID). |
| [**putQuotaApi**](BillingApi.md#putQuotaApi) | **PUT** /api/v1/quota | Write the per-tenant quota override (&#x60;admin:settings&#x60;). An empty object clears the override. |


<a id="getPlans"></a>
# **getPlans**
> ApiResponseVecPlan getPlans()

All canonical plans (free/starter/business/enterprise) — the single source of truth lives in &#x60;crate::saasy::plans&#x60;, matching marketing.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BillingApi()
try {
    val result : ApiResponseVecPlan = apiInstance.getPlans()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#getPlans")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#getPlans")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseVecPlan**](ApiResponseVecPlan.md)

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

<a id="getQuotaApi"></a>
# **getQuotaApi**
> getQuotaApi()

Effective limits + current usage for the calling tenant.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BillingApi()
try {
    apiInstance.getQuotaApi()
} catch (e: ClientException) {
    println("4xx response calling BillingApi#getQuotaApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#getQuotaApi")
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

<a id="getSubscriptionApi"></a>
# **getSubscriptionApi**
> ApiResponseSubscriptionOverview getSubscriptionApi()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BillingApi()
try {
    val result : ApiResponseSubscriptionOverview = apiInstance.getSubscriptionApi()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#getSubscriptionApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#getSubscriptionApi")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseSubscriptionOverview**](ApiResponseSubscriptionOverview.md)

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

<a id="getUsageApi"></a>
# **getUsageApi**
> getUsageApi(meter)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BillingApi()
val meter : kotlin.String = meter_example // kotlin.String | 
try {
    apiInstance.getUsageApi(meter)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#getUsageApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#getUsageApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **meter** | **kotlin.String**|  | [optional] |

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

<a id="paddleSubscriptionWebhook"></a>
# **paddleSubscriptionWebhook**
> paddleSubscriptionWebhook()

Paddle Billing subscription webhook. Verifies the &#x60;Paddle-Signature&#x60; header (HMAC-SHA256 over &#x60;\&quot;{ts}:{raw_body}\&quot;&#x60; with the webhook secret), then updates &#x60;billing_info&#x60; and &#x60;tenants.plan&#x60; for the tenant identified by the subscription &#x60;custom_data&#x60; (JSON &#x60;{\&quot;tenant_id\&quot;: \&quot;...\&quot;}&#x60; or a bare tenant UUID).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BillingApi()
try {
    apiInstance.paddleSubscriptionWebhook()
} catch (e: ClientException) {
    println("4xx response calling BillingApi#paddleSubscriptionWebhook")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#paddleSubscriptionWebhook")
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

<a id="putQuotaApi"></a>
# **putQuotaApi**
> putQuotaApi(quotaOverride)

Write the per-tenant quota override (&#x60;admin:settings&#x60;). An empty object clears the override.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BillingApi()
val quotaOverride : QuotaOverride =  // QuotaOverride | 
try {
    apiInstance.putQuotaApi(quotaOverride)
} catch (e: ClientException) {
    println("4xx response calling BillingApi#putQuotaApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BillingApi#putQuotaApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **quotaOverride** | [**QuotaOverride**](QuotaOverride.md)|  | |

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
 - **Accept**: Not defined

