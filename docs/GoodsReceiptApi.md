# GoodsReceiptApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createGoodsReceipt**](GoodsReceiptApi.md#createGoodsReceipt) | **POST** /api/v1/goods-receipts | 
[**deleteGoodsReceipt**](GoodsReceiptApi.md#deleteGoodsReceipt) | **DELETE** /api/v1/goods-receipts/{goods_receipt_id} | 
[**getGoodsReceipt**](GoodsReceiptApi.md#getGoodsReceipt) | **GET** /api/v1/goods-receipts/{goods_receipt_id} | 
[**listGoodsReceipts**](GoodsReceiptApi.md#listGoodsReceipts) | **GET** /api/v1/goods-receipts/ | 



## createGoodsReceipt

> GoodsReceipt createGoodsReceipt(goodsReceipt)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GoodsReceiptApi;

GoodsReceiptApi apiInstance = new GoodsReceiptApi();
GoodsReceipt goodsReceipt = new GoodsReceipt(); // GoodsReceipt | 
try {
    GoodsReceipt result = apiInstance.createGoodsReceipt(goodsReceipt);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GoodsReceiptApi#createGoodsReceipt");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **goodsReceipt** | [**GoodsReceipt**](GoodsReceipt.md)|  |

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteGoodsReceipt

> deleteGoodsReceipt(goodsReceiptId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GoodsReceiptApi;

GoodsReceiptApi apiInstance = new GoodsReceiptApi();
String goodsReceiptId = null; // String | 
try {
    apiInstance.deleteGoodsReceipt(goodsReceiptId);
} catch (ApiException e) {
    System.err.println("Exception when calling GoodsReceiptApi#deleteGoodsReceipt");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **goodsReceiptId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getGoodsReceipt

> GoodsReceipt getGoodsReceipt(goodsReceiptId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GoodsReceiptApi;

GoodsReceiptApi apiInstance = new GoodsReceiptApi();
String goodsReceiptId = null; // String | 
try {
    GoodsReceipt result = apiInstance.getGoodsReceipt(goodsReceiptId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GoodsReceiptApi#getGoodsReceipt");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **goodsReceiptId** | **String**|  | [default to null]

### Return type

[**GoodsReceipt**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listGoodsReceipts

> List&lt;GoodsReceipt&gt; listGoodsReceipts(page, pageSize, purchaseOrderId, supplierName, warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GoodsReceiptApi;

GoodsReceiptApi apiInstance = new GoodsReceiptApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String purchaseOrderId = null; // String | 
String supplierName = null; // String | 
String warehouseId = null; // String | 
try {
    List<GoodsReceipt> result = apiInstance.listGoodsReceipts(page, pageSize, purchaseOrderId, supplierName, warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GoodsReceiptApi#listGoodsReceipts");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **purchaseOrderId** | **String**|  | [optional] [default to null]
 **supplierName** | **String**|  | [optional] [default to null]
 **warehouseId** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;GoodsReceipt&gt;**](GoodsReceipt.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

