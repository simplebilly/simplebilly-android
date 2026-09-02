# BillingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getPlans**](BillingApi.md#getPlans) | **GET** /api/v1/plans | All canonical plans (free/starter/business/enterprise) — the single source of truth lives in &#x60;crate::saasy::plans&#x60;, matching marketing.
[**getQuotaApi**](BillingApi.md#getQuotaApi) | **GET** /api/v1/quota | Effective limits + current usage for the calling tenant.
[**getSubscriptionApi**](BillingApi.md#getSubscriptionApi) | **GET** /api/v1/subscription | 
[**getUsageApi**](BillingApi.md#getUsageApi) | **GET** /api/v1/usage | 
[**paddleSubscriptionWebhook**](BillingApi.md#paddleSubscriptionWebhook) | **POST** /api/webhooks/paddle/subscription | Paddle Billing subscription webhook. Verifies the &#x60;Paddle-Signature&#x60; header (HMAC-SHA256 over &#x60;\&quot;{ts}:{raw_body}\&quot;&#x60; with the webhook secret), then updates &#x60;billing_info&#x60; and &#x60;tenants.plan&#x60; for the tenant identified by the subscription &#x60;custom_data&#x60; (JSON &#x60;{\&quot;tenant_id\&quot;: \&quot;...\&quot;}&#x60; or a bare tenant UUID).
[**putQuotaApi**](BillingApi.md#putQuotaApi) | **PUT** /api/v1/quota | Write the per-tenant quota override (&#x60;admin:settings&#x60;). An empty object clears the override.



## getPlans

> ApiResponseVecPlan getPlans()

All canonical plans (free/starter/business/enterprise) — the single source of truth lives in &#x60;crate::saasy::plans&#x60;, matching marketing.

### Example

```java
// Import classes:
//import org.openapitools.client.api.BillingApi;

BillingApi apiInstance = new BillingApi();
try {
    ApiResponseVecPlan result = apiInstance.getPlans();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BillingApi#getPlans");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseVecPlan**](ApiResponseVecPlan.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getQuotaApi

> getQuotaApi()

Effective limits + current usage for the calling tenant.

### Example

```java
// Import classes:
//import org.openapitools.client.api.BillingApi;

BillingApi apiInstance = new BillingApi();
try {
    apiInstance.getQuotaApi();
} catch (ApiException e) {
    System.err.println("Exception when calling BillingApi#getQuotaApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getSubscriptionApi

> ApiResponseSubscriptionOverview getSubscriptionApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.BillingApi;

BillingApi apiInstance = new BillingApi();
try {
    ApiResponseSubscriptionOverview result = apiInstance.getSubscriptionApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BillingApi#getSubscriptionApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseSubscriptionOverview**](ApiResponseSubscriptionOverview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getUsageApi

> getUsageApi(meter)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BillingApi;

BillingApi apiInstance = new BillingApi();
String meter = null; // String | 
try {
    apiInstance.getUsageApi(meter);
} catch (ApiException e) {
    System.err.println("Exception when calling BillingApi#getUsageApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **meter** | **String**|  | [optional] [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## paddleSubscriptionWebhook

> paddleSubscriptionWebhook()

Paddle Billing subscription webhook. Verifies the &#x60;Paddle-Signature&#x60; header (HMAC-SHA256 over &#x60;\&quot;{ts}:{raw_body}\&quot;&#x60; with the webhook secret), then updates &#x60;billing_info&#x60; and &#x60;tenants.plan&#x60; for the tenant identified by the subscription &#x60;custom_data&#x60; (JSON &#x60;{\&quot;tenant_id\&quot;: \&quot;...\&quot;}&#x60; or a bare tenant UUID).

### Example

```java
// Import classes:
//import org.openapitools.client.api.BillingApi;

BillingApi apiInstance = new BillingApi();
try {
    apiInstance.paddleSubscriptionWebhook();
} catch (ApiException e) {
    System.err.println("Exception when calling BillingApi#paddleSubscriptionWebhook");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## putQuotaApi

> putQuotaApi(quotaOverride)

Write the per-tenant quota override (&#x60;admin:settings&#x60;). An empty object clears the override.

### Example

```java
// Import classes:
//import org.openapitools.client.api.BillingApi;

BillingApi apiInstance = new BillingApi();
QuotaOverride quotaOverride = new QuotaOverride(); // QuotaOverride | 
try {
    apiInstance.putQuotaApi(quotaOverride);
} catch (ApiException e) {
    System.err.println("Exception when calling BillingApi#putQuotaApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **quotaOverride** | [**QuotaOverride**](QuotaOverride.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

