# InventoryValueApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getInventoryValueApi**](InventoryValueApi.md#getInventoryValueApi) | **GET** /api/v1/bookkeeping/inventory-value | 
[**recordInventoryValueApi**](InventoryValueApi.md#recordInventoryValueApi) | **POST** /api/v1/bookkeeping/inventory-value/record | 



## getInventoryValueApi

> CurrentInventoryValue getInventoryValueApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryValueApi;

InventoryValueApi apiInstance = new InventoryValueApi();
try {
    CurrentInventoryValue result = apiInstance.getInventoryValueApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryValueApi#getInventoryValueApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**CurrentInventoryValue**](CurrentInventoryValue.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordInventoryValueApi

> InventoryValuePoint recordInventoryValueApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryValueApi;

InventoryValueApi apiInstance = new InventoryValueApi();
try {
    InventoryValuePoint result = apiInstance.recordInventoryValueApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryValueApi#recordInventoryValueApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**InventoryValuePoint**](InventoryValuePoint.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

