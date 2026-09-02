# OssReportApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**ossReportApi**](OssReportApi.md#ossReportApi) | **GET** /api/v1/bookkeeping/oss | 



## ossReportApi

> OssReport ossReportApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.OssReportApi;

OssReportApi apiInstance = new OssReportApi();
try {
    OssReport result = apiInstance.ossReportApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OssReportApi#ossReportApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OssReport**](OssReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

