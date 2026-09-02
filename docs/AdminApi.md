# AdminApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**triggerMirror**](AdminApi.md#triggerMirror) | **POST** /api/v1/admin/storage/mirror | 



## triggerMirror

> MirrorTriggerResponse triggerMirror()



### Example

```java
// Import classes:
//import org.openapitools.client.api.AdminApi;

AdminApi apiInstance = new AdminApi();
try {
    MirrorTriggerResponse result = apiInstance.triggerMirror();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AdminApi#triggerMirror");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**MirrorTriggerResponse**](MirrorTriggerResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

