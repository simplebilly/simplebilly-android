# OrderConfirmationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createConfirmation**](OrderConfirmationApi.md#createConfirmation) | **POST** /api/v1/order-confirmations | 
[**deleteConfirmation**](OrderConfirmationApi.md#deleteConfirmation) | **DELETE** /api/v1/order-confirmations/{confirmation_id} | 
[**downloadConfirmationPdf**](OrderConfirmationApi.md#downloadConfirmationPdf) | **GET** /api/v1/order-confirmations/{confirmation_id}/pdf | 
[**getConfirmation**](OrderConfirmationApi.md#getConfirmation) | **GET** /api/v1/order-confirmations/{confirmation_id} | 
[**listConfirmations**](OrderConfirmationApi.md#listConfirmations) | **GET** /api/v1/order-confirmations/ | 
[**orderconfirmationRestore**](OrderConfirmationApi.md#orderconfirmationRestore) | **POST** /api/v1/order-confirmations/{confirmation_id}/restore | 
[**pursueConfirmation**](OrderConfirmationApi.md#pursueConfirmation) | **POST** /api/v1/order-confirmations/{confirmation_id}/pursue | 



## createConfirmation

> OrderConfirmation createConfirmation(orderConfirmationCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
OrderConfirmationCreate orderConfirmationCreate = new OrderConfirmationCreate(); // OrderConfirmationCreate | 
try {
    OrderConfirmation result = apiInstance.createConfirmation(orderConfirmationCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#createConfirmation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderConfirmationCreate** | [**OrderConfirmationCreate**](OrderConfirmationCreate.md)|  |

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteConfirmation

> deleteConfirmation(confirmationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
String confirmationId = null; // String | 
try {
    apiInstance.deleteConfirmation(confirmationId);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#deleteConfirmation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **confirmationId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## downloadConfirmationPdf

> downloadConfirmationPdf(confirmationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
String confirmationId = null; // String | 
try {
    apiInstance.downloadConfirmationPdf(confirmationId);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#downloadConfirmationPdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **confirmationId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json


## getConfirmation

> OrderConfirmation getConfirmation(confirmationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
String confirmationId = null; // String | 
try {
    OrderConfirmation result = apiInstance.getConfirmation(confirmationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#getConfirmation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **confirmationId** | **String**|  | [default to null]

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listConfirmations

> List&lt;OrderConfirmation&gt; listConfirmations(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<OrderConfirmation> result = apiInstance.listConfirmations(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#listConfirmations");
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

[**List&lt;OrderConfirmation&gt;**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## orderconfirmationRestore

> OrderConfirmation orderconfirmationRestore(confirmationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
String confirmationId = null; // String | 
try {
    OrderConfirmation result = apiInstance.orderconfirmationRestore(confirmationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#orderconfirmationRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **confirmationId** | **String**|  | [default to null]

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## pursueConfirmation

> DeliveryNote pursueConfirmation(confirmationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderConfirmationApi;

OrderConfirmationApi apiInstance = new OrderConfirmationApi();
String confirmationId = null; // String | 
try {
    DeliveryNote result = apiInstance.pursueConfirmation(confirmationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderConfirmationApi#pursueConfirmation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **confirmationId** | **String**|  | [default to null]

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

