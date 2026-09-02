# EbilanzApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ebilanzReportApi**](EbilanzApi.md#ebilanzReportApi) | **GET** /api/v1/bookkeeping/ebilanz | 
[**ebilanzXbrlExportApi**](EbilanzApi.md#ebilanzXbrlExportApi) | **GET** /api/v1/bookkeeping/ebilanz/xbrl | 



## ebilanzReportApi

> EBilanzReport ebilanzReportApi(year, dateFrom, dateTo)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EbilanzApi;

EbilanzApi apiInstance = new EbilanzApi();
Integer year = null; // Integer | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
try {
    EBilanzReport result = apiInstance.ebilanzReportApi(year, dateFrom, dateTo);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EbilanzApi#ebilanzReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]

### Return type

[**EBilanzReport**](EBilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## ebilanzXbrlExportApi

> ebilanzXbrlExportApi(year, dateFrom, dateTo)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EbilanzApi;

EbilanzApi apiInstance = new EbilanzApi();
Integer year = null; // Integer | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
try {
    apiInstance.ebilanzXbrlExportApi(year, dateFrom, dateTo);
} catch (ApiException e) {
    System.err.println("Exception when calling EbilanzApi#ebilanzXbrlExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/xml

