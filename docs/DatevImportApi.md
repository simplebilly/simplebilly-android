# DatevImportApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**datevImportApi**](DatevImportApi.md#datevImportApi) | **POST** /api/v1/bookkeeping/datev/import | 



## datevImportApi

> DatevImportResponse datevImportApi(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DatevImportApi;

DatevImportApi apiInstance = new DatevImportApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    DatevImportResponse result = apiInstance.datevImportApi(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DatevImportApi#datevImportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**DatevImportResponse**](DatevImportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

