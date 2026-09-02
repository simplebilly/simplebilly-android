# PackingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**completePacking**](PackingApi.md#completePacking) | **POST** /api/v1/packing/{order_number}/complete | Mark packing as complete and transition order to shipped
[**getPackingQueue**](PackingApi.md#getPackingQueue) | **GET** /api/v1/packing/queue | Get the packing queue - orders ready for packing
[**printDeliveryNote**](PackingApi.md#printDeliveryNote) | **POST** /api/v1/packing/{order_number}/print-delivery-note | Print delivery note (Lieferschein) for an order
[**printLabel**](PackingApi.md#printLabel) | **POST** /api/v1/packing/{order_number}/print-label | Print shipping label for an order
[**recordPackingVideo**](PackingApi.md#recordPackingVideo) | **POST** /api/v1/packing/{order_number}/record-video | Record video of packing process



## completePacking

> PackingCompleteResponse completePacking(orderNumber, packingCompleteRequest)

Mark packing as complete and transition order to shipped

### Example

```java
// Import classes:
//import org.openapitools.client.api.PackingApi;

PackingApi apiInstance = new PackingApi();
String orderNumber = null; // String | 
PackingCompleteRequest packingCompleteRequest = new PackingCompleteRequest(); // PackingCompleteRequest | 
try {
    PackingCompleteResponse result = apiInstance.completePacking(orderNumber, packingCompleteRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PackingApi#completePacking");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]
 **packingCompleteRequest** | [**PackingCompleteRequest**](PackingCompleteRequest.md)|  |

### Return type

[**PackingCompleteResponse**](PackingCompleteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getPackingQueue

> PackingQueue getPackingQueue(page, pageSize, search)

Get the packing queue - orders ready for packing

### Example

```java
// Import classes:
//import org.openapitools.client.api.PackingApi;

PackingApi apiInstance = new PackingApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
try {
    PackingQueue result = apiInstance.getPackingQueue(page, pageSize, search);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PackingApi#getPackingQueue");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]

### Return type

[**PackingQueue**](PackingQueue.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## printDeliveryNote

> PrintDeliveryNoteResponse printDeliveryNote(orderNumber)

Print delivery note (Lieferschein) for an order

### Example

```java
// Import classes:
//import org.openapitools.client.api.PackingApi;

PackingApi apiInstance = new PackingApi();
String orderNumber = null; // String | 
try {
    PrintDeliveryNoteResponse result = apiInstance.printDeliveryNote(orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PackingApi#printDeliveryNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]

### Return type

[**PrintDeliveryNoteResponse**](PrintDeliveryNoteResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## printLabel

> PrintLabelResponse printLabel(orderNumber)

Print shipping label for an order

### Example

```java
// Import classes:
//import org.openapitools.client.api.PackingApi;

PackingApi apiInstance = new PackingApi();
String orderNumber = null; // String | 
try {
    PrintLabelResponse result = apiInstance.printLabel(orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PackingApi#printLabel");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]

### Return type

[**PrintLabelResponse**](PrintLabelResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## recordPackingVideo

> PackingVideoResponse recordPackingVideo(orderNumber, body)

Record video of packing process

### Example

```java
// Import classes:
//import org.openapitools.client.api.PackingApi;

PackingApi apiInstance = new PackingApi();
String orderNumber = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    PackingVideoResponse result = apiInstance.recordPackingVideo(orderNumber, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PackingApi#recordPackingVideo");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**PackingVideoResponse**](PackingVideoResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

