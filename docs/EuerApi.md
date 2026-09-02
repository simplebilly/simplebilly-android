# EuerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**euerApi**](EuerApi.md#euerApi) | **GET** /api/v1/bookkeeping/euer | 
[**euerKategorienApi**](EuerApi.md#euerKategorienApi) | **GET** /api/v1/bookkeeping/euer/kategorien | 



## euerApi

> EuerErgebnis euerApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EuerApi;

EuerApi apiInstance = new EuerApi();
Integer year = null; // Integer | 
try {
    EuerErgebnis result = apiInstance.euerApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EuerApi#euerApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**EuerErgebnis**](EuerErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## euerKategorienApi

> EuerDetailErgebnis euerKategorienApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EuerApi;

EuerApi apiInstance = new EuerApi();
Integer year = null; // Integer | 
try {
    EuerDetailErgebnis result = apiInstance.euerKategorienApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EuerApi#euerKategorienApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**EuerDetailErgebnis**](EuerDetailErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

