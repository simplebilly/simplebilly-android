# ZugferdApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generateZugferdApi**](ZugferdApi.md#generateZugferdApi) | **GET** /api/v1/invoices/{id}/zugferd | 



## generateZugferdApi

> generateZugferdApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ZugferdApi;

ZugferdApi apiInstance = new ZugferdApi();
String id = null; // String | 
String supplierName = null; // String | 
String supplierStreet = null; // String | 
String supplierCity = null; // String | 
String supplierZip = null; // String | 
String supplierCountry = null; // String | 
String supplierVatId = null; // String | 
try {
    apiInstance.generateZugferdApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId);
} catch (ApiException e) {
    System.err.println("Exception when calling ZugferdApi#generateZugferdApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]
 **supplierName** | **String**|  | [optional] [default to null]
 **supplierStreet** | **String**|  | [optional] [default to null]
 **supplierCity** | **String**|  | [optional] [default to null]
 **supplierZip** | **String**|  | [optional] [default to null]
 **supplierCountry** | **String**|  | [optional] [default to null]
 **supplierVatId** | **String**|  | [optional] [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf

