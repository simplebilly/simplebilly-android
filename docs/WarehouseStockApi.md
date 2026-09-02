# WarehouseStockApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createWarehouseStock**](WarehouseStockApi.md#createWarehouseStock) | **POST** /api/v1/warehouses/{warehouse_id}/stock | 
[**deleteWarehouseStock**](WarehouseStockApi.md#deleteWarehouseStock) | **DELETE** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 
[**listWarehouseStock**](WarehouseStockApi.md#listWarehouseStock) | **GET** /api/v1/warehouses/{warehouse_id}/stock | 
[**updateWarehouseStock**](WarehouseStockApi.md#updateWarehouseStock) | **PUT** /api/v1/warehouses/{warehouse_id}/stock/{product_id} | 



## createWarehouseStock

> WarehouseStock createWarehouseStock(warehouseId, stockAdjustment)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseStockApi;

WarehouseStockApi apiInstance = new WarehouseStockApi();
String warehouseId = null; // String | 
StockAdjustment stockAdjustment = new StockAdjustment(); // StockAdjustment | 
try {
    WarehouseStock result = apiInstance.createWarehouseStock(warehouseId, stockAdjustment);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseStockApi#createWarehouseStock");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]
 **stockAdjustment** | [**StockAdjustment**](StockAdjustment.md)|  |

### Return type

[**WarehouseStock**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteWarehouseStock

> deleteWarehouseStock(warehouseId, productId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseStockApi;

WarehouseStockApi apiInstance = new WarehouseStockApi();
String warehouseId = null; // String | 
UUID productId = null; // UUID | 
try {
    apiInstance.deleteWarehouseStock(warehouseId, productId);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseStockApi#deleteWarehouseStock");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]
 **productId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listWarehouseStock

> List&lt;WarehouseStock&gt; listWarehouseStock(warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseStockApi;

WarehouseStockApi apiInstance = new WarehouseStockApi();
String warehouseId = null; // String | 
try {
    List<WarehouseStock> result = apiInstance.listWarehouseStock(warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseStockApi#listWarehouseStock");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]

### Return type

[**List&lt;WarehouseStock&gt;**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateWarehouseStock

> WarehouseStock updateWarehouseStock(warehouseId, productId, stockAdjustment)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseStockApi;

WarehouseStockApi apiInstance = new WarehouseStockApi();
String warehouseId = null; // String | 
UUID productId = null; // UUID | 
StockAdjustment stockAdjustment = new StockAdjustment(); // StockAdjustment | 
try {
    WarehouseStock result = apiInstance.updateWarehouseStock(warehouseId, productId, stockAdjustment);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseStockApi#updateWarehouseStock");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]
 **productId** | **UUID**|  | [default to null]
 **stockAdjustment** | [**StockAdjustment**](StockAdjustment.md)|  |

### Return type

[**WarehouseStock**](WarehouseStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

