# WarehouseApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createWarehouse**](WarehouseApi.md#createWarehouse) | **POST** /api/v1/warehouses | 
[**deleteWarehouse**](WarehouseApi.md#deleteWarehouse) | **DELETE** /api/v1/warehouses/{warehouse_id} | 
[**getWarehouse**](WarehouseApi.md#getWarehouse) | **GET** /api/v1/warehouses/{warehouse_id} | 
[**listWarehouses**](WarehouseApi.md#listWarehouses) | **GET** /api/v1/warehouses/ | 
[**updateWarehouse**](WarehouseApi.md#updateWarehouse) | **PUT** /api/v1/warehouses/{warehouse_id} | 



## createWarehouse

> Warehouse createWarehouse(warehouse)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseApi;

WarehouseApi apiInstance = new WarehouseApi();
Warehouse warehouse = new Warehouse(); // Warehouse | 
try {
    Warehouse result = apiInstance.createWarehouse(warehouse);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseApi#createWarehouse");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouse** | [**Warehouse**](Warehouse.md)|  |

### Return type

[**Warehouse**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteWarehouse

> deleteWarehouse(warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseApi;

WarehouseApi apiInstance = new WarehouseApi();
String warehouseId = null; // String | 
try {
    apiInstance.deleteWarehouse(warehouseId);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseApi#deleteWarehouse");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getWarehouse

> Warehouse getWarehouse(warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseApi;

WarehouseApi apiInstance = new WarehouseApi();
String warehouseId = null; // String | 
try {
    Warehouse result = apiInstance.getWarehouse(warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseApi#getWarehouse");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]

### Return type

[**Warehouse**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listWarehouses

> List&lt;Warehouse&gt; listWarehouses(page, pageSize, search, isActive)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseApi;

WarehouseApi apiInstance = new WarehouseApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean isActive = null; // Boolean | 
try {
    List<Warehouse> result = apiInstance.listWarehouses(page, pageSize, search, isActive);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseApi#listWarehouses");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **isActive** | **Boolean**|  | [optional] [default to null]

### Return type

[**List&lt;Warehouse&gt;**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateWarehouse

> Warehouse updateWarehouse(warehouseId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WarehouseApi;

WarehouseApi apiInstance = new WarehouseApi();
String warehouseId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Warehouse result = apiInstance.updateWarehouse(warehouseId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WarehouseApi#updateWarehouse");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **warehouseId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Warehouse**](Warehouse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

