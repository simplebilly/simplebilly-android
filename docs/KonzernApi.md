# KonzernApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**konzernExportApi**](KonzernApi.md#konzernExportApi) | **GET** /api/v1/bookkeeping/konzern/status/export | 
[**konzernStatusApi**](KonzernApi.md#konzernStatusApi) | **GET** /api/v1/bookkeeping/konzern/status | 



## konzernExportApi

> KonzernExportResponse konzernExportApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KonzernApi;

KonzernApi apiInstance = new KonzernApi();
Integer year = null; // Integer | 
try {
    KonzernExportResponse result = apiInstance.konzernExportApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KonzernApi#konzernExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**KonzernExportResponse**](KonzernExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## konzernStatusApi

> KonzernStatus konzernStatusApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KonzernApi;

KonzernApi apiInstance = new KonzernApi();
Integer year = null; // Integer | 
try {
    KonzernStatus result = apiInstance.konzernStatusApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KonzernApi#konzernStatusApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**KonzernStatus**](KonzernStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

