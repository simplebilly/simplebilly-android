# KostenVorschauApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**kostenVorschauApi**](KostenVorschauApi.md#kostenVorschauApi) | **GET** /api/v1/bookkeeping/kosten-vorschau | 



## kostenVorschauApi

> KostenVorschau kostenVorschauApi(year, month)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KostenVorschauApi;

KostenVorschauApi apiInstance = new KostenVorschauApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
try {
    KostenVorschau result = apiInstance.kostenVorschauApi(year, month);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KostenVorschauApi#kostenVorschauApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]
 **month** | **Integer**|  | [default to null]

### Return type

[**KostenVorschau**](KostenVorschau.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

