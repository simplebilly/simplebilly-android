# ShippingThresholdApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShippingThreshold**](ShippingThresholdApi.md#createShippingThreshold) | **POST** /api/v1/shipping-thresholds | 
[**deleteShippingThreshold**](ShippingThresholdApi.md#deleteShippingThreshold) | **DELETE** /api/v1/shipping-thresholds/{threshold_id} | 
[**getDeliverable**](ShippingThresholdApi.md#getDeliverable) | **GET** /api/v1/shipping-thresholds/deliverable | 
[**getShippingThreshold**](ShippingThresholdApi.md#getShippingThreshold) | **GET** /api/v1/shipping-thresholds/{threshold_id} | 
[**listShippingThresholds**](ShippingThresholdApi.md#listShippingThresholds) | **GET** /api/v1/shipping-thresholds/ | 
[**updateShippingThreshold**](ShippingThresholdApi.md#updateShippingThreshold) | **PUT** /api/v1/shipping-thresholds/{threshold_id} | 



## createShippingThreshold

> ShippingThreshold createShippingThreshold(shippingThresholdCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingThresholdApi;

ShippingThresholdApi apiInstance = new ShippingThresholdApi();
ShippingThresholdCreate shippingThresholdCreate = new ShippingThresholdCreate(); // ShippingThresholdCreate | 
try {
    ShippingThreshold result = apiInstance.createShippingThreshold(shippingThresholdCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingThresholdApi#createShippingThreshold");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shippingThresholdCreate** | [**ShippingThresholdCreate**](ShippingThresholdCreate.md)|  |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShippingThreshold

> deleteShippingThreshold(thresholdId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingThresholdApi;

ShippingThresholdApi apiInstance = new ShippingThresholdApi();
String thresholdId = null; // String | 
try {
    apiInstance.deleteShippingThreshold(thresholdId);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingThresholdApi#deleteShippingThreshold");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **thresholdId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliverable

> DeliverableResponse getDeliverable(productId, warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingThresholdApi;

ShippingThresholdApi apiInstance = new ShippingThresholdApi();
UUID productId = null; // UUID | 
String warehouseId = null; // String | 
try {
    DeliverableResponse result = apiInstance.getDeliverable(productId, warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingThresholdApi#getDeliverable");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]
 **warehouseId** | **String**|  | [optional] [default to null]

### Return type

[**DeliverableResponse**](DeliverableResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShippingThreshold

> ShippingThreshold getShippingThreshold(thresholdId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingThresholdApi;

ShippingThresholdApi apiInstance = new ShippingThresholdApi();
String thresholdId = null; // String | 
try {
    ShippingThreshold result = apiInstance.getShippingThreshold(thresholdId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingThresholdApi#getShippingThreshold");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **thresholdId** | **String**|  | [default to null]

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listShippingThresholds

> List&lt;ShippingThreshold&gt; listShippingThresholds(page, pageSize, productId, warehouseId, isActive)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingThresholdApi;

ShippingThresholdApi apiInstance = new ShippingThresholdApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
UUID productId = null; // UUID | 
String warehouseId = null; // String | 
Boolean isActive = null; // Boolean | 
try {
    List<ShippingThreshold> result = apiInstance.listShippingThresholds(page, pageSize, productId, warehouseId, isActive);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingThresholdApi#listShippingThresholds");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **productId** | **UUID**|  | [optional] [default to null]
 **warehouseId** | **String**|  | [optional] [default to null]
 **isActive** | **Boolean**|  | [optional] [default to null]

### Return type

[**List&lt;ShippingThreshold&gt;**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShippingThreshold

> ShippingThreshold updateShippingThreshold(thresholdId, shippingThresholdUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingThresholdApi;

ShippingThresholdApi apiInstance = new ShippingThresholdApi();
String thresholdId = null; // String | 
ShippingThresholdUpdate shippingThresholdUpdate = new ShippingThresholdUpdate(); // ShippingThresholdUpdate | 
try {
    ShippingThreshold result = apiInstance.updateShippingThreshold(thresholdId, shippingThresholdUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingThresholdApi#updateShippingThreshold");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **thresholdId** | **String**|  | [default to null]
 **shippingThresholdUpdate** | [**ShippingThresholdUpdate**](ShippingThresholdUpdate.md)|  |

### Return type

[**ShippingThreshold**](ShippingThreshold.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

