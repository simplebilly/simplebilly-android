# WebhooksApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSubscription**](WebhooksApi.md#createSubscription) | **POST** /api/v1/webhook-subscriptions | Create a webhook subscription (outbound hook).
[**deleteSubscription**](WebhooksApi.md#deleteSubscription) | **DELETE** /api/v1/webhook-subscriptions/{subscription_id} | Delete a webhook subscription.
[**emitApi**](WebhooksApi.md#emitApi) | **POST** /api/v1/webhooks/emit | Manually fire an event against matching hooks (for testing/flows).
[**listEvent**](WebhooksApi.md#listEvent) | **GET** /api/v1/webhook-events | List webhook events (inbound + outbound log).
[**listSubscriptions**](WebhooksApi.md#listSubscriptions) | **GET** /api/v1/webhook-subscriptions | List webhook subscriptions for the tenant.
[**updateSubscription**](WebhooksApi.md#updateSubscription) | **PUT** /api/v1/webhook-subscriptions/{subscription_id} | Update a webhook subscription.



## createSubscription

> WebhookSubscription createSubscription(createSubscriptionRequest)

Create a webhook subscription (outbound hook).

### Example

```java
// Import classes:
//import org.openapitools.client.api.WebhooksApi;

WebhooksApi apiInstance = new WebhooksApi();
CreateSubscriptionRequest createSubscriptionRequest = new CreateSubscriptionRequest(); // CreateSubscriptionRequest | 
try {
    WebhookSubscription result = apiInstance.createSubscription(createSubscriptionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WebhooksApi#createSubscription");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createSubscriptionRequest** | [**CreateSubscriptionRequest**](CreateSubscriptionRequest.md)|  |

### Return type

[**WebhookSubscription**](WebhookSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSubscription

> deleteSubscription(subscriptionId)

Delete a webhook subscription.

### Example

```java
// Import classes:
//import org.openapitools.client.api.WebhooksApi;

WebhooksApi apiInstance = new WebhooksApi();
String subscriptionId = null; // String | 
try {
    apiInstance.deleteSubscription(subscriptionId);
} catch (ApiException e) {
    System.err.println("Exception when calling WebhooksApi#deleteSubscription");
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
- **Accept**: Not defined


## emitApi

> emitApi(emitEventRequest)

Manually fire an event against matching hooks (for testing/flows).

### Example

```java
// Import classes:
//import org.openapitools.client.api.WebhooksApi;

WebhooksApi apiInstance = new WebhooksApi();
EmitEventRequest emitEventRequest = new EmitEventRequest(); // EmitEventRequest | 
try {
    apiInstance.emitApi(emitEventRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling WebhooksApi#emitApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emitEventRequest** | [**EmitEventRequest**](EmitEventRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## listEvent

> List&lt;WebhookEvent&gt; listEvent()

List webhook events (inbound + outbound log).

### Example

```java
// Import classes:
//import org.openapitools.client.api.WebhooksApi;

WebhooksApi apiInstance = new WebhooksApi();
try {
    List<WebhookEvent> result = apiInstance.listEvent();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WebhooksApi#listEvent");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;WebhookEvent&gt;**](WebhookEvent.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listSubscriptions

> List&lt;WebhookSubscription&gt; listSubscriptions()

List webhook subscriptions for the tenant.

### Example

```java
// Import classes:
//import org.openapitools.client.api.WebhooksApi;

WebhooksApi apiInstance = new WebhooksApi();
try {
    List<WebhookSubscription> result = apiInstance.listSubscriptions();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WebhooksApi#listSubscriptions");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;WebhookSubscription&gt;**](WebhookSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSubscription

> WebhookSubscription updateSubscription(subscriptionId, updateSubscriptionRequest)

Update a webhook subscription.

### Example

```java
// Import classes:
//import org.openapitools.client.api.WebhooksApi;

WebhooksApi apiInstance = new WebhooksApi();
String subscriptionId = null; // String | 
UpdateSubscriptionRequest updateSubscriptionRequest = new UpdateSubscriptionRequest(); // UpdateSubscriptionRequest | 
try {
    WebhookSubscription result = apiInstance.updateSubscription(subscriptionId, updateSubscriptionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WebhooksApi#updateSubscription");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **subscriptionId** | **String**|  | [default to null]
 **updateSubscriptionRequest** | [**UpdateSubscriptionRequest**](UpdateSubscriptionRequest.md)|  |

### Return type

[**WebhookSubscription**](WebhookSubscription.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

