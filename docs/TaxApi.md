# TaxApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createTaxRate**](TaxApi.md#createTaxRate) | **POST** /api/v1/tax-rates | Create a tax rate (&#x60;admin:settings&#x60;). |
| [**deleteTaxRate**](TaxApi.md#deleteTaxRate) | **DELETE** /api/v1/tax-rates/{id} | Delete a tax rate by id (&#x60;admin:settings&#x60;). |
| [**listTaxRates**](TaxApi.md#listTaxRates) | **GET** /api/v1/tax-rates | List the calling tenant&#39;s tax rates. |
| [**updateTaxRate**](TaxApi.md#updateTaxRate) | **PUT** /api/v1/tax-rates/{id} | Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields. |


<a id="createTaxRate"></a>
# **createTaxRate**
> createTaxRate(taxRateCreate)

Create a tax rate (&#x60;admin:settings&#x60;).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TaxApi()
val taxRateCreate : TaxRateCreate =  // TaxRateCreate | 
try {
    apiInstance.createTaxRate(taxRateCreate)
} catch (e: ClientException) {
    println("4xx response calling TaxApi#createTaxRate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaxApi#createTaxRate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **taxRateCreate** | [**TaxRateCreate**](TaxRateCreate.md)|  | |

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

<a id="deleteTaxRate"></a>
# **deleteTaxRate**
> deleteTaxRate(id)

Delete a tax rate by id (&#x60;admin:settings&#x60;).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TaxApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    apiInstance.deleteTaxRate(id)
} catch (e: ClientException) {
    println("4xx response calling TaxApi#deleteTaxRate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaxApi#deleteTaxRate")
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

<a id="listTaxRates"></a>
# **listTaxRates**
> listTaxRates()

List the calling tenant&#39;s tax rates.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TaxApi()
try {
    apiInstance.listTaxRates()
} catch (e: ClientException) {
    println("4xx response calling TaxApi#listTaxRates")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaxApi#listTaxRates")
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

<a id="updateTaxRate"></a>
# **updateTaxRate**
> updateTaxRate(id, taxRateCreate)

Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TaxApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val taxRateCreate : TaxRateCreate =  // TaxRateCreate | 
try {
    apiInstance.updateTaxRate(id, taxRateCreate)
} catch (e: ClientException) {
    println("4xx response calling TaxApi#updateTaxRate")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TaxApi#updateTaxRate")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **taxRateCreate** | [**TaxRateCreate**](TaxRateCreate.md)|  | |

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

