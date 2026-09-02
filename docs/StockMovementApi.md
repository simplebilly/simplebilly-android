# StockMovementApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getStockMovement**](StockMovementApi.md#getStockMovement) | **GET** /api/v1/stock-movements/{movement_id} | 
[**listStockMovements**](StockMovementApi.md#listStockMovements) | **GET** /api/v1/stock-movements/ | 



## getStockMovement

> StockMovement getStockMovement(movementId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockMovementApi;

StockMovementApi apiInstance = new StockMovementApi();
String movementId = null; // String | 
try {
    StockMovement result = apiInstance.getStockMovement(movementId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StockMovementApi#getStockMovement");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **movementId** | **String**|  | [default to null]

### Return type

[**StockMovement**](StockMovement.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listStockMovements

> List&lt;StockMovement&gt; listStockMovements(page, pageSize, productId, warehouseId, movementType, from, to)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockMovementApi;

StockMovementApi apiInstance = new StockMovementApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
UUID productId = null; // UUID | 
String warehouseId = null; // String | 
String movementType = null; // String | 
Date from = null; // Date | Only movements on or after this date (inclusive).
Date to = null; // Date | Only movements on or before this date (inclusive).
try {
    List<StockMovement> result = apiInstance.listStockMovements(page, pageSize, productId, warehouseId, movementType, from, to);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StockMovementApi#listStockMovements");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **productId** | **UUID**|  | [optional] [default to null]
 **warehouseId** | **String**|  | [optional] [default to null]
 **movementType** | **String**|  | [optional] [default to null]
 **from** | **Date**| Only movements on or after this date (inclusive). | [optional] [default to null]
 **to** | **Date**| Only movements on or before this date (inclusive). | [optional] [default to null]

### Return type

[**List&lt;StockMovement&gt;**](StockMovement.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

