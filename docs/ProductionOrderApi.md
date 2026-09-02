# ProductionOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductionOrder**](ProductionOrderApi.md#createProductionOrder) | **POST** /api/v1/production-orders | 
[**deleteProductionOrder**](ProductionOrderApi.md#deleteProductionOrder) | **DELETE** /api/v1/production-orders/{production_order_id} | 
[**getProductionOrder**](ProductionOrderApi.md#getProductionOrder) | **GET** /api/v1/production-orders/{production_order_id} | 
[**listProductionOrders**](ProductionOrderApi.md#listProductionOrders) | **GET** /api/v1/production-orders/ | 
[**productionOrderCosting**](ProductionOrderApi.md#productionOrderCosting) | **GET** /api/v1/production-orders/{production_order_id}/costing | Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price.
[**updateProductionOrder**](ProductionOrderApi.md#updateProductionOrder) | **PUT** /api/v1/production-orders/{production_order_id} | 
[**updateProductionOrderStatus**](ProductionOrderApi.md#updateProductionOrderStatus) | **PUT** /api/v1/production-orders/{production_order_id}/status | 



## createProductionOrder

> ProductionOrder createProductionOrder(productionOrder)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
ProductionOrder productionOrder = new ProductionOrder(); // ProductionOrder | 
try {
    ProductionOrder result = apiInstance.createProductionOrder(productionOrder);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#createProductionOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productionOrder** | [**ProductionOrder**](ProductionOrder.md)|  |

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductionOrder

> deleteProductionOrder(productionOrderId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
UUID productionOrderId = null; // UUID | 
try {
    apiInstance.deleteProductionOrder(productionOrderId);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#deleteProductionOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productionOrderId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductionOrder

> ProductionOrder getProductionOrder(productionOrderId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
UUID productionOrderId = null; // UUID | 
try {
    ProductionOrder result = apiInstance.getProductionOrder(productionOrderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#getProductionOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productionOrderId** | **UUID**|  | [default to null]

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductionOrders

> List&lt;ProductionOrder&gt; listProductionOrders(page, pageSize, search, status)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
String status = null; // String | Filter by status.
try {
    List<ProductionOrder> result = apiInstance.listProductionOrders(page, pageSize, search, status);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#listProductionOrders");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **status** | **String**| Filter by status. | [optional] [default to null]

### Return type

[**List&lt;ProductionOrder&gt;**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## productionOrderCosting

> ProductionOrderCosting productionOrderCosting(productionOrderId)

Actual-costing report (Nachkalkulation) — material costs from BOM components at their purchase price plus the resulting per-unit cost and margin against the finished product&#39;s sale price.

### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
UUID productionOrderId = null; // UUID | 
try {
    ProductionOrderCosting result = apiInstance.productionOrderCosting(productionOrderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#productionOrderCosting");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productionOrderId** | **UUID**|  | [default to null]

### Return type

[**ProductionOrderCosting**](ProductionOrderCosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductionOrder

> ProductionOrder updateProductionOrder(productionOrderId, productionOrder)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
UUID productionOrderId = null; // UUID | 
ProductionOrder productionOrder = new ProductionOrder(); // ProductionOrder | 
try {
    ProductionOrder result = apiInstance.updateProductionOrder(productionOrderId, productionOrder);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#updateProductionOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productionOrderId** | **UUID**|  | [default to null]
 **productionOrder** | [**ProductionOrder**](ProductionOrder.md)|  |

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateProductionOrderStatus

> ProductionOrder updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductionOrderApi;

ProductionOrderApi apiInstance = new ProductionOrderApi();
UUID productionOrderId = null; // UUID | 
ProductionOrderStatusUpdate productionOrderStatusUpdate = new ProductionOrderStatusUpdate(); // ProductionOrderStatusUpdate | 
try {
    ProductionOrder result = apiInstance.updateProductionOrderStatus(productionOrderId, productionOrderStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductionOrderApi#updateProductionOrderStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productionOrderId** | **UUID**|  | [default to null]
 **productionOrderStatusUpdate** | [**ProductionOrderStatusUpdate**](ProductionOrderStatusUpdate.md)|  |

### Return type

[**ProductionOrder**](ProductionOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

