# QuotationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createQuotation**](QuotationApi.md#createQuotation) | **POST** /api/v1/quotations | 
[**deleteQuotation**](QuotationApi.md#deleteQuotation) | **DELETE** /api/v1/quotations/{quotation_id} | 
[**downloadQuotationPdf**](QuotationApi.md#downloadQuotationPdf) | **GET** /api/v1/quotations/{quotation_id}/pdf | 
[**getQuotation**](QuotationApi.md#getQuotation) | **GET** /api/v1/quotations/{quotation_id} | 
[**listQuotations**](QuotationApi.md#listQuotations) | **GET** /api/v1/quotations/ | 
[**pursueQuotation**](QuotationApi.md#pursueQuotation) | **POST** /api/v1/quotations/{quotation_id}/pursue | 
[**quotationRestore**](QuotationApi.md#quotationRestore) | **POST** /api/v1/quotations/{quotation_id}/restore | 
[**updateQuotation**](QuotationApi.md#updateQuotation) | **PUT** /api/v1/quotations/{quotation_id} | 



## createQuotation

> Quotation createQuotation(quotationCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
QuotationCreate quotationCreate = new QuotationCreate(); // QuotationCreate | 
try {
    Quotation result = apiInstance.createQuotation(quotationCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#createQuotation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationCreate** | [**QuotationCreate**](QuotationCreate.md)|  |

### Return type

[**Quotation**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteQuotation

> deleteQuotation(quotationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
String quotationId = null; // String | 
try {
    apiInstance.deleteQuotation(quotationId);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#deleteQuotation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## downloadQuotationPdf

> downloadQuotationPdf(quotationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
String quotationId = null; // String | 
try {
    apiInstance.downloadQuotationPdf(quotationId);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#downloadQuotationPdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json


## getQuotation

> Quotation getQuotation(quotationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
String quotationId = null; // String | 
try {
    Quotation result = apiInstance.getQuotation(quotationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#getQuotation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationId** | **String**|  | [default to null]

### Return type

[**Quotation**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listQuotations

> List&lt;Quotation&gt; listQuotations(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Quotation> result = apiInstance.listQuotations(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#listQuotations");
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

[**List&lt;Quotation&gt;**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## pursueQuotation

> OrderConfirmation pursueQuotation(quotationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
String quotationId = null; // String | 
try {
    OrderConfirmation result = apiInstance.pursueQuotation(quotationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#pursueQuotation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationId** | **String**|  | [default to null]

### Return type

[**OrderConfirmation**](OrderConfirmation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## quotationRestore

> Quotation quotationRestore(quotationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
String quotationId = null; // String | 
try {
    Quotation result = apiInstance.quotationRestore(quotationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#quotationRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationId** | **String**|  | [default to null]

### Return type

[**Quotation**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateQuotation

> Quotation updateQuotation(quotationId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.QuotationApi;

QuotationApi apiInstance = new QuotationApi();
String quotationId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Quotation result = apiInstance.updateQuotation(quotationId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling QuotationApi#updateQuotation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotationId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Quotation**](Quotation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

