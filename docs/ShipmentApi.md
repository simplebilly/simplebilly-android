# ShipmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShipment**](ShipmentApi.md#createShipment) | **POST** /api/v1/shipments | 
[**createShipmentFromOrder**](ShipmentApi.md#createShipmentFromOrder) | **POST** /api/v1/orders/{order_number}/shipments | Create a real shipment for an order: calls the configured carrier&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped.
[**deleteShipment**](ShipmentApi.md#deleteShipment) | **DELETE** /api/v1/shipments/{shipment_id} | 
[**getShipment**](ShipmentApi.md#getShipment) | **GET** /api/v1/shipments/{shipment_id} | 
[**listShipments**](ShipmentApi.md#listShipments) | **GET** /api/v1/shipments | 
[**trackOrderPublic**](ShipmentApi.md#trackOrderPublic) | **POST** /api/v1/public/track | Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API).
[**trackShipmentApi**](ShipmentApi.md#trackShipmentApi) | **GET** /api/v1/shipments/{shipment_id}/tracking | 
[**updateShipmentStatus**](ShipmentApi.md#updateShipmentStatus) | **PUT** /api/v1/shipments/{shipment_id}/status | 



## createShipment

> Shipment createShipment(shipment)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
Shipment shipment = new Shipment(); // Shipment | 
try {
    Shipment result = apiInstance.createShipment(shipment);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#createShipment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipment** | [**Shipment**](Shipment.md)|  |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createShipmentFromOrder

> Shipment createShipmentFromOrder(orderNumber, createShipmentRequest)

Create a real shipment for an order: calls the configured carrier&#39;s label API, stores the returned tracking/label on a new shipment row, and marks the order as shipped.

### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
String orderNumber = null; // String | 
CreateShipmentRequest createShipmentRequest = new CreateShipmentRequest(); // CreateShipmentRequest | 
try {
    Shipment result = apiInstance.createShipmentFromOrder(orderNumber, createShipmentRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#createShipmentFromOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]
 **createShipmentRequest** | [**CreateShipmentRequest**](CreateShipmentRequest.md)|  |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShipment

> deleteShipment(shipmentId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
String shipmentId = null; // String | 
try {
    apiInstance.deleteShipment(shipmentId);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#deleteShipment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipmentId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShipment

> Shipment getShipment(shipmentId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
String shipmentId = null; // String | 
try {
    Shipment result = apiInstance.getShipment(shipmentId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#getShipment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipmentId** | **String**|  | [default to null]

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listShipments

> List&lt;Shipment&gt; listShipments(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Shipment> result = apiInstance.listShipments(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#listShipments");
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

[**List&lt;Shipment&gt;**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## trackOrderPublic

> TrackOrderResponse trackOrderPublic(trackOrderRequest)

Customer-facing tracking lookup: order number + email → shipment status and live carrier events. No auth (public storefront API).

### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
TrackOrderRequest trackOrderRequest = new TrackOrderRequest(); // TrackOrderRequest | 
try {
    TrackOrderResponse result = apiInstance.trackOrderPublic(trackOrderRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#trackOrderPublic");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **trackOrderRequest** | [**TrackOrderRequest**](TrackOrderRequest.md)|  |

### Return type

[**TrackOrderResponse**](TrackOrderResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## trackShipmentApi

> TrackingInfo trackShipmentApi(shipmentId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
String shipmentId = null; // String | 
try {
    TrackingInfo result = apiInstance.trackShipmentApi(shipmentId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#trackShipmentApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipmentId** | **String**|  | [default to null]

### Return type

[**TrackingInfo**](TrackingInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShipmentStatus

> Shipment updateShipmentStatus(shipmentId, shipmentStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShipmentApi;

ShipmentApi apiInstance = new ShipmentApi();
String shipmentId = null; // String | 
ShipmentStatusUpdate shipmentStatusUpdate = new ShipmentStatusUpdate(); // ShipmentStatusUpdate | 
try {
    Shipment result = apiInstance.updateShipmentStatus(shipmentId, shipmentStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShipmentApi#updateShipmentStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shipmentId** | **String**|  | [default to null]
 **shipmentStatusUpdate** | [**ShipmentStatusUpdate**](ShipmentStatusUpdate.md)|  |

### Return type

[**Shipment**](Shipment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

