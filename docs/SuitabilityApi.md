# SuitabilityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shippingSuitabilityApi**](SuitabilityApi.md#shippingSuitabilityApi) | **POST** /api/v1/shipping/suitability | 



## shippingSuitabilityApi

> SuitabilityResult shippingSuitabilityApi(suitabilityRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SuitabilityApi;

SuitabilityApi apiInstance = new SuitabilityApi();
SuitabilityRequest suitabilityRequest = new SuitabilityRequest(); // SuitabilityRequest | 
try {
    SuitabilityResult result = apiInstance.shippingSuitabilityApi(suitabilityRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SuitabilityApi#shippingSuitabilityApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **suitabilityRequest** | [**SuitabilityRequest**](SuitabilityRequest.md)|  |

### Return type

[**SuitabilityResult**](SuitabilityResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

