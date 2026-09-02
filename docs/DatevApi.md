# DatevApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**datevExportApi**](DatevApi.md#datevExportApi) | **GET** /api/v1/bookkeeping/datev/export | Export bookkeeping data as DATEV CSV
[**datevPreviewApi**](DatevApi.md#datevPreviewApi) | **GET** /api/v1/bookkeeping/datev/preview | Exported_datev_bookings: returns formed bookings for review



## datevExportApi

> DatevExportResponse datevExportApi(accountSchema, dateFrom, dateTo, page, pageSize)

Export bookkeeping data as DATEV CSV

### Example

```java
// Import classes:
//import org.openapitools.client.api.DatevApi;

DatevApi apiInstance = new DatevApi();
String accountSchema = null; // String | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    DatevExportResponse result = apiInstance.datevExportApi(accountSchema, dateFrom, dateTo, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DatevApi#datevExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountSchema** | **String**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**DatevExportResponse**](DatevExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## datevPreviewApi

> List&lt;DatevBookingPreview&gt; datevPreviewApi(accountSchema, dateFrom, dateTo, page, pageSize)

Exported_datev_bookings: returns formed bookings for review

### Example

```java
// Import classes:
//import org.openapitools.client.api.DatevApi;

DatevApi apiInstance = new DatevApi();
String accountSchema = null; // String | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    List<DatevBookingPreview> result = apiInstance.datevPreviewApi(accountSchema, dateFrom, dateTo, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DatevApi#datevPreviewApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **accountSchema** | **String**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**List&lt;DatevBookingPreview&gt;**](DatevBookingPreview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

