# FristenApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**fristenApi**](FristenApi.md#fristenApi) | **GET** /api/v1/bookkeeping/fristen | 



## fristenApi

> FristenErgebnis fristenApi(bundesland, voranmeldungsrhythmus, dauerfristverlaengerung, estAktiv, gewstAktiv, monate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.FristenApi;

FristenApi apiInstance = new FristenApi();
String bundesland = null; // String | 
String voranmeldungsrhythmus = null; // String | 
Boolean dauerfristverlaengerung = null; // Boolean | 
Boolean estAktiv = null; // Boolean | 
Boolean gewstAktiv = null; // Boolean | 
Integer monate = null; // Integer | 
try {
    FristenErgebnis result = apiInstance.fristenApi(bundesland, voranmeldungsrhythmus, dauerfristverlaengerung, estAktiv, gewstAktiv, monate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling FristenApi#fristenApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bundesland** | **String**|  | [optional] [default to null]
 **voranmeldungsrhythmus** | **String**|  | [optional] [default to null]
 **dauerfristverlaengerung** | **Boolean**|  | [optional] [default to null]
 **estAktiv** | **Boolean**|  | [optional] [default to null]
 **gewstAktiv** | **Boolean**|  | [optional] [default to null]
 **monate** | **Integer**|  | [optional] [default to null]

### Return type

[**FristenErgebnis**](FristenErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

