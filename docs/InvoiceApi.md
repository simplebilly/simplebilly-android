# InvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createInvoice**](InvoiceApi.md#createInvoice) | **POST** /api/v1/invoices | 
[**deleteInvoice**](InvoiceApi.md#deleteInvoice) | **DELETE** /api/v1/invoices/{id} | 
[**downloadInvoicePdf**](InvoiceApi.md#downloadInvoicePdf) | **GET** /api/v1/invoices/{id}/pdf | 
[**getInvoice**](InvoiceApi.md#getInvoice) | **GET** /api/v1/invoices/{id} | 
[**getInvoicePdfUrl**](InvoiceApi.md#getInvoicePdfUrl) | **GET** /api/v1/invoices/{id}/pdf-url | 
[**getInvoices**](InvoiceApi.md#getInvoices) | **GET** /api/v1/invoices/ | 
[**invoiceRestore**](InvoiceApi.md#invoiceRestore) | **POST** /api/v1/invoices/{id}/restore | 
[**updateInvoice**](InvoiceApi.md#updateInvoice) | **PUT** /api/v1/invoices/{id} | 



## createInvoice

> Invoice createInvoice(invoiceCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
InvoiceCreate invoiceCreate = new InvoiceCreate(); // InvoiceCreate | 
try {
    Invoice result = apiInstance.createInvoice(invoiceCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#createInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **invoiceCreate** | [**InvoiceCreate**](InvoiceCreate.md)|  |

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteInvoice

> deleteInvoice(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
String id = null; // String | 
try {
    apiInstance.deleteInvoice(id);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#deleteInvoice");
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


## downloadInvoicePdf

> downloadInvoicePdf(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
String id = null; // String | 
try {
    apiInstance.downloadInvoicePdf(id);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#downloadInvoicePdf");
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
- **Accept**: application/pdf, application/json


## getInvoice

> Invoice getInvoice(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
String id = null; // String | 
try {
    Invoice result = apiInstance.getInvoice(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#getInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getInvoicePdfUrl

> InvoicePdfUrlResponse getInvoicePdfUrl(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
String id = null; // String | 
try {
    InvoicePdfUrlResponse result = apiInstance.getInvoicePdfUrl(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#getInvoicePdfUrl");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

[**InvoicePdfUrlResponse**](InvoicePdfUrlResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getInvoices

> List&lt;Invoice&gt; getInvoices(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Invoice> result = apiInstance.getInvoices(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#getInvoices");
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

[**List&lt;Invoice&gt;**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## invoiceRestore

> Invoice invoiceRestore(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
String id = null; // String | 
try {
    Invoice result = apiInstance.invoiceRestore(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#invoiceRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateInvoice

> Invoice updateInvoice(id, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InvoiceApi;

InvoiceApi apiInstance = new InvoiceApi();
String id = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Invoice result = apiInstance.updateInvoice(id, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InvoiceApi#updateInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

