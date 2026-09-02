# ShipmentApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**createShipment**](ShipmentApi.md#createShipment) | **POST** /api/v1/shipments |  |
| [**createShipmentFromOrder**](ShipmentApi.md#createShipmentFromOrder) | **POST** /api/v1/orders/{order_number}/shipments | Create a real shipment for an order: calls the configured carrier&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped. |
| [**deleteShipment**](ShipmentApi.md#deleteShipment) | **DELETE** /api/v1/shipments/{shipment_id} |  |
| [**getShipment**](ShipmentApi.md#getShipment) | **GET** /api/v1/shipments/{shipment_id} |  |
| [**listShipments**](ShipmentApi.md#listShipments) | **GET** /api/v1/shipments |  |
| [**trackOrderPublic**](ShipmentApi.md#trackOrderPublic) | **POST** /api/v1/public/track | Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API). |
| [**trackShipmentApi**](ShipmentApi.md#trackShipmentApi) | **GET** /api/v1/shipments/{shipment_id}/tracking |  |
| [**updateShipmentStatus**](ShipmentApi.md#updateShipmentStatus) | **PUT** /api/v1/shipments/{shipment_id}/status |  |


<a id="createShipment"></a>
# **createShipment**
> Shipment createShipment(shipment)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val shipment : Shipment =  // Shipment | 
try {
    val result : Shipment = apiInstance.createShipment(shipment)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#createShipment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#createShipment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shipment** | [**Shipment**](Shipment.md)|  | |

### Return type

[**Shipment**](Shipment.md)

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

<a id="createShipmentFromOrder"></a>
# **createShipmentFromOrder**
> Shipment createShipmentFromOrder(orderNumber, createShipmentRequest)

Create a real shipment for an order: calls the configured carrier&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val orderNumber : kotlin.String = orderNumber_example // kotlin.String | 
val createShipmentRequest : CreateShipmentRequest =  // CreateShipmentRequest | 
try {
    val result : Shipment = apiInstance.createShipmentFromOrder(orderNumber, createShipmentRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#createShipmentFromOrder")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#createShipmentFromOrder")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **orderNumber** | **kotlin.String**|  | |
| **createShipmentRequest** | [**CreateShipmentRequest**](CreateShipmentRequest.md)|  | |

### Return type

[**Shipment**](Shipment.md)

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

<a id="deleteShipment"></a>
# **deleteShipment**
> deleteShipment(shipmentId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val shipmentId : kotlin.String = shipmentId_example // kotlin.String | 
try {
    apiInstance.deleteShipment(shipmentId)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#deleteShipment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#deleteShipment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shipmentId** | **kotlin.String**|  | |

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

<a id="getShipment"></a>
# **getShipment**
> Shipment getShipment(shipmentId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val shipmentId : kotlin.String = shipmentId_example // kotlin.String | 
try {
    val result : Shipment = apiInstance.getShipment(shipmentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#getShipment")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#getShipment")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shipmentId** | **kotlin.String**|  | |

### Return type

[**Shipment**](Shipment.md)

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

<a id="listShipments"></a>
# **listShipments**
> kotlin.collections.List&lt;Shipment&gt; listShipments(page, pageSize, search, includeDeleted)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val page : kotlin.Int = 1 // kotlin.Int | 
val pageSize : kotlin.Int = 56 // kotlin.Int | 
val search : kotlin.String = search_example // kotlin.String | 
val includeDeleted : kotlin.Boolean = true // kotlin.Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    val result : kotlin.collections.List<Shipment> = apiInstance.listShipments(page, pageSize, search, includeDeleted)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#listShipments")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#listShipments")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **page** | **kotlin.Int**|  | [optional] |
| **pageSize** | **kotlin.Int**|  | [optional] |
| **search** | **kotlin.String**|  | [optional] |
| **includeDeleted** | **kotlin.Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] |

### Return type

[**kotlin.collections.List&lt;Shipment&gt;**](Shipment.md)

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

<a id="trackOrderPublic"></a>
# **trackOrderPublic**
> TrackOrderResponse trackOrderPublic(trackOrderRequest)

Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val trackOrderRequest : TrackOrderRequest =  // TrackOrderRequest | 
try {
    val result : TrackOrderResponse = apiInstance.trackOrderPublic(trackOrderRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#trackOrderPublic")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#trackOrderPublic")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **trackOrderRequest** | [**TrackOrderRequest**](TrackOrderRequest.md)|  | |

### Return type

[**TrackOrderResponse**](TrackOrderResponse.md)

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

<a id="trackShipmentApi"></a>
# **trackShipmentApi**
> TrackingInfo trackShipmentApi(shipmentId)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val shipmentId : kotlin.String = shipmentId_example // kotlin.String | 
try {
    val result : TrackingInfo = apiInstance.trackShipmentApi(shipmentId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#trackShipmentApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#trackShipmentApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shipmentId** | **kotlin.String**|  | |

### Return type

[**TrackingInfo**](TrackingInfo.md)

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

<a id="updateShipmentStatus"></a>
# **updateShipmentStatus**
> Shipment updateShipmentStatus(shipmentId, shipmentStatusUpdate)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = ShipmentApi()
val shipmentId : kotlin.String = shipmentId_example // kotlin.String | 
val shipmentStatusUpdate : ShipmentStatusUpdate =  // ShipmentStatusUpdate | 
try {
    val result : Shipment = apiInstance.updateShipmentStatus(shipmentId, shipmentStatusUpdate)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling ShipmentApi#updateShipmentStatus")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling ShipmentApi#updateShipmentStatus")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **shipmentId** | **kotlin.String**|  | |
| **shipmentStatusUpdate** | [**ShipmentStatusUpdate**](ShipmentStatusUpdate.md)|  | |

### Return type

[**Shipment**](Shipment.md)

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

