# DownPaymentInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**downloadDownPaymentInvoicePdf**](DownPaymentInvoiceApi.md#downloadDownPaymentInvoicePdf) | **GET** /api/v1/down-payment-invoices/{id}/pdf | 
[**getDownPaymentInvoice**](DownPaymentInvoiceApi.md#getDownPaymentInvoice) | **GET** /api/v1/down-payment-invoices/{id} | 
[**listDownPaymentInvoices**](DownPaymentInvoiceApi.md#listDownPaymentInvoices) | **GET** /api/v1/down-payment-invoices/ | 



## downloadDownPaymentInvoicePdf

> downloadDownPaymentInvoicePdf(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DownPaymentInvoiceApi;

DownPaymentInvoiceApi apiInstance = new DownPaymentInvoiceApi();
String id = null; // String | 
try {
    apiInstance.downloadDownPaymentInvoicePdf(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DownPaymentInvoiceApi#downloadDownPaymentInvoicePdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDownPaymentInvoice

> DownPaymentInvoice getDownPaymentInvoice(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DownPaymentInvoiceApi;

DownPaymentInvoiceApi apiInstance = new DownPaymentInvoiceApi();
String id = null; // String | 
try {
    DownPaymentInvoice result = apiInstance.getDownPaymentInvoice(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DownPaymentInvoiceApi#getDownPaymentInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

[**DownPaymentInvoice**](DownPaymentInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDownPaymentInvoices

> List&lt;DownPaymentInvoice&gt; listDownPaymentInvoices(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DownPaymentInvoiceApi;

DownPaymentInvoiceApi apiInstance = new DownPaymentInvoiceApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<DownPaymentInvoice> result = apiInstance.listDownPaymentInvoices(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DownPaymentInvoiceApi#listDownPaymentInvoices");
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

[**List&lt;DownPaymentInvoice&gt;**](DownPaymentInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

