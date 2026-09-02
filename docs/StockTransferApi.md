# StockTransferApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createStockTransfer**](StockTransferApi.md#createStockTransfer) | **POST** /api/v1/stock-transfers | 
[**deleteStockTransfer**](StockTransferApi.md#deleteStockTransfer) | **DELETE** /api/v1/stock-transfers/{stock_transfer_id} | 
[**getStockTransfer**](StockTransferApi.md#getStockTransfer) | **GET** /api/v1/stock-transfers/{stock_transfer_id} | 
[**listStockTransfers**](StockTransferApi.md#listStockTransfers) | **GET** /api/v1/stock-transfers/ | 
[**updateStockTransferStatus**](StockTransferApi.md#updateStockTransferStatus) | **PUT** /api/v1/stock-transfers/{stock_transfer_id}/status | 



## createStockTransfer

> StockTransfer createStockTransfer(stockTransfer)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockTransferApi;

StockTransferApi apiInstance = new StockTransferApi();
StockTransfer stockTransfer = new StockTransfer(); // StockTransfer | 
try {
    StockTransfer result = apiInstance.createStockTransfer(stockTransfer);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StockTransferApi#createStockTransfer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stockTransfer** | [**StockTransfer**](StockTransfer.md)|  |

### Return type

[**StockTransfer**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteStockTransfer

> deleteStockTransfer(stockTransferId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockTransferApi;

StockTransferApi apiInstance = new StockTransferApi();
String stockTransferId = null; // String | 
try {
    apiInstance.deleteStockTransfer(stockTransferId);
} catch (ApiException e) {
    System.err.println("Exception when calling StockTransferApi#deleteStockTransfer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stockTransferId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getStockTransfer

> StockTransfer getStockTransfer(stockTransferId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockTransferApi;

StockTransferApi apiInstance = new StockTransferApi();
String stockTransferId = null; // String | 
try {
    StockTransfer result = apiInstance.getStockTransfer(stockTransferId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StockTransferApi#getStockTransfer");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stockTransferId** | **String**|  | [default to null]

### Return type

[**StockTransfer**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listStockTransfers

> List&lt;StockTransfer&gt; listStockTransfers(page, pageSize, status, warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockTransferApi;

StockTransferApi apiInstance = new StockTransferApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String warehouseId = null; // String | 
try {
    List<StockTransfer> result = apiInstance.listStockTransfers(page, pageSize, status, warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StockTransferApi#listStockTransfers");
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

[**List&lt;StockTransfer&gt;**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateStockTransferStatus

> StockTransfer updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.StockTransferApi;

StockTransferApi apiInstance = new StockTransferApi();
String stockTransferId = null; // String | 
StockTransferStatusUpdate stockTransferStatusUpdate = new StockTransferStatusUpdate(); // StockTransferStatusUpdate | 
try {
    StockTransfer result = apiInstance.updateStockTransferStatus(stockTransferId, stockTransferStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling StockTransferApi#updateStockTransferStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **stockTransferId** | **String**|  | [default to null]
 **stockTransferStatusUpdate** | [**StockTransferStatusUpdate**](StockTransferStatusUpdate.md)|  |

### Return type

[**StockTransfer**](StockTransfer.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

