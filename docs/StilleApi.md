# StilleApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**stilleExportApi**](StilleApi.md#stilleExportApi) | **GET** /api/v1/bookkeeping/stille/export | 
[**stilleReportApi**](StilleApi.md#stilleReportApi) | **GET** /api/v1/bookkeeping/stille/report | 



## stilleExportApi

> StilleExportResponse stilleExportApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StilleApi;

StilleApi apiInstance = new StilleApi();
Integer year = null; // Integer | 
try {
    StilleExportResponse result = apiInstance.stilleExportApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StilleApi#stilleExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**StilleExportResponse**](StilleExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## stilleReportApi

> StilleReport stilleReportApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StilleApi;

StilleApi apiInstance = new StilleApi();
Integer year = null; // Integer | 
try {
    StilleReport result = apiInstance.stilleReportApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StilleApi#stilleReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**StilleReport**](StilleReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

