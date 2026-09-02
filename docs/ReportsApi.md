# ReportsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bilanzReportApi**](ReportsApi.md#bilanzReportApi) | **GET** /api/v1/bookkeeping/reports/bilanz | Bilanz (Balance Sheet)
[**guvReportApi**](ReportsApi.md#guvReportApi) | **GET** /api/v1/bookkeeping/reports/guv | Gewinn- und Verlustrechnung (P&amp;L statement)
[**kontenansichtReportApi**](ReportsApi.md#kontenansichtReportApi) | **GET** /api/v1/bookkeeping/reports/kontenansicht | Kontenansicht (Account Overview)
[**umsatzsteuerReportApi**](ReportsApi.md#umsatzsteuerReportApi) | **GET** /api/v1/bookkeeping/reports/umsatzsteuer | Umsatzsteuer-Voranmeldung (VAT report)



## bilanzReportApi

> BilanzReport bilanzReportApi(year, month, dateFrom, dateTo, page, pageSize)

Bilanz (Balance Sheet)

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReportsApi;

ReportsApi apiInstance = new ReportsApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    BilanzReport result = apiInstance.bilanzReportApi(year, month, dateFrom, dateTo, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReportsApi#bilanzReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **month** | **Integer**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**BilanzReport**](BilanzReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## guvReportApi

> GuVReport guvReportApi(year, month, dateFrom, dateTo, page, pageSize)

Gewinn- und Verlustrechnung (P&amp;L statement)

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReportsApi;

ReportsApi apiInstance = new ReportsApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    GuVReport result = apiInstance.guvReportApi(year, month, dateFrom, dateTo, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReportsApi#guvReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **month** | **Integer**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**GuVReport**](GuVReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## kontenansichtReportApi

> KontoReport kontenansichtReportApi(year, month, dateFrom, dateTo, page, pageSize)

Kontenansicht (Account Overview)

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReportsApi;

ReportsApi apiInstance = new ReportsApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    KontoReport result = apiInstance.kontenansichtReportApi(year, month, dateFrom, dateTo, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReportsApi#kontenansichtReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **month** | **Integer**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**KontoReport**](KontoReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## umsatzsteuerReportApi

> UmsatzsteuerReport umsatzsteuerReportApi(year, month, dateFrom, dateTo, page, pageSize)

Umsatzsteuer-Voranmeldung (VAT report)

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReportsApi;

ReportsApi apiInstance = new ReportsApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
String dateFrom = null; // String | 
String dateTo = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    UmsatzsteuerReport result = apiInstance.umsatzsteuerReportApi(year, month, dateFrom, dateTo, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReportsApi#umsatzsteuerReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **month** | **Integer**|  | [optional] [default to null]
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**UmsatzsteuerReport**](UmsatzsteuerReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

