# TimeEntriesApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**clockInTimeEntry**](TimeEntriesApi.md#clockInTimeEntry) | **POST** /api/v1/time-entries | Clock in for the authenticated user (resolved via their employee profile). |
| [**clockOutTimeEntry**](TimeEntriesApi.md#clockOutTimeEntry) | **PATCH** /api/v1/time-entries/{id} | Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;. |
| [**getLaborCosts**](TimeEntriesApi.md#getLaborCosts) | **GET** /api/v1/labor-costs | Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate. |
| [**listTimeEntries**](TimeEntriesApi.md#listTimeEntries) | **GET** /api/v1/time-entries | List time entries with optional date-range / active / employee filters. |


<a id="clockInTimeEntry"></a>
# **clockInTimeEntry**
> TimeEntryDto clockInTimeEntry(timeEntryClockIn)

Clock in for the authenticated user (resolved via their employee profile).

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TimeEntriesApi()
val timeEntryClockIn : TimeEntryClockIn =  // TimeEntryClockIn | 
try {
    val result : TimeEntryDto = apiInstance.clockInTimeEntry(timeEntryClockIn)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TimeEntriesApi#clockInTimeEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TimeEntriesApi#clockInTimeEntry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **timeEntryClockIn** | [**TimeEntryClockIn**](TimeEntryClockIn.md)|  | |

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

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

<a id="clockOutTimeEntry"></a>
# **clockOutTimeEntry**
> TimeEntryDto clockOutTimeEntry(id, timeEntryClockOut)

Clock out an entry: the entry&#39;s owner, or anyone with &#x60;time_entries:write&#x60;.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TimeEntriesApi()
val id : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
val timeEntryClockOut : TimeEntryClockOut =  // TimeEntryClockOut | 
try {
    val result : TimeEntryDto = apiInstance.clockOutTimeEntry(id, timeEntryClockOut)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TimeEntriesApi#clockOutTimeEntry")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TimeEntriesApi#clockOutTimeEntry")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **id** | **java.util.UUID**|  | |
| **timeEntryClockOut** | [**TimeEntryClockOut**](TimeEntryClockOut.md)|  | |

### Return type

[**TimeEntryDto**](TimeEntryDto.md)

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

<a id="getLaborCosts"></a>
# **getLaborCosts**
> kotlin.collections.List&lt;LaborCostRow&gt; getLaborCosts(from, to, groupBy)

Labor-cost report: worked hours aggregated per employee / order / day, valued at the employee&#39;s hourly cost rate.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TimeEntriesApi()
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val groupBy : kotlin.String = groupBy_example // kotlin.String | One of \"employee\", \"order\" or \"day\".
try {
    val result : kotlin.collections.List<LaborCostRow> = apiInstance.getLaborCosts(from, to, groupBy)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TimeEntriesApi#getLaborCosts")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TimeEntriesApi#getLaborCosts")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **from** | **java.time.LocalDate**|  | |
| **to** | **java.time.LocalDate**|  | |
| **groupBy** | **kotlin.String**| One of \&quot;employee\&quot;, \&quot;order\&quot; or \&quot;day\&quot;. | |

### Return type

[**kotlin.collections.List&lt;LaborCostRow&gt;**](LaborCostRow.md)

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

<a id="listTimeEntries"></a>
# **listTimeEntries**
> kotlin.collections.List&lt;TimeEntryDto&gt; listTimeEntries(from, to, active, employeeId)

List time entries with optional date-range / active / employee filters.

### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = TimeEntriesApi()
val from : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val to : java.time.LocalDate = 2013-10-20 // java.time.LocalDate | 
val active : kotlin.Boolean = true // kotlin.Boolean | Only currently running shifts (clock_in set, clock_out null).
val employeeId : java.util.UUID = 38400000-8cf0-11bd-b23e-10b96e4ef00d // java.util.UUID | 
try {
    val result : kotlin.collections.List<TimeEntryDto> = apiInstance.listTimeEntries(from, to, active, employeeId)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling TimeEntriesApi#listTimeEntries")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling TimeEntriesApi#listTimeEntries")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **from** | **java.time.LocalDate**|  | [optional] |
| **to** | **java.time.LocalDate**|  | [optional] |
| **active** | **kotlin.Boolean**| Only currently running shifts (clock_in set, clock_out null). | [optional] |
| **employeeId** | **java.util.UUID**|  | [optional] |

### Return type

[**kotlin.collections.List&lt;TimeEntryDto&gt;**](TimeEntryDto.md)

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

