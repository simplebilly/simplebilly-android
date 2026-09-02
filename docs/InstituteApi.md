# InstituteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**instituteStatusApi**](InstituteApi.md#instituteStatusApi) | **GET** /api/v1/bookkeeping/institute/status | 



## instituteStatusApi

> InstituteStatus instituteStatusApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.InstituteApi;

InstituteApi apiInstance = new InstituteApi();
try {
    InstituteStatus result = apiInstance.instituteStatusApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InstituteApi#instituteStatusApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**InstituteStatus**](InstituteStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

