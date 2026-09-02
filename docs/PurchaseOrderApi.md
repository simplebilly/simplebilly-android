# PurchaseOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPurchaseOrder**](PurchaseOrderApi.md#createPurchaseOrder) | **POST** /api/v1/purchase-orders | 
[**deletePurchaseOrder**](PurchaseOrderApi.md#deletePurchaseOrder) | **DELETE** /api/v1/purchase-orders/{purchase_order_id} | 
[**getPurchaseOrder**](PurchaseOrderApi.md#getPurchaseOrder) | **GET** /api/v1/purchase-orders/{purchase_order_id} | 
[**listPurchaseOrders**](PurchaseOrderApi.md#listPurchaseOrders) | **GET** /api/v1/purchase-orders/ | 
[**matchInvoice**](PurchaseOrderApi.md#matchInvoice) | **POST** /api/v1/purchase-orders/{purchase_order_id}/match-invoice | 3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.
[**updatePurchaseOrder**](PurchaseOrderApi.md#updatePurchaseOrder) | **PUT** /api/v1/purchase-orders/{purchase_order_id} | 
[**updatePurchaseOrderStatus**](PurchaseOrderApi.md#updatePurchaseOrderStatus) | **PUT** /api/v1/purchase-orders/{purchase_order_id}/status | 



## createPurchaseOrder

> PurchaseOrder createPurchaseOrder(purchaseOrder)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
PurchaseOrder purchaseOrder = new PurchaseOrder(); // PurchaseOrder | 
try {
    PurchaseOrder result = apiInstance.createPurchaseOrder(purchaseOrder);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#createPurchaseOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchaseOrder** | [**PurchaseOrder**](PurchaseOrder.md)|  |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePurchaseOrder

> deletePurchaseOrder(purchaseOrderId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
String purchaseOrderId = null; // String | 
try {
    apiInstance.deletePurchaseOrder(purchaseOrderId);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#deletePurchaseOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchaseOrderId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPurchaseOrder

> PurchaseOrder getPurchaseOrder(purchaseOrderId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
String purchaseOrderId = null; // String | 
try {
    PurchaseOrder result = apiInstance.getPurchaseOrder(purchaseOrderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#getPurchaseOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchaseOrderId** | **String**|  | [default to null]

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPurchaseOrders

> List&lt;PurchaseOrder&gt; listPurchaseOrders(page, pageSize, status, supplierName, search)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String supplierName = null; // String | 
String search = null; // String | 
try {
    List<PurchaseOrder> result = apiInstance.listPurchaseOrders(page, pageSize, status, supplierName, search);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#listPurchaseOrders");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **supplierName** | **String**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;PurchaseOrder&gt;**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## matchInvoice

> OasAnyTypeNotMapped matchInvoice(purchaseOrderId, invoiceMatchRequest)

3-way invoice check (Rechnungsprüfung): compares the purchase order line items, the quantities received via goods receipts, and the supplier invoice line items, reporting quantity and price variances per product.

### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
String purchaseOrderId = null; // String | 
InvoiceMatchRequest invoiceMatchRequest = new InvoiceMatchRequest(); // InvoiceMatchRequest | 
try {
    OasAnyTypeNotMapped result = apiInstance.matchInvoice(purchaseOrderId, invoiceMatchRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#matchInvoice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchaseOrderId** | **String**|  | [default to null]
 **invoiceMatchRequest** | [**InvoiceMatchRequest**](InvoiceMatchRequest.md)|  |

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updatePurchaseOrder

> PurchaseOrder updatePurchaseOrder(purchaseOrderId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
String purchaseOrderId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    PurchaseOrder result = apiInstance.updatePurchaseOrder(purchaseOrderId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#updatePurchaseOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchaseOrderId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updatePurchaseOrderStatus

> PurchaseOrder updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PurchaseOrderApi;

PurchaseOrderApi apiInstance = new PurchaseOrderApi();
String purchaseOrderId = null; // String | 
PurchaseOrderStatusUpdate purchaseOrderStatusUpdate = new PurchaseOrderStatusUpdate(); // PurchaseOrderStatusUpdate | 
try {
    PurchaseOrder result = apiInstance.updatePurchaseOrderStatus(purchaseOrderId, purchaseOrderStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PurchaseOrderApi#updatePurchaseOrderStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **purchaseOrderId** | **String**|  | [default to null]
 **purchaseOrderStatusUpdate** | [**PurchaseOrderStatusUpdate**](PurchaseOrderStatusUpdate.md)|  |

### Return type

[**PurchaseOrder**](PurchaseOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

