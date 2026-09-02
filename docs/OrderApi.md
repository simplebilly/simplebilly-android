# OrderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**addOrderTags**](OrderApi.md#addOrderTags) | **POST** /api/v1/orders/{order_id}/tags | 
[**findOrderByExternalRef**](OrderApi.md#findOrderByExternalRef) | **GET** /api/v1/orders/by-ext-ref/{ext_ref} | 
[**getOrder**](OrderApi.md#getOrder) | **GET** /api/v1/order/{order_number} | 
[**getOrders**](OrderApi.md#getOrders) | **GET** /api/v1/orders | 
[**patchOrder**](OrderApi.md#patchOrder) | **PATCH** /api/v1/orders/{order_id} | 
[**replaceOrderTags**](OrderApi.md#replaceOrderTags) | **PUT** /api/v1/orders/{order_id}/tags | 
[**updateOrderState**](OrderApi.md#updateOrderState) | **PUT** /api/v1/orders/{order_id}/state | 



## addOrderTags

> Order addOrderTags(orderId, orderTagsRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
String orderId = null; // String | 
OrderTagsRequest orderTagsRequest = new OrderTagsRequest(); // OrderTagsRequest | 
try {
    Order result = apiInstance.addOrderTags(orderId, orderTagsRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#addOrderTags");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**|  | [default to null]
 **orderTagsRequest** | [**OrderTagsRequest**](OrderTagsRequest.md)|  |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## findOrderByExternalRef

> Order findOrderByExternalRef(extRef)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
String extRef = null; // String | 
try {
    Order result = apiInstance.findOrderByExternalRef(extRef);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#findOrderByExternalRef");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **extRef** | **String**|  | [default to null]

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrder

> Order getOrder(orderNumber)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
String orderNumber = null; // String | 
try {
    Order result = apiInstance.getOrder(orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#getOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOrders

> List&lt;Order&gt; getOrders(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Order> result = apiInstance.getOrders(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#getOrders");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **includeDeleted** | **Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] [default to null]

### Return type

[**List&lt;Order&gt;**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## patchOrder

> Order patchOrder(orderId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
String orderId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Order result = apiInstance.patchOrder(orderId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#patchOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## replaceOrderTags

> Order replaceOrderTags(orderId, orderTagsRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
String orderId = null; // String | 
OrderTagsRequest orderTagsRequest = new OrderTagsRequest(); // OrderTagsRequest | 
try {
    Order result = apiInstance.replaceOrderTags(orderId, orderTagsRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#replaceOrderTags");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**|  | [default to null]
 **orderTagsRequest** | [**OrderTagsRequest**](OrderTagsRequest.md)|  |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateOrderState

> Order updateOrderState(orderId, orderStateUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OrderApi;

OrderApi apiInstance = new OrderApi();
String orderId = null; // String | 
OrderStateUpdate orderStateUpdate = new OrderStateUpdate(); // OrderStateUpdate | 
try {
    Order result = apiInstance.updateOrderState(orderId, orderStateUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OrderApi#updateOrderState");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderId** | **String**|  | [default to null]
 **orderStateUpdate** | [**OrderStateUpdate**](OrderStateUpdate.md)|  |

### Return type

[**Order**](Order.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

