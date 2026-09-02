# GdprApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**acceptDpa**](GdprApi.md#acceptDpa) | **PUT** /api/v1/gdpr/dpa | Record DPA acceptance: sets dpa_accepted_at/by/version on the tenant settings row (created with company-type defaults if missing). |
| [**accountErasure**](GdprApi.md#accountErasure) | **POST** /api/v1/gdpr/account-erasure | Erase ALL personal data of the tenant (TOS §11: deletion 90 days after termination). |
| [**erasureContact**](GdprApi.md#erasureContact) | **POST** /api/v1/gdpr/erasure/{contact_id} | Anonymize + soft-delete a contact: personal attributes are cleared, the record itself is kept for GoBD retention (Art. 17(3)(e) DSGVO). The audit trigger on &#x60;contacts&#x60; already records who/when. |
| [**exportContactData**](GdprApi.md#exportContactData) | **GET** /api/v1/gdpr/export/{contact_id} | Art. 15 data-subject access export for a contact. |
| [**exportGdpr**](GdprApi.md#exportGdpr) | **GET** /api/v1/gdpr/export | Export the current user&#39;s personal data (GDPR Art. 15/20). |
| [**getDpa**](GdprApi.md#getDpa) | **GET** /api/v1/gdpr/dpa | Current DPA acceptance status (from tenant_settings). |


<a id="acceptDpa"></a>
# **acceptDpa**
> DpaStatus acceptDpa(dpaAcceptRequest)

Record DPA acceptance: sets dpa_accepted_at/by/version on the tenant settings row (created with company-type defaults if missing).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GdprApi()
val dpaAcceptRequest : DpaAcceptRequest =  // DpaAcceptRequest | 
try {
    val result : DpaStatus = apiInstance.acceptDpa(dpaAcceptRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GdprApi#acceptDpa")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GdprApi#acceptDpa")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **dpaAcceptRequest** | [**DpaAcceptRequest**](DpaAcceptRequest.md)|  | |

### Return type

[**DpaStatus**](DpaStatus.md)

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

<a id="accountErasure"></a>
# **accountErasure**
> kotlin.Any accountErasure()

Erase ALL personal data of the tenant (TOS §11: deletion 90 days after termination).

Anonymizes every contact, anonymizes personal fields on bookkeeping records (orders/invoices/payments keep amounts and dates for GoBD), removes the tenant linkage of the (global, saasy-framework) users and marks the erasure on &#x60;tenant_settings.gdpr_erased_at&#x60;. No row is physically deleted. The audit triggers on the touched tables record who/when.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GdprApi()
try {
    val result : kotlin.Any = apiInstance.accountErasure()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GdprApi#accountErasure")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GdprApi#accountErasure")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

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

<a id="erasureContact"></a>
# **erasureContact**
> kotlin.Any erasureContact(contactId)

Anonymize + soft-delete a contact: personal attributes are cleared, the record itself is kept for GoBD retention (Art. 17(3)(e) DSGVO). The audit trigger on &#x60;contacts&#x60; already records who/when.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GdprApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.erasureContact(contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GdprApi#erasureContact")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GdprApi#erasureContact")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |

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

<a id="exportContactData"></a>
# **exportContactData**
> kotlin.Any exportContactData(contactId)

Art. 15 data-subject access export for a contact.

Returns the contact itself plus the tenant-scoped rows linked to it.  ## Relations The &#x60;customers&#x60;/&#x60;orders&#x60;/&#x60;invoices&#x60;/&#x60;payments&#x60; tables have no FK to &#x60;contacts&#x60;; they are linked through the &#x60;customer_id&#x60; column, which per the app&#39;s conventions holds one of: - the admin customer&#39;s &#x60;customer_id&#x60; (a UUID, often the same value as   the contact&#39;s &#x60;contact_id&#x60;/&#x60;customer_number&#x60;), - the buyer&#39;s email for shop orders, or - the marketplace&#39;s external customer id for plugin orders.  The export therefore matches the contact&#39;s identifiers (&#x60;contact_id&#x60;, &#x60;customer_number&#x60;, &#x60;external_id&#x60;, &#x60;email&#x60;) plus any resolved customer ids against &#x60;customer_id&#x60;. &#x60;delivery_notes&#x60; and &#x60;customer_communications&#x60; reference contacts directly via &#x60;contact_id&#x60;. Soft-deleted rows are included (their data is still processed and retained for GoBD). Relations that genuinely do not exist for a contact stay empty but the key is always present.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GdprApi()
val contactId : kotlin.String = contactId_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.exportContactData(contactId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GdprApi#exportContactData")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GdprApi#exportContactData")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **contactId** | **kotlin.String**|  | |

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

<a id="exportGdpr"></a>
# **exportGdpr**
> ApiResponseGdprExport exportGdpr()

Export the current user&#39;s personal data (GDPR Art. 15/20).

No admin permission required: a user always exports their own data.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GdprApi()
try {
    val result : ApiResponseGdprExport = apiInstance.exportGdpr()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GdprApi#exportGdpr")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GdprApi#exportGdpr")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**ApiResponseGdprExport**](ApiResponseGdprExport.md)

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

<a id="getDpa"></a>
# **getDpa**
> DpaStatus getDpa()

Current DPA acceptance status (from tenant_settings).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = GdprApi()
try {
    val result : DpaStatus = apiInstance.getDpa()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling GdprApi#getDpa")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling GdprApi#getDpa")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**DpaStatus**](DpaStatus.md)

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

