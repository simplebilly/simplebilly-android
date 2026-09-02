# CreditNoteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCreditNote**](CreditNoteApi.md#createCreditNote) | **POST** /api/v1/credit-notes | 
[**downloadCreditNotePdf**](CreditNoteApi.md#downloadCreditNotePdf) | **GET** /api/v1/credit-notes/{credit_note_id}/pdf | 
[**getCreditNote**](CreditNoteApi.md#getCreditNote) | **GET** /api/v1/credit-notes/{credit_note_id} | 
[**listCreditNotes**](CreditNoteApi.md#listCreditNotes) | **GET** /api/v1/credit-notes/ | 



## createCreditNote

> Invoice createCreditNote(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CreditNoteApi;

CreditNoteApi apiInstance = new CreditNoteApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Invoice result = apiInstance.createCreditNote(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CreditNoteApi#createCreditNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## downloadCreditNotePdf

> downloadCreditNotePdf(creditNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CreditNoteApi;

CreditNoteApi apiInstance = new CreditNoteApi();
String creditNoteId = null; // String | 
try {
    apiInstance.downloadCreditNotePdf(creditNoteId);
} catch (ApiException e) {
    System.err.println("Exception when calling CreditNoteApi#downloadCreditNotePdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **creditNoteId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json


## getCreditNote

> Invoice getCreditNote(creditNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CreditNoteApi;

CreditNoteApi apiInstance = new CreditNoteApi();
String creditNoteId = null; // String | 
try {
    Invoice result = apiInstance.getCreditNote(creditNoteId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CreditNoteApi#getCreditNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **creditNoteId** | **String**|  | [default to null]

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listCreditNotes

> List&lt;Invoice&gt; listCreditNotes(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CreditNoteApi;

CreditNoteApi apiInstance = new CreditNoteApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Invoice> result = apiInstance.listCreditNotes(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CreditNoteApi#listCreditNotes");
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

