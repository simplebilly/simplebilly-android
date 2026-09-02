# ComplianceTrainingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createComplianceTraining**](ComplianceTrainingApi.md#createComplianceTraining) | **POST** /api/v1/compliance-trainings | 
[**deleteComplianceTraining**](ComplianceTrainingApi.md#deleteComplianceTraining) | **DELETE** /api/v1/compliance-trainings/{id} | 
[**getComplianceTraining**](ComplianceTrainingApi.md#getComplianceTraining) | **GET** /api/v1/compliance-trainings/{id} | 
[**getComplianceTrainings**](ComplianceTrainingApi.md#getComplianceTrainings) | **GET** /api/v1/compliance-trainings/ | 
[**updateComplianceTraining**](ComplianceTrainingApi.md#updateComplianceTraining) | **PUT** /api/v1/compliance-trainings/{id} | 



## createComplianceTraining

> ComplianceTraining createComplianceTraining(complianceTrainingCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ComplianceTrainingApi;

ComplianceTrainingApi apiInstance = new ComplianceTrainingApi();
ComplianceTrainingCreate complianceTrainingCreate = new ComplianceTrainingCreate(); // ComplianceTrainingCreate | 
try {
    ComplianceTraining result = apiInstance.createComplianceTraining(complianceTrainingCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ComplianceTrainingApi#createComplianceTraining");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **complianceTrainingCreate** | [**ComplianceTrainingCreate**](ComplianceTrainingCreate.md)|  |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteComplianceTraining

> deleteComplianceTraining(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ComplianceTrainingApi;

ComplianceTrainingApi apiInstance = new ComplianceTrainingApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteComplianceTraining(id);
} catch (ApiException e) {
    System.err.println("Exception when calling ComplianceTrainingApi#deleteComplianceTraining");
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


## getComplianceTraining

> ComplianceTraining getComplianceTraining(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ComplianceTrainingApi;

ComplianceTrainingApi apiInstance = new ComplianceTrainingApi();
UUID id = null; // UUID | 
try {
    ComplianceTraining result = apiInstance.getComplianceTraining(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ComplianceTrainingApi#getComplianceTraining");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getComplianceTrainings

> List&lt;ComplianceTraining&gt; getComplianceTrainings(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ComplianceTrainingApi;

ComplianceTrainingApi apiInstance = new ComplianceTrainingApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<ComplianceTraining> result = apiInstance.getComplianceTrainings(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ComplianceTrainingApi#getComplianceTrainings");
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

[**List&lt;ComplianceTraining&gt;**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateComplianceTraining

> ComplianceTraining updateComplianceTraining(id, complianceTrainingUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ComplianceTrainingApi;

ComplianceTrainingApi apiInstance = new ComplianceTrainingApi();
UUID id = null; // UUID | 
ComplianceTrainingUpdate complianceTrainingUpdate = new ComplianceTrainingUpdate(); // ComplianceTrainingUpdate | 
try {
    ComplianceTraining result = apiInstance.updateComplianceTraining(id, complianceTrainingUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ComplianceTrainingApi#updateComplianceTraining");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **complianceTrainingUpdate** | [**ComplianceTrainingUpdate**](ComplianceTrainingUpdate.md)|  |

### Return type

[**ComplianceTraining**](ComplianceTraining.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

