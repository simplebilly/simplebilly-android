# InventoryCountApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createInventoryCount**](InventoryCountApi.md#createInventoryCount) | **POST** /api/v1/inventory-counts | 
[**deleteInventoryCount**](InventoryCountApi.md#deleteInventoryCount) | **DELETE** /api/v1/inventory-counts/{inventory_count_id} | 
[**generateInventoryCount**](InventoryCountApi.md#generateInventoryCount) | **POST** /api/v1/inventory-counts/generate | 
[**getInventoryCount**](InventoryCountApi.md#getInventoryCount) | **GET** /api/v1/inventory-counts/{inventory_count_id} | 
[**listInventoryCounts**](InventoryCountApi.md#listInventoryCounts) | **GET** /api/v1/inventory-counts/ | 
[**updateInventoryCount**](InventoryCountApi.md#updateInventoryCount) | **PUT** /api/v1/inventory-counts/{inventory_count_id} | 
[**updateInventoryCountStatus**](InventoryCountApi.md#updateInventoryCountStatus) | **PUT** /api/v1/inventory-counts/{inventory_count_id}/status | 



## createInventoryCount

> InventoryCount createInventoryCount(inventoryCount)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
InventoryCount inventoryCount = new InventoryCount(); // InventoryCount | 
try {
    InventoryCount result = apiInstance.createInventoryCount(inventoryCount);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#createInventoryCount");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventoryCount** | [**InventoryCount**](InventoryCount.md)|  |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteInventoryCount

> deleteInventoryCount(inventoryCountId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
String inventoryCountId = null; // String | 
try {
    apiInstance.deleteInventoryCount(inventoryCountId);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#deleteInventoryCount");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventoryCountId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## generateInventoryCount

> InventoryCount generateInventoryCount(generateCountRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
GenerateCountRequest generateCountRequest = new GenerateCountRequest(); // GenerateCountRequest | 
try {
    InventoryCount result = apiInstance.generateInventoryCount(generateCountRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#generateInventoryCount");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generateCountRequest** | [**GenerateCountRequest**](GenerateCountRequest.md)|  |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getInventoryCount

> InventoryCount getInventoryCount(inventoryCountId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
String inventoryCountId = null; // String | 
try {
    InventoryCount result = apiInstance.getInventoryCount(inventoryCountId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#getInventoryCount");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventoryCountId** | **String**|  | [default to null]

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listInventoryCounts

> List&lt;InventoryCount&gt; listInventoryCounts(page, pageSize, status, warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String warehouseId = null; // String | 
try {
    List<InventoryCount> result = apiInstance.listInventoryCounts(page, pageSize, status, warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#listInventoryCounts");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **warehouseId** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;InventoryCount&gt;**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateInventoryCount

> InventoryCount updateInventoryCount(inventoryCountId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
String inventoryCountId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    InventoryCount result = apiInstance.updateInventoryCount(inventoryCountId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#updateInventoryCount");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventoryCountId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateInventoryCountStatus

> InventoryCount updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.InventoryCountApi;

InventoryCountApi apiInstance = new InventoryCountApi();
String inventoryCountId = null; // String | 
InventoryCountStatusUpdate inventoryCountStatusUpdate = new InventoryCountStatusUpdate(); // InventoryCountStatusUpdate | 
try {
    InventoryCount result = apiInstance.updateInventoryCountStatus(inventoryCountId, inventoryCountStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InventoryCountApi#updateInventoryCountStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inventoryCountId** | **String**|  | [default to null]
 **inventoryCountStatusUpdate** | [**InventoryCountStatusUpdate**](InventoryCountStatusUpdate.md)|  |

### Return type

[**InventoryCount**](InventoryCount.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

