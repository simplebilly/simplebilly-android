# BudgetsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**budgetsApi**](BudgetsApi.md#budgetsApi) | **GET** /api/v1/bookkeeping/budgets | 
[**upsertBudgetGoalApi**](BudgetsApi.md#upsertBudgetGoalApi) | **PUT** /api/v1/bookkeeping/budgets/goals/{category} | 



## budgetsApi

> BudgetErgebnis budgetsApi(year, month)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BudgetsApi;

BudgetsApi apiInstance = new BudgetsApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
try {
    BudgetErgebnis result = apiInstance.budgetsApi(year, month);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BudgetsApi#budgetsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]
 **month** | **Integer**|  | [default to null]

### Return type

[**BudgetErgebnis**](BudgetErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## upsertBudgetGoalApi

> Budget upsertBudgetGoalApi(category, budgetGoalRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BudgetsApi;

BudgetsApi apiInstance = new BudgetsApi();
String category = null; // String | 
BudgetGoalRequest budgetGoalRequest = new BudgetGoalRequest(); // BudgetGoalRequest | 
try {
    Budget result = apiInstance.upsertBudgetGoalApi(category, budgetGoalRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BudgetsApi#upsertBudgetGoalApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **category** | **String**|  | [default to null]
 **budgetGoalRequest** | [**BudgetGoalRequest**](BudgetGoalRequest.md)|  |

### Return type

[**Budget**](Budget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

