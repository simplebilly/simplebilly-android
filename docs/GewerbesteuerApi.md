# GewerbesteuerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gewerbesteuerApi**](GewerbesteuerApi.md#gewerbesteuerApi) | **GET** /api/v1/bookkeeping/gewerbesteuer | 



## gewerbesteuerApi

> GewerbesteuerErgebnis gewerbesteuerApi(year, hebesatz, gewerbeertrag, country, gemeindeschluessel)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GewerbesteuerApi;

GewerbesteuerApi apiInstance = new GewerbesteuerApi();
Integer year = null; // Integer | 
String hebesatz = null; // String | 
String gewerbeertrag = null; // String | 
String country = null; // String | 
String gemeindeschluessel = null; // String | 
try {
    GewerbesteuerErgebnis result = apiInstance.gewerbesteuerApi(year, hebesatz, gewerbeertrag, country, gemeindeschluessel);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GewerbesteuerApi#gewerbesteuerApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]
 **hebesatz** | **String**|  | [optional] [default to null]
 **gewerbeertrag** | **String**|  | [optional] [default to null]
 **country** | **String**|  | [optional] [default to null]
 **gemeindeschluessel** | **String**|  | [optional] [default to null]

### Return type

[**GewerbesteuerErgebnis**](GewerbesteuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

