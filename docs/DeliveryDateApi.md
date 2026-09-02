# DeliveryDateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeliveryDate**](DeliveryDateApi.md#createDeliveryDate) | **POST** /api/v1/delivery-dates | 
[**deleteDeliveryDate**](DeliveryDateApi.md#deleteDeliveryDate) | **DELETE** /api/v1/delivery-dates/{delivery_date_id} | 
[**getDeliveryDate**](DeliveryDateApi.md#getDeliveryDate) | **GET** /api/v1/delivery-dates/{delivery_date_id} | 
[**getDeliveryPerformance**](DeliveryDateApi.md#getDeliveryPerformance) | **GET** /api/v1/delivery-dates/performance | On-time performance summary: how many promised delivery dates were met within a period.
[**listDeliveryDates**](DeliveryDateApi.md#listDeliveryDates) | **GET** /api/v1/delivery-dates/ | 
[**updateDeliveryDate**](DeliveryDateApi.md#updateDeliveryDate) | **PUT** /api/v1/delivery-dates/{delivery_date_id} | 
[**updateDeliveryDateStatus**](DeliveryDateApi.md#updateDeliveryDateStatus) | **PUT** /api/v1/delivery-dates/{delivery_date_id}/status | 



## createDeliveryDate

> DeliveryDate createDeliveryDate(deliveryDateCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
DeliveryDateCreate deliveryDateCreate = new DeliveryDateCreate(); // DeliveryDateCreate | 
try {
    DeliveryDate result = apiInstance.createDeliveryDate(deliveryDateCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#createDeliveryDate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryDateCreate** | [**DeliveryDateCreate**](DeliveryDateCreate.md)|  |

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteDeliveryDate

> deleteDeliveryDate(deliveryDateId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
String deliveryDateId = null; // String | 
try {
    apiInstance.deleteDeliveryDate(deliveryDateId);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#deleteDeliveryDate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryDateId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliveryDate

> DeliveryDate getDeliveryDate(deliveryDateId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
String deliveryDateId = null; // String | 
try {
    DeliveryDate result = apiInstance.getDeliveryDate(deliveryDateId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#getDeliveryDate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryDateId** | **String**|  | [default to null]

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliveryPerformance

> OasAnyTypeNotMapped getDeliveryPerformance(page, pageSize, orderNumber, status, from, to)

On-time performance summary: how many promised delivery dates were met within a period.

### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String orderNumber = null; // String | 
String status = null; // String | 
Date from = null; // Date | Only dates on or after this date.
Date to = null; // Date | Only dates on or before this date.
try {
    OasAnyTypeNotMapped result = apiInstance.getDeliveryPerformance(page, pageSize, orderNumber, status, from, to);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#getDeliveryPerformance");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **orderNumber** | **String**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **from** | **Date**| Only dates on or after this date. | [optional] [default to null]
 **to** | **Date**| Only dates on or before this date. | [optional] [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDeliveryDates

> List&lt;DeliveryDate&gt; listDeliveryDates(page, pageSize, orderNumber, status, from, to)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String orderNumber = null; // String | 
String status = null; // String | 
Date from = null; // Date | Only dates on or after this date.
Date to = null; // Date | Only dates on or before this date.
try {
    List<DeliveryDate> result = apiInstance.listDeliveryDates(page, pageSize, orderNumber, status, from, to);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#listDeliveryDates");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **orderNumber** | **String**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **from** | **Date**| Only dates on or after this date. | [optional] [default to null]
 **to** | **Date**| Only dates on or before this date. | [optional] [default to null]

### Return type

[**List&lt;DeliveryDate&gt;**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateDeliveryDate

> DeliveryDate updateDeliveryDate(deliveryDateId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
String deliveryDateId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    DeliveryDate result = apiInstance.updateDeliveryDate(deliveryDateId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#updateDeliveryDate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryDateId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateDeliveryDateStatus

> DeliveryDate updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryDateApi;

DeliveryDateApi apiInstance = new DeliveryDateApi();
String deliveryDateId = null; // String | 
DeliveryDateStatusUpdate deliveryDateStatusUpdate = new DeliveryDateStatusUpdate(); // DeliveryDateStatusUpdate | 
try {
    DeliveryDate result = apiInstance.updateDeliveryDateStatus(deliveryDateId, deliveryDateStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryDateApi#updateDeliveryDateStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryDateId** | **String**|  | [default to null]
 **deliveryDateStatusUpdate** | [**DeliveryDateStatusUpdate**](DeliveryDateStatusUpdate.md)|  |

### Return type

[**DeliveryDate**](DeliveryDate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

