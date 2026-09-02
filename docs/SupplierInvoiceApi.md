# SupplierInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSupplierInvoice**](SupplierInvoiceApi.md#createSupplierInvoice) | **POST** /api/v1/supplier-invoices | 
[**deleteSupplierInvoice**](SupplierInvoiceApi.md#deleteSupplierInvoice) | **DELETE** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**getSupplierInvoice**](SupplierInvoiceApi.md#getSupplierInvoice) | **GET** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**listSupplierInvoices**](SupplierInvoiceApi.md#listSupplierInvoices) | **GET** /api/v1/supplier-invoices/ | 
[**updateSupplierInvoice**](SupplierInvoiceApi.md#updateSupplierInvoice) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id} | 
[**updateSupplierInvoiceStatus**](SupplierInvoiceApi.md#updateSupplierInvoiceStatus) | **PUT** /api/v1/supplier-invoices/{supplier_invoice_id}/status | 



## createSupplierInvoice

> SupplierInvoice createSupplierInvoice(supplierInvoice)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierInvoiceApi;

SupplierInvoiceApi apiInstance = new SupplierInvoiceApi();
SupplierInvoice supplierInvoice = new SupplierInvoice(); // SupplierInvoice | 
try {
    SupplierInvoice result = apiInstance.createSupplierInvoice(supplierInvoice);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierInvoiceApi#createSupplierInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierInvoice** | [**SupplierInvoice**](SupplierInvoice.md)|  |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSupplierInvoice

> deleteSupplierInvoice(supplierInvoiceId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierInvoiceApi;

SupplierInvoiceApi apiInstance = new SupplierInvoiceApi();
String supplierInvoiceId = null; // String | 
try {
    apiInstance.deleteSupplierInvoice(supplierInvoiceId);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierInvoiceApi#deleteSupplierInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierInvoiceId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSupplierInvoice

> SupplierInvoice getSupplierInvoice(supplierInvoiceId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierInvoiceApi;

SupplierInvoiceApi apiInstance = new SupplierInvoiceApi();
String supplierInvoiceId = null; // String | 
try {
    SupplierInvoice result = apiInstance.getSupplierInvoice(supplierInvoiceId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierInvoiceApi#getSupplierInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierInvoiceId** | **String**|  | [default to null]

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listSupplierInvoices

> List&lt;SupplierInvoice&gt; listSupplierInvoices(page, pageSize, status, purchaseOrderId, supplierName)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierInvoiceApi;

SupplierInvoiceApi apiInstance = new SupplierInvoiceApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String purchaseOrderId = null; // String | 
String supplierName = null; // String | 
try {
    List<SupplierInvoice> result = apiInstance.listSupplierInvoices(page, pageSize, status, purchaseOrderId, supplierName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierInvoiceApi#listSupplierInvoices");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **purchaseOrderId** | **String**|  | [optional] [default to null]
 **supplierName** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;SupplierInvoice&gt;**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSupplierInvoice

> SupplierInvoice updateSupplierInvoice(supplierInvoiceId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierInvoiceApi;

SupplierInvoiceApi apiInstance = new SupplierInvoiceApi();
String supplierInvoiceId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    SupplierInvoice result = apiInstance.updateSupplierInvoice(supplierInvoiceId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierInvoiceApi#updateSupplierInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierInvoiceId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateSupplierInvoiceStatus

> SupplierInvoice updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupplierInvoiceApi;

SupplierInvoiceApi apiInstance = new SupplierInvoiceApi();
String supplierInvoiceId = null; // String | 
SupplierInvoiceStatusUpdate supplierInvoiceStatusUpdate = new SupplierInvoiceStatusUpdate(); // SupplierInvoiceStatusUpdate | 
try {
    SupplierInvoice result = apiInstance.updateSupplierInvoiceStatus(supplierInvoiceId, supplierInvoiceStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupplierInvoiceApi#updateSupplierInvoiceStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **supplierInvoiceId** | **String**|  | [default to null]
 **supplierInvoiceStatusUpdate** | [**SupplierInvoiceStatusUpdate**](SupplierInvoiceStatusUpdate.md)|  |

### Return type

[**SupplierInvoice**](SupplierInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

