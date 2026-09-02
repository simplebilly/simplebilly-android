# ProformaInvoiceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convertProformaToInvoice**](ProformaInvoiceApi.md#convertProformaToInvoice) | **POST** /api/v1/proforma-invoices/{proforma_id}/convert | 
[**createProformaInvoice**](ProformaInvoiceApi.md#createProformaInvoice) | **POST** /api/v1/proforma-invoices | 
[**deleteProformaInvoice**](ProformaInvoiceApi.md#deleteProformaInvoice) | **DELETE** /api/v1/proforma-invoices/{proforma_id} | 
[**getProformaInvoice**](ProformaInvoiceApi.md#getProformaInvoice) | **GET** /api/v1/proforma-invoices/{proforma_id} | 
[**listProformaInvoices**](ProformaInvoiceApi.md#listProformaInvoices) | **GET** /api/v1/proforma-invoices/ | 
[**updateProformaInvoice**](ProformaInvoiceApi.md#updateProformaInvoice) | **PUT** /api/v1/proforma-invoices/{proforma_id} | 



## convertProformaToInvoice

> ConvertResponse convertProformaToInvoice(proformaId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProformaInvoiceApi;

ProformaInvoiceApi apiInstance = new ProformaInvoiceApi();
String proformaId = null; // String | 
try {
    ConvertResponse result = apiInstance.convertProformaToInvoice(proformaId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProformaInvoiceApi#convertProformaToInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proformaId** | **String**|  | [default to null]

### Return type

[**ConvertResponse**](ConvertResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## createProformaInvoice

> ProformaInvoice createProformaInvoice(proformaInvoice)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProformaInvoiceApi;

ProformaInvoiceApi apiInstance = new ProformaInvoiceApi();
ProformaInvoice proformaInvoice = new ProformaInvoice(); // ProformaInvoice | 
try {
    ProformaInvoice result = apiInstance.createProformaInvoice(proformaInvoice);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProformaInvoiceApi#createProformaInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proformaInvoice** | [**ProformaInvoice**](ProformaInvoice.md)|  |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProformaInvoice

> deleteProformaInvoice(proformaId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProformaInvoiceApi;

ProformaInvoiceApi apiInstance = new ProformaInvoiceApi();
String proformaId = null; // String | 
try {
    apiInstance.deleteProformaInvoice(proformaId);
} catch (ApiException e) {
    System.err.println("Exception when calling ProformaInvoiceApi#deleteProformaInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proformaId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProformaInvoice

> ProformaInvoice getProformaInvoice(proformaId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProformaInvoiceApi;

ProformaInvoiceApi apiInstance = new ProformaInvoiceApi();
String proformaId = null; // String | 
try {
    ProformaInvoice result = apiInstance.getProformaInvoice(proformaId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProformaInvoiceApi#getProformaInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proformaId** | **String**|  | [default to null]

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProformaInvoices

> List&lt;ProformaInvoice&gt; listProformaInvoices(page, pageSize, status, customerId, orderNumber)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProformaInvoiceApi;

ProformaInvoiceApi apiInstance = new ProformaInvoiceApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String customerId = null; // String | 
String orderNumber = null; // String | 
try {
    List<ProformaInvoice> result = apiInstance.listProformaInvoices(page, pageSize, status, customerId, orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProformaInvoiceApi#listProformaInvoices");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **customerId** | **String**|  | [optional] [default to null]
 **orderNumber** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;ProformaInvoice&gt;**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProformaInvoice

> ProformaInvoice updateProformaInvoice(proformaId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProformaInvoiceApi;

ProformaInvoiceApi apiInstance = new ProformaInvoiceApi();
String proformaId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    ProformaInvoice result = apiInstance.updateProformaInvoice(proformaId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProformaInvoiceApi#updateProformaInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **proformaId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**ProformaInvoice**](ProformaInvoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

