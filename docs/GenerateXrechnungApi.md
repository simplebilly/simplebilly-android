# GenerateXrechnungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generateXrechnungApi**](GenerateXrechnungApi.md#generateXrechnungApi) | **GET** /api/v1/invoices/{id}/xrechnung | 



## generateXrechnungApi

> XRechnungResponse generateXrechnungApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GenerateXrechnungApi;

GenerateXrechnungApi apiInstance = new GenerateXrechnungApi();
String id = null; // String | 
String supplierName = null; // String | 
String supplierStreet = null; // String | 
String supplierCity = null; // String | 
String supplierZip = null; // String | 
String supplierCountry = null; // String | 
String supplierVatId = null; // String | 
try {
    XRechnungResponse result = apiInstance.generateXrechnungApi(id, supplierName, supplierStreet, supplierCity, supplierZip, supplierCountry, supplierVatId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GenerateXrechnungApi#generateXrechnungApi");
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

[**XRechnungResponse**](XRechnungResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

