# SupplierConditionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSupplierCondition**](SupplierConditionApi.md#createSupplierCondition) | **POST** /api/v1/supplier-conditions | 
[**deleteSupplierCondition**](SupplierConditionApi.md#deleteSupplierCondition) | **DELETE** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**getSupplierCondition**](SupplierConditionApi.md#getSupplierCondition) | **GET** /api/v1/supplier-conditions/{supplier_condition_id} | 
[**listSupplierConditions**](SupplierConditionApi.md#listSupplierConditions) | **GET** /api/v1/supplier-conditions/ | 
[**updateSupplierCondition**](SupplierConditionApi.md#updateSupplierCondition) | **PUT** /api/v1/supplier-conditions/{supplier_condition_id} | 



## createSupplierCondition

> SupplierCondition createSupplierCondition(supplierConditionCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierConditionApi;

SupplierConditionApi apiInstance = new SupplierConditionApi();
SupplierConditionCreate supplierConditionCreate = new SupplierConditionCreate(); // SupplierConditionCreate | 
try {
    SupplierCondition result = apiInstance.createSupplierCondition(supplierConditionCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierConditionApi#createSupplierCondition");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierConditionCreate** | [**SupplierConditionCreate**](SupplierConditionCreate.md)|  |

### Return type

[**SupplierCondition**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSupplierCondition

> deleteSupplierCondition(supplierConditionId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierConditionApi;

SupplierConditionApi apiInstance = new SupplierConditionApi();
String supplierConditionId = null; // String | 
try {
    apiInstance.deleteSupplierCondition(supplierConditionId);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierConditionApi#deleteSupplierCondition");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierConditionId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSupplierCondition

> SupplierCondition getSupplierCondition(supplierConditionId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierConditionApi;

SupplierConditionApi apiInstance = new SupplierConditionApi();
String supplierConditionId = null; // String | 
try {
    SupplierCondition result = apiInstance.getSupplierCondition(supplierConditionId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierConditionApi#getSupplierCondition");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierConditionId** | **String**|  | [default to null]

### Return type

[**SupplierCondition**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listSupplierConditions

> List&lt;SupplierCondition&gt; listSupplierConditions(page, pageSize, supplierContactId, search)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierConditionApi;

SupplierConditionApi apiInstance = new SupplierConditionApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String supplierContactId = null; // String | 
String search = null; // String | 
try {
    List<SupplierCondition> result = apiInstance.listSupplierConditions(page, pageSize, supplierContactId, search);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierConditionApi#listSupplierConditions");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **supplierContactId** | **String**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;SupplierCondition&gt;**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSupplierCondition

> SupplierCondition updateSupplierCondition(supplierConditionId, supplierConditionUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierConditionApi;

SupplierConditionApi apiInstance = new SupplierConditionApi();
String supplierConditionId = null; // String | 
SupplierConditionUpdate supplierConditionUpdate = new SupplierConditionUpdate(); // SupplierConditionUpdate | 
try {
    SupplierCondition result = apiInstance.updateSupplierCondition(supplierConditionId, supplierConditionUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierConditionApi#updateSupplierCondition");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierConditionId** | **String**|  | [default to null]
 **supplierConditionUpdate** | [**SupplierConditionUpdate**](SupplierConditionUpdate.md)|  |

### Return type

[**SupplierCondition**](SupplierCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

