# PosApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**posBilling**](PosApi.md#posBilling) | **GET** /api/pos/billing |  |
| [**posCreateOrder**](PosApi.md#posCreateOrder) | **POST** /api/pos/orders |  |
| [**posCreateRegister**](PosApi.md#posCreateRegister) | **POST** /api/pos/registers |  |
| [**posCreateTable**](PosApi.md#posCreateTable) | **POST** /api/pos/tables |  |
| [**posDisableRegister**](PosApi.md#posDisableRegister) | **POST** /api/pos/registers/{id}/disable |  |
| [**posFreeTable**](PosApi.md#posFreeTable) | **POST** /api/pos/tables/{id}/free |  |
| [**posKasseClosing**](PosApi.md#posKasseClosing) | **POST** /api/pos/kasse/closing |  |
| [**posKasseEntries**](PosApi.md#posKasseEntries) | **GET** /api/pos/kasse/entries |  |
| [**posKasseExport**](PosApi.md#posKasseExport) | **GET** /api/pos/kasse/export |  |
| [**posKassePayInOut**](PosApi.md#posKassePayInOut) | **POST** /api/pos/kasse/pay-in-out |  |
| [**posListOrders**](PosApi.md#posListOrders) | **GET** /api/pos/orders |  |
| [**posListProducts**](PosApi.md#posListProducts) | **GET** /api/pos/products |  |
| [**posListRegisters**](PosApi.md#posListRegisters) | **GET** /api/pos/registers |  |
| [**posListTables**](PosApi.md#posListTables) | **GET** /api/pos/tables |  |
| [**posOrderPrint**](PosApi.md#posOrderPrint) | **GET** /api/pos/orders/{order_number}/print |  |
| [**posOrderReceipt**](PosApi.md#posOrderReceipt) | **GET** /api/pos/orders/{order_number}/receipt |  |
| [**posPayOrder**](PosApi.md#posPayOrder) | **POST** /api/pos/orders/{order_number}/pay |  |
| [**posSumupCheckout**](PosApi.md#posSumupCheckout) | **POST** /api/pos/sumup/checkout |  |


<a id="posBilling"></a>
# **posBilling**
> kotlin.Any posBilling()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
try {
    val result : kotlin.Any = apiInstance.posBilling()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posBilling")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posBilling")
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

<a id="posCreateOrder"></a>
# **posCreateOrder**
> kotlin.Any posCreateOrder(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.posCreateOrder(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posCreateOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posCreateOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="posCreateRegister"></a>
# **posCreateRegister**
> PosRegister posCreateRegister(posRegisterCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val posRegisterCreate : PosRegisterCreate =  // PosRegisterCreate | 
try {
    val result : PosRegister = apiInstance.posCreateRegister(posRegisterCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posCreateRegister")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posCreateRegister")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **posRegisterCreate** | [**PosRegisterCreate**](PosRegisterCreate.md)|  | |

### Return type

[**PosRegister**](PosRegister.md)

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

<a id="posCreateTable"></a>
# **posCreateTable**
> PosTable posCreateTable(posTableCreate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val posTableCreate : PosTableCreate =  // PosTableCreate | 
try {
    val result : PosTable = apiInstance.posCreateTable(posTableCreate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posCreateTable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posCreateTable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **posTableCreate** | [**PosTableCreate**](PosTableCreate.md)|  | |

### Return type

[**PosTable**](PosTable.md)

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

<a id="posDisableRegister"></a>
# **posDisableRegister**
> PosRegister posDisableRegister(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : PosRegister = apiInstance.posDisableRegister(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posDisableRegister")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posDisableRegister")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**PosRegister**](PosRegister.md)

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

<a id="posFreeTable"></a>
# **posFreeTable**
> PosTable posFreeTable(id)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : PosTable = apiInstance.posFreeTable(id)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posFreeTable")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posFreeTable")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |

### Return type

[**PosTable**](PosTable.md)

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

<a id="posKasseClosing"></a>
# **posKasseClosing**
> kotlin.Any posKasseClosing(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.posKasseClosing(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posKasseClosing")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posKasseClosing")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="posKasseEntries"></a>
# **posKasseEntries**
> kotlin.Any posKasseEntries()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
try {
    val result : kotlin.Any = apiInstance.posKasseEntries()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posKasseEntries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posKasseEntries")
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

<a id="posKasseExport"></a>
# **posKasseExport**
> kotlin.Any posKasseExport()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
try {
    val result : kotlin.Any = apiInstance.posKasseExport()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posKasseExport")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posKasseExport")
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

<a id="posKassePayInOut"></a>
# **posKassePayInOut**
> kotlin.Any posKassePayInOut(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.posKassePayInOut(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posKassePayInOut")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posKassePayInOut")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

<a id="posListOrders"></a>
# **posListOrders**
> kotlin.Any posListOrders(status)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val status : kotlin.String = status_example // kotlin.String | Filter by order status
try {
    val result : kotlin.Any = apiInstance.posListOrders(status)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posListOrders")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posListOrders")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **status** | **kotlin.String**| Filter by order status | [optional] |

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

<a id="posListProducts"></a>
# **posListProducts**
> kotlin.Any posListProducts(q)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val q : kotlin.String = q_example // kotlin.String | Product search
try {
    val result : kotlin.Any = apiInstance.posListProducts(q)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posListProducts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posListProducts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **q** | **kotlin.String**| Product search | [optional] |

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

<a id="posListRegisters"></a>
# **posListRegisters**
> kotlin.collections.List&lt;PosRegister&gt; posListRegisters()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
try {
    val result : kotlin.collections.List<PosRegister> = apiInstance.posListRegisters()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posListRegisters")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posListRegisters")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PosRegister&gt;**](PosRegister.md)

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

<a id="posListTables"></a>
# **posListTables**
> kotlin.collections.List&lt;PosTable&gt; posListTables()



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
try {
    val result : kotlin.collections.List<PosTable> = apiInstance.posListTables()
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posListTables")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posListTables")
    e.printStackTrace()
}
```

### Parameters
This endpoint does not need any parameter.

### Return type

[**kotlin.collections.List&lt;PosTable&gt;**](PosTable.md)

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

<a id="posOrderPrint"></a>
# **posOrderPrint**
> kotlin.Any posOrderPrint(orderNumber)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.posOrderPrint(orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posOrderPrint")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posOrderPrint")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |

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

<a id="posOrderReceipt"></a>
# **posOrderReceipt**
> kotlin.Any posOrderReceipt(orderNumber)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
try {
    val result : kotlin.Any = apiInstance.posOrderReceipt(orderNumber)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posOrderReceipt")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posOrderReceipt")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |

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

<a id="posPayOrder"></a>
# **posPayOrder**
> kotlin.Any posPayOrder(orderNumber, body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.posPayOrder(orderNumber, body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posPayOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posPayOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |
| **body** | **kotlin.Any**|  | |

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

<a id="posSumupCheckout"></a>
# **posSumupCheckout**
> kotlin.Any posSumupCheckout(body)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = PosApi()
val body : kotlin.Any =  // kotlin.Any | 
try {
    val result : kotlin.Any = apiInstance.posSumupCheckout(body)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling PosApi#posSumupCheckout")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling PosApi#posSumupCheckout")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **body** | **kotlin.Any**|  | |

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

