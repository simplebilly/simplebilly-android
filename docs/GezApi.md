# GezApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**gezApi**](GezApi.md#gezApi) | **GET** /api/v1/bookkeeping/gez | 



## gezApi

> GezReport gezApi(jahr, betriebsstaetten, kfz, hotelzimmer, beschaefigte)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GezApi;

GezApi apiInstance = new GezApi();
Integer jahr = null; // Integer | 
String betriebsstaetten = null; // String | Liste der Betriebsstätten als JSON, z.B. `[{\"name\":\"Filiale 1\",\"beschaefigte\":12}]`.
Long kfz = null; // Long | Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind).
Long hotelzimmer = null; // Long | Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen.
Long beschaefigte = null; // Long | Gesamtzahl der Beschäftigten (verwendet nur, wenn `betriebsstaetten` fehlt; dann wird eine einzelne Betriebsstätte angenommen).
try {
    GezReport result = apiInstance.gezApi(jahr, betriebsstaetten, kfz, hotelzimmer, beschaefigte);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GezApi#gezApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jahr** | **Integer**|  | [optional] [default to null]
 **betriebsstaetten** | **String**| Liste der Betriebsstätten als JSON, z.B. &#x60;[{\&quot;name\&quot;:\&quot;Filiale 1\&quot;,\&quot;beschaefigte\&quot;:12}]&#x60;. | [optional] [default to null]
 **kfz** | **Long**| Gesamtzahl der betrieblich genutzten Kfz (falls keine Betriebsstätten angegeben sind). | [optional] [default to null]
 **hotelzimmer** | **Long**| Gesamtzahl der Hotel-/Gästezimmer und Ferienwohnungen. | [optional] [default to null]
 **beschaefigte** | **Long**| Gesamtzahl der Beschäftigten (verwendet nur, wenn &#x60;betriebsstaetten&#x60; fehlt; dann wird eine einzelne Betriebsstätte angenommen). | [optional] [default to null]

### Return type

[**GezReport**](GezReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

