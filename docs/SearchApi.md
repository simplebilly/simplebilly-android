# SearchApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**globalSearch**](SearchApi.md#globalSearch) | **GET** /api/v1/search | GET /api/v1/search?q&#x3D;...
[**myPermissions**](SearchApi.md#myPermissions) | **GET** /api/v1/me/permissions | GET /api/v1/me/permissions — resolved permissions from the auth token, used by the frontend to show/hide admin navigation.



## globalSearch

> OasAnyTypeNotMapped globalSearch(q)

GET /api/v1/search?q&#x3D;...

### Example

```java
// Import classes:
//import org.openapitools.client.api.SearchApi;

SearchApi apiInstance = new SearchApi();
String q = null; // String | Search text (min 2 chars)
try {
    OasAnyTypeNotMapped result = apiInstance.globalSearch(q);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SearchApi#globalSearch");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **String**| Search text (min 2 chars) | [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## myPermissions

> OasAnyTypeNotMapped myPermissions()

GET /api/v1/me/permissions — resolved permissions from the auth token, used by the frontend to show/hide admin navigation.

### Example

```java
// Import classes:
//import org.openapitools.client.api.SearchApi;

SearchApi apiInstance = new SearchApi();
try {
    OasAnyTypeNotMapped result = apiInstance.myPermissions();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SearchApi#myPermissions");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

