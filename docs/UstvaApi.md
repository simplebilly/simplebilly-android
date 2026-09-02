# UstvaApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**jahresustApi**](UstvaApi.md#jahresustApi) | **GET** /api/v1/bookkeeping/jahresust | 
[**ustvaApi**](UstvaApi.md#ustvaApi) | **GET** /api/v1/bookkeeping/ustva | 



## jahresustApi

> JahresUstErgebnis jahresustApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.UstvaApi;

UstvaApi apiInstance = new UstvaApi();
Integer year = null; // Integer | 
try {
    JahresUstErgebnis result = apiInstance.jahresustApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UstvaApi#jahresustApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**JahresUstErgebnis**](JahresUstErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## ustvaApi

> UstvaErgebnis ustvaApi(zeitraum)



### Example

```java
// Import classes:
//import org.openapitools.client.api.UstvaApi;

UstvaApi apiInstance = new UstvaApi();
String zeitraum = null; // String | 
try {
    UstvaErgebnis result = apiInstance.ustvaApi(zeitraum);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UstvaApi#ustvaApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zeitraum** | **String**|  | [default to null]

### Return type

[**UstvaErgebnis**](UstvaErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

