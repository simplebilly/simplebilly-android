# KstApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**kstApi**](KstApi.md#kstApi) | **GET** /api/v1/bookkeeping/kst | 



## kstApi

> KstErgebnis kstApi(year, gewinn)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KstApi;

KstApi apiInstance = new KstApi();
Integer year = null; // Integer | 
String gewinn = null; // String | 
try {
    KstErgebnis result = apiInstance.kstApi(year, gewinn);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KstApi#kstApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]
 **gewinn** | **String**|  | [optional] [default to null]

### Return type

[**KstErgebnis**](KstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

