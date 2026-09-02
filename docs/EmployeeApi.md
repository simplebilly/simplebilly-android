# EmployeeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createEmployee**](EmployeeApi.md#createEmployee) | **POST** /api/v1/employees | 
[**deleteEmployee**](EmployeeApi.md#deleteEmployee) | **DELETE** /api/v1/employees/{id} | 
[**employeeRestore**](EmployeeApi.md#employeeRestore) | **POST** /api/v1/employees/{id}/restore | 
[**getEmployee**](EmployeeApi.md#getEmployee) | **GET** /api/v1/employees/{id} | 
[**getEmployeePayrollSummary**](EmployeeApi.md#getEmployeePayrollSummary) | **GET** /api/v1/employees/{id}/payroll-summary | 
[**getEmployees**](EmployeeApi.md#getEmployees) | **GET** /api/v1/employees/ | 
[**updateEmployee**](EmployeeApi.md#updateEmployee) | **PUT** /api/v1/employees/{id} | 



## createEmployee

> Employee createEmployee(employeeCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
EmployeeCreate employeeCreate = new EmployeeCreate(); // EmployeeCreate | 
try {
    Employee result = apiInstance.createEmployee(employeeCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#createEmployee");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employeeCreate** | [**EmployeeCreate**](EmployeeCreate.md)|  |

### Return type

[**Employee**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteEmployee

> deleteEmployee(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteEmployee(id);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#deleteEmployee");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## employeeRestore

> Employee employeeRestore(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
UUID id = null; // UUID | 
try {
    Employee result = apiInstance.employeeRestore(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#employeeRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Employee**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getEmployee

> Employee getEmployee(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
UUID id = null; // UUID | 
try {
    Employee result = apiInstance.getEmployee(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#getEmployee");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Employee**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getEmployeePayrollSummary

> PayrollSummary getEmployeePayrollSummary(id, year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
UUID id = null; // UUID | 
Integer year = null; // Integer | Fiscal year for the breakdown; defaults to the current year.
try {
    PayrollSummary result = apiInstance.getEmployeePayrollSummary(id, year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#getEmployeePayrollSummary");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **year** | **Integer**| Fiscal year for the breakdown; defaults to the current year. | [optional] [default to null]

### Return type

[**PayrollSummary**](PayrollSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getEmployees

> List&lt;Employee&gt; getEmployees(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Employee> result = apiInstance.getEmployees(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#getEmployees");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **includeDeleted** | **Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] [default to null]

### Return type

[**List&lt;Employee&gt;**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateEmployee

> Employee updateEmployee(id, employeeUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmployeeApi;

EmployeeApi apiInstance = new EmployeeApi();
UUID id = null; // UUID | 
EmployeeUpdate employeeUpdate = new EmployeeUpdate(); // EmployeeUpdate | 
try {
    Employee result = apiInstance.updateEmployee(id, employeeUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmployeeApi#updateEmployee");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **employeeUpdate** | [**EmployeeUpdate**](EmployeeUpdate.md)|  |

### Return type

[**Employee**](Employee.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

