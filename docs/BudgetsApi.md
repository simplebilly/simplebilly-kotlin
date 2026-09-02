# BudgetsApi

All URIs are relative to *https://demo.simplebilly.com*

| Method | HTTP request | Description |
| ------------- | ------------- | ------------- |
| [**budgetsApi**](BudgetsApi.md#budgetsApi) | **GET** /api/v1/bookkeeping/budgets |  |
| [**upsertBudgetGoalApi**](BudgetsApi.md#upsertBudgetGoalApi) | **PUT** /api/v1/bookkeeping/budgets/goals/{category} |  |


<a id="budgetsApi"></a>
# **budgetsApi**
> BudgetErgebnis budgetsApi(year, month)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BudgetsApi()
val year : kotlin.Int = 56 // kotlin.Int | 
val month : kotlin.Int = 56 // kotlin.Int | 
try {
    val result : BudgetErgebnis = apiInstance.budgetsApi(year, month)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BudgetsApi#budgetsApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BudgetsApi#budgetsApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **year** | **kotlin.Int**|  | |
| **month** | **kotlin.Int**|  | |

### Return type

[**BudgetErgebnis**](BudgetErgebnis.md)

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

<a id="upsertBudgetGoalApi"></a>
# **upsertBudgetGoalApi**
> Budget upsertBudgetGoalApi(category, budgetGoalRequest)



### Example
```kotlin
// Import classes:
//import org.openapitools.client.infrastructure.*
//import org.openapitools.client.models.*

val apiInstance = BudgetsApi()
val category : kotlin.String = category_example // kotlin.String | 
val budgetGoalRequest : BudgetGoalRequest =  // BudgetGoalRequest | 
try {
    val result : Budget = apiInstance.upsertBudgetGoalApi(category, budgetGoalRequest)
    println(result)
} catch (e: ClientException) {
    println("4xx response calling BudgetsApi#upsertBudgetGoalApi")
    e.printStackTrace()
} catch (e: ServerException) {
    println("5xx response calling BudgetsApi#upsertBudgetGoalApi")
    e.printStackTrace()
}
```

### Parameters
| Name | Type | Description  | Notes |
| ------------- | ------------- | ------------- | ------------- |
| **category** | **kotlin.String**|  | |
| **budgetGoalRequest** | [**BudgetGoalRequest**](BudgetGoalRequest.md)|  | |

### Return type

[**Budget**](Budget.md)

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

