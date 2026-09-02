# PeppolApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**peppolApi**](PeppolApi.md#peppolApi) | **GET** /api/v1/invoices/{id}/peppol | 



## peppolApi

> PeppolResponse peppolApi(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PeppolApi;

PeppolApi apiInstance = new PeppolApi();
String id = null; // String | 
try {
    PeppolResponse result = apiInstance.peppolApi(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PeppolApi#peppolApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

[**PeppolResponse**](PeppolResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

