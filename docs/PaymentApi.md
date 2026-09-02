# PaymentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPayment**](PaymentApi.md#createPayment) | **POST** /api/v1/payments | 
[**deletePayment**](PaymentApi.md#deletePayment) | **DELETE** /api/v1/payments/{id} | 
[**getPayment**](PaymentApi.md#getPayment) | **GET** /api/v1/payments/{id} | 
[**getPayments**](PaymentApi.md#getPayments) | **GET** /api/v1/payments/ | 
[**paymentRestore**](PaymentApi.md#paymentRestore) | **POST** /api/v1/payments/{id}/restore | 
[**updatePayment**](PaymentApi.md#updatePayment) | **PUT** /api/v1/payments/{id} | 



## createPayment

> Payment createPayment(paymentCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentApi;

PaymentApi apiInstance = new PaymentApi();
PaymentCreate paymentCreate = new PaymentCreate(); // PaymentCreate | 
try {
    Payment result = apiInstance.createPayment(paymentCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentApi#createPayment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **paymentCreate** | [**PaymentCreate**](PaymentCreate.md)|  |

### Return type

[**Payment**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePayment

> deletePayment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentApi;

PaymentApi apiInstance = new PaymentApi();
UUID id = null; // UUID | 
try {
    apiInstance.deletePayment(id);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentApi#deletePayment");
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


## getPayment

> Payment getPayment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentApi;

PaymentApi apiInstance = new PaymentApi();
UUID id = null; // UUID | 
try {
    Payment result = apiInstance.getPayment(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentApi#getPayment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Payment**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPayments

> List&lt;Payment&gt; getPayments(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentApi;

PaymentApi apiInstance = new PaymentApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Payment> result = apiInstance.getPayments(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentApi#getPayments");
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

[**List&lt;Payment&gt;**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## paymentRestore

> Payment paymentRestore(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentApi;

PaymentApi apiInstance = new PaymentApi();
UUID id = null; // UUID | 
try {
    Payment result = apiInstance.paymentRestore(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentApi#paymentRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Payment**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updatePayment

> Payment updatePayment(id, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentApi;

PaymentApi apiInstance = new PaymentApi();
UUID id = null; // UUID | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Payment result = apiInstance.updatePayment(id, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentApi#updatePayment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Payment**](Payment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

