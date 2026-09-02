# CustomerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCustomer**](CustomerApi.md#createCustomer) | **POST** /api/v1/customers | 
[**customerRestore**](CustomerApi.md#customerRestore) | **POST** /api/v1/customers/{customer_id}/restore | 
[**deleteCustomer**](CustomerApi.md#deleteCustomer) | **DELETE** /api/v1/customers/{customer_id} | 
[**getCustomer**](CustomerApi.md#getCustomer) | **GET** /api/v1/customers/{customer_id} | 
[**getCustomers**](CustomerApi.md#getCustomers) | **GET** /api/v1/customers/ | 
[**updateCustomer**](CustomerApi.md#updateCustomer) | **PUT** /api/v1/customers/{customer_id} | 



## createCustomer

> Customer createCustomer(customerCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
CustomerCreate customerCreate = new CustomerCreate(); // CustomerCreate | 
try {
    Customer result = apiInstance.createCustomer(customerCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#createCustomer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerCreate** | [**CustomerCreate**](CustomerCreate.md)|  |

### Return type

[**Customer**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## customerRestore

> Customer customerRestore(customerId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String customerId = null; // String | 
try {
    Customer result = apiInstance.customerRestore(customerId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#customerRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerId** | **String**|  | [default to null]

### Return type

[**Customer**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## deleteCustomer

> deleteCustomer(customerId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String customerId = null; // String | 
try {
    apiInstance.deleteCustomer(customerId);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#deleteCustomer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCustomer

> Customer getCustomer(customerId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String customerId = null; // String | 
try {
    Customer result = apiInstance.getCustomer(customerId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#getCustomer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerId** | **String**|  | [default to null]

### Return type

[**Customer**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCustomers

> List&lt;Customer&gt; getCustomers(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Customer> result = apiInstance.getCustomers(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#getCustomers");
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

[**List&lt;Customer&gt;**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCustomer

> Customer updateCustomer(customerId, customerUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerApi;

CustomerApi apiInstance = new CustomerApi();
String customerId = null; // String | 
CustomerUpdate customerUpdate = new CustomerUpdate(); // CustomerUpdate | 
try {
    Customer result = apiInstance.updateCustomer(customerId, customerUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerApi#updateCustomer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerId** | **String**|  | [default to null]
 **customerUpdate** | [**CustomerUpdate**](CustomerUpdate.md)|  |

### Return type

[**Customer**](Customer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

