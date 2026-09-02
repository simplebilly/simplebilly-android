# CustomerGroupApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addGroupMembers**](CustomerGroupApi.md#addGroupMembers) | **POST** /api/v1/customer-groups/{customer_group_id}/members | 
[**createCustomerGroup**](CustomerGroupApi.md#createCustomerGroup) | **POST** /api/v1/customer-groups | 
[**deleteCustomerGroup**](CustomerGroupApi.md#deleteCustomerGroup) | **DELETE** /api/v1/customer-groups/{customer_group_id} | 
[**getCustomerGroup**](CustomerGroupApi.md#getCustomerGroup) | **GET** /api/v1/customer-groups/{customer_group_id} | 
[**listCustomerGroups**](CustomerGroupApi.md#listCustomerGroups) | **GET** /api/v1/customer-groups/ | 
[**updateCustomerGroup**](CustomerGroupApi.md#updateCustomerGroup) | **PUT** /api/v1/customer-groups/{customer_group_id} | 



## addGroupMembers

> CustomerGroup addGroupMembers(customerGroupId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerGroupApi;

CustomerGroupApi apiInstance = new CustomerGroupApi();
String customerGroupId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    CustomerGroup result = apiInstance.addGroupMembers(customerGroupId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerGroupApi#addGroupMembers");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerGroupId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createCustomerGroup

> CustomerGroup createCustomerGroup(customerGroupCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerGroupApi;

CustomerGroupApi apiInstance = new CustomerGroupApi();
CustomerGroupCreate customerGroupCreate = new CustomerGroupCreate(); // CustomerGroupCreate | 
try {
    CustomerGroup result = apiInstance.createCustomerGroup(customerGroupCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerGroupApi#createCustomerGroup");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerGroupCreate** | [**CustomerGroupCreate**](CustomerGroupCreate.md)|  |

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteCustomerGroup

> deleteCustomerGroup(customerGroupId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerGroupApi;

CustomerGroupApi apiInstance = new CustomerGroupApi();
String customerGroupId = null; // String | 
try {
    apiInstance.deleteCustomerGroup(customerGroupId);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerGroupApi#deleteCustomerGroup");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerGroupId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCustomerGroup

> CustomerGroup getCustomerGroup(customerGroupId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerGroupApi;

CustomerGroupApi apiInstance = new CustomerGroupApi();
String customerGroupId = null; // String | 
try {
    CustomerGroup result = apiInstance.getCustomerGroup(customerGroupId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerGroupApi#getCustomerGroup");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerGroupId** | **String**|  | [default to null]

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listCustomerGroups

> List&lt;CustomerGroup&gt; listCustomerGroups(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerGroupApi;

CustomerGroupApi apiInstance = new CustomerGroupApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<CustomerGroup> result = apiInstance.listCustomerGroups(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerGroupApi#listCustomerGroups");
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

[**List&lt;CustomerGroup&gt;**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCustomerGroup

> CustomerGroup updateCustomerGroup(customerGroupId, customerGroupUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerGroupApi;

CustomerGroupApi apiInstance = new CustomerGroupApi();
String customerGroupId = null; // String | 
CustomerGroupUpdate customerGroupUpdate = new CustomerGroupUpdate(); // CustomerGroupUpdate | 
try {
    CustomerGroup result = apiInstance.updateCustomerGroup(customerGroupId, customerGroupUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerGroupApi#updateCustomerGroup");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerGroupId** | **String**|  | [default to null]
 **customerGroupUpdate** | [**CustomerGroupUpdate**](CustomerGroupUpdate.md)|  |

### Return type

[**CustomerGroup**](CustomerGroup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

