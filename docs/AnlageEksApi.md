# AnlageEksApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**eksApi**](AnlageEksApi.md#eksApi) | **GET** /api/v1/bookkeeping/eks | 



## eksApi

> EksErgebnis eksApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AnlageEksApi;

AnlageEksApi apiInstance = new AnlageEksApi();
Integer year = null; // Integer | 
try {
    EksErgebnis result = apiInstance.eksApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnlageEksApi#eksApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**EksErgebnis**](EksErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

