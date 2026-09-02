# PlausibilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**plausibilityCheckApi**](PlausibilityApi.md#plausibilityCheckApi) | **GET** /api/v1/bookkeeping/plausibility | 



## plausibilityCheckApi

> PlausibilityReport plausibilityCheckApi(dateFrom, dateTo)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PlausibilityApi;

PlausibilityApi apiInstance = new PlausibilityApi();
String dateFrom = null; // String | 
String dateTo = null; // String | 
try {
    PlausibilityReport result = apiInstance.plausibilityCheckApi(dateFrom, dateTo);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PlausibilityApi#plausibilityCheckApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **dateFrom** | **String**|  | [optional] [default to null]
 **dateTo** | **String**|  | [optional] [default to null]

### Return type

[**PlausibilityReport**](PlausibilityReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

