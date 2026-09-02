# EventSubscriptionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createEventSubscription**](EventSubscriptionApi.md#createEventSubscription) | **POST** /api/v1/event-subscriptions | 
[**deleteEventSubscription**](EventSubscriptionApi.md#deleteEventSubscription) | **DELETE** /api/v1/event-subscriptions/{subscription_id} | 
[**listEventSubscriptions**](EventSubscriptionApi.md#listEventSubscriptions) | **GET** /api/v1/event-subscriptions/ | 



## createEventSubscription

> EventSubscription createEventSubscription(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EventSubscriptionApi;

EventSubscriptionApi apiInstance = new EventSubscriptionApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    EventSubscription result = apiInstance.createEventSubscription(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EventSubscriptionApi#createEventSubscription");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**EventSubscription**](EventSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteEventSubscription

> deleteEventSubscription(subscriptionId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EventSubscriptionApi;

EventSubscriptionApi apiInstance = new EventSubscriptionApi();
String subscriptionId = null; // String | 
try {
    apiInstance.deleteEventSubscription(subscriptionId);
} catch (ApiException e) {
    System.err.println("Exception when calling EventSubscriptionApi#deleteEventSubscription");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscriptionId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listEventSubscriptions

> List&lt;EventSubscription&gt; listEventSubscriptions()



### Example

```java
// Import classes:
//import org.openapitools.client.api.EventSubscriptionApi;

EventSubscriptionApi apiInstance = new EventSubscriptionApi();
try {
    List<EventSubscription> result = apiInstance.listEventSubscriptions();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EventSubscriptionApi#listEventSubscriptions");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;EventSubscription&gt;**](EventSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

