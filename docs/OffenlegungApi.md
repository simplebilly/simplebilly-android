# OffenlegungApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**offenlegungApi**](OffenlegungApi.md#offenlegungApi) | **GET** /api/v1/bookkeeping/offenlegung | 



## offenlegungApi

> OffenlegungReport offenlegungApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.OffenlegungApi;

OffenlegungApi apiInstance = new OffenlegungApi();
try {
    OffenlegungReport result = apiInstance.offenlegungApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OffenlegungApi#offenlegungApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OffenlegungReport**](OffenlegungReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

