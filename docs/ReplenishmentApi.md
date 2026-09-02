# ReplenishmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**applyReplenishments**](ReplenishmentApi.md#applyReplenishments) | **POST** /api/v1/replenishments/apply | Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.
[**getReplenishments**](ReplenishmentApi.md#getReplenishments) | **GET** /api/v1/replenishments | 



## applyReplenishments

> OasAnyTypeNotMapped applyReplenishments(targetWarehouseId, sourceWarehouseId)

Create one draft stock transfer per (source → target) pair carrying all suggested product lines for that pair.

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReplenishmentApi;

ReplenishmentApi apiInstance = new ReplenishmentApi();
String targetWarehouseId = null; // String | Warehouse to be replenished. Defaults to the tenant's default warehouse.
String sourceWarehouseId = null; // String | Restrict source warehouses to this id.
try {
    OasAnyTypeNotMapped result = apiInstance.applyReplenishments(targetWarehouseId, sourceWarehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReplenishmentApi#applyReplenishments");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **targetWarehouseId** | **String**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] [default to null]
 **sourceWarehouseId** | **String**| Restrict source warehouses to this id. | [optional] [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getReplenishments

> ReplenishmentResponse getReplenishments(targetWarehouseId, sourceWarehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReplenishmentApi;

ReplenishmentApi apiInstance = new ReplenishmentApi();
String targetWarehouseId = null; // String | Warehouse to be replenished. Defaults to the tenant's default warehouse.
String sourceWarehouseId = null; // String | Restrict source warehouses to this id.
try {
    ReplenishmentResponse result = apiInstance.getReplenishments(targetWarehouseId, sourceWarehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReplenishmentApi#getReplenishments");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **targetWarehouseId** | **String**| Warehouse to be replenished. Defaults to the tenant&#39;s default warehouse. | [optional] [default to null]
 **sourceWarehouseId** | **String**| Restrict source warehouses to this id. | [optional] [default to null]

### Return type

[**ReplenishmentResponse**](ReplenishmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

