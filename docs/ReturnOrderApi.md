# ReturnOrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createReturnOrder**](ReturnOrderApi.md#createReturnOrder) | **POST** /api/v1/returns | 
[**deleteReturnOrder**](ReturnOrderApi.md#deleteReturnOrder) | **DELETE** /api/v1/returns/{return_order_id} | 
[**getReturnOrder**](ReturnOrderApi.md#getReturnOrder) | **GET** /api/v1/returns/{return_order_id} | 
[**listReturnOrders**](ReturnOrderApi.md#listReturnOrders) | **GET** /api/v1/returns/ | 
[**returnLogisticsQueue**](ReturnOrderApi.md#returnLogisticsQueue) | **GET** /api/v1/returns/logistics-queue | 
[**returnLogisticsSummary**](ReturnOrderApi.md#returnLogisticsSummary) | **GET** /api/v1/returns/logistics-summary | Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.
[**updateReturnOrder**](ReturnOrderApi.md#updateReturnOrder) | **PUT** /api/v1/returns/{return_order_id} | 
[**updateReturnOrderStatus**](ReturnOrderApi.md#updateReturnOrderStatus) | **PUT** /api/v1/returns/{return_order_id}/status | 



## createReturnOrder

> ReturnOrder createReturnOrder(returnOrder)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
ReturnOrder returnOrder = new ReturnOrder(); // ReturnOrder | 
try {
    ReturnOrder result = apiInstance.createReturnOrder(returnOrder);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#createReturnOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnOrder** | [**ReturnOrder**](ReturnOrder.md)|  |

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteReturnOrder

> deleteReturnOrder(returnOrderId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
String returnOrderId = null; // String | 
try {
    apiInstance.deleteReturnOrder(returnOrderId);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#deleteReturnOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnOrderId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getReturnOrder

> ReturnOrder getReturnOrder(returnOrderId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
String returnOrderId = null; // String | 
try {
    ReturnOrder result = apiInstance.getReturnOrder(returnOrderId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#getReturnOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnOrderId** | **String**|  | [default to null]

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listReturnOrders

> List&lt;ReturnOrder&gt; listReturnOrders(page, pageSize, status, customerName, orderNumber)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String customerName = null; // String | 
String orderNumber = null; // String | 
try {
    List<ReturnOrder> result = apiInstance.listReturnOrders(page, pageSize, status, customerName, orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#listReturnOrders");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **customerName** | **String**|  | [optional] [default to null]
 **orderNumber** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;ReturnOrder&gt;**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## returnLogisticsQueue

> List&lt;ReturnLogisticsQueueItem&gt; returnLogisticsQueue()



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
try {
    List<ReturnLogisticsQueueItem> result = apiInstance.returnLogisticsQueue();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#returnLogisticsQueue");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;ReturnLogisticsQueueItem&gt;**](ReturnLogisticsQueueItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## returnLogisticsSummary

> ReturnLogisticsSummary returnLogisticsSummary()

Returns-logistics aggregation for the dashboard: quantities received, restocked and scrapped per warehouse.

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
try {
    ReturnLogisticsSummary result = apiInstance.returnLogisticsSummary();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#returnLogisticsSummary");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ReturnLogisticsSummary**](ReturnLogisticsSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateReturnOrder

> ReturnOrder updateReturnOrder(returnOrderId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
String returnOrderId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    ReturnOrder result = apiInstance.updateReturnOrder(returnOrderId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#updateReturnOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnOrderId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateReturnOrderStatus

> ReturnOrder updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReturnOrderApi;

ReturnOrderApi apiInstance = new ReturnOrderApi();
String returnOrderId = null; // String | 
ReturnOrderStatusUpdate returnOrderStatusUpdate = new ReturnOrderStatusUpdate(); // ReturnOrderStatusUpdate | 
try {
    ReturnOrder result = apiInstance.updateReturnOrderStatus(returnOrderId, returnOrderStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReturnOrderApi#updateReturnOrderStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **returnOrderId** | **String**|  | [default to null]
 **returnOrderStatusUpdate** | [**ReturnOrderStatusUpdate**](ReturnOrderStatusUpdate.md)|  |

### Return type

[**ReturnOrder**](ReturnOrder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

