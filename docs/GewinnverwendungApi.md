# GewinnverwendungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gewinnverwendungApi**](GewinnverwendungApi.md#gewinnverwendungApi) | **GET** /api/v1/bookkeeping/gewinnverwendung | 
[**gewinnverwendungExportApi**](GewinnverwendungApi.md#gewinnverwendungExportApi) | **GET** /api/v1/bookkeeping/gewinnverwendung/export | 



## gewinnverwendungApi

> GewinnverwendungsReport gewinnverwendungApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GewinnverwendungApi;

GewinnverwendungApi apiInstance = new GewinnverwendungApi();
Integer year = null; // Integer | 
try {
    GewinnverwendungsReport result = apiInstance.gewinnverwendungApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GewinnverwendungApi#gewinnverwendungApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**GewinnverwendungsReport**](GewinnverwendungsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## gewinnverwendungExportApi

> GewinnverwendungsExportResponse gewinnverwendungExportApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GewinnverwendungApi;

GewinnverwendungApi apiInstance = new GewinnverwendungApi();
Integer year = null; // Integer | 
try {
    GewinnverwendungsExportResponse result = apiInstance.gewinnverwendungExportApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GewinnverwendungApi#gewinnverwendungExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**GewinnverwendungsExportResponse**](GewinnverwendungsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

