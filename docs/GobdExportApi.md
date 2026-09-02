# GobdExportApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**buchhalterCsvApi**](GobdExportApi.md#buchhalterCsvApi) | **GET** /api/v1/bookkeeping/buchhalter-csv | 
[**gobdExportApi**](GobdExportApi.md#gobdExportApi) | **GET** /api/v1/bookkeeping/gobd | GoBD/GDPdU export. Default: ZIP archive (&#x60;index.xml&#x60; + CSV tables, IDEA format). &#x60;?format&#x3D;csv&#x60; returns the legacy single-journal CSV as JSON.



## buchhalterCsvApi

> GoBDExportResponse buchhalterCsvApi(dateFrom, dateTo)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GobdExportApi;

GobdExportApi apiInstance = new GobdExportApi();
String dateFrom = null; // String | 
String dateTo = null; // String | 
try {
    GoBDExportResponse result = apiInstance.buchhalterCsvApi(dateFrom, dateTo);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GobdExportApi#buchhalterCsvApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dateFrom** | **String**|  | [default to null]
 **dateTo** | **String**|  | [default to null]

### Return type

[**GoBDExportResponse**](GoBDExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## gobdExportApi

> gobdExportApi(year, format)

GoBD/GDPdU export. Default: ZIP archive (&#x60;index.xml&#x60; + CSV tables, IDEA format). &#x60;?format&#x3D;csv&#x60; returns the legacy single-journal CSV as JSON.

### Example

```java
// Import classes:
//import org.openapitools.client.api.GobdExportApi;

GobdExportApi apiInstance = new GobdExportApi();
Integer year = null; // Integer | 
String format = zip; // String | Export format: `zip` (default, full GDPdU/IDEA export) or `csv` (legacy single-journal CSV as JSON).
try {
    apiInstance.gobdExportApi(year, format);
} catch (ApiException e) {
    System.err.println("Exception when calling GobdExportApi#gobdExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]
 **format** | **String**| Export format: &#x60;zip&#x60; (default, full GDPdU/IDEA export) or &#x60;csv&#x60; (legacy single-journal CSV as JSON). | [optional] [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/zip, application/json

