# PaygapApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**paygapAuskunftApi**](PaygapApi.md#paygapAuskunftApi) | **GET** /api/v1/bookkeeping/paygap/auskunft/{employee_id} | 
[**paygapExportApi**](PaygapApi.md#paygapExportApi) | **GET** /api/v1/bookkeeping/paygap/export | 
[**paygapReportApi**](PaygapApi.md#paygapReportApi) | **GET** /api/v1/bookkeeping/paygap/report | 



## paygapAuskunftApi

> PayGapInfoResponse paygapAuskunftApi(employeeId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaygapApi;

PaygapApi apiInstance = new PaygapApi();
UUID employeeId = null; // UUID | 
try {
    PayGapInfoResponse result = apiInstance.paygapAuskunftApi(employeeId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaygapApi#paygapAuskunftApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **employeeId** | **UUID**|  | [default to null]

### Return type

[**PayGapInfoResponse**](PayGapInfoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## paygapExportApi

> PayGapExportResponse paygapExportApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaygapApi;

PaygapApi apiInstance = new PaygapApi();
try {
    PayGapExportResponse result = apiInstance.paygapExportApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaygapApi#paygapExportApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**PayGapExportResponse**](PayGapExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## paygapReportApi

> PayGapReport paygapReportApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaygapApi;

PaygapApi apiInstance = new PaygapApi();
try {
    PayGapReport result = apiInstance.paygapReportApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaygapApi#paygapReportApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**PayGapReport**](PayGapReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

