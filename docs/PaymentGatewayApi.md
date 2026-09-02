# PaymentGatewayApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPaymentGatewayApi**](PaymentGatewayApi.md#createPaymentGatewayApi) | **POST** /api/v1/payment-gateways | 
[**deletePaymentGatewayApi**](PaymentGatewayApi.md#deletePaymentGatewayApi) | **DELETE** /api/v1/payment-gateways/{gateway_id} | 
[**listPaymentGatewaysApi**](PaymentGatewayApi.md#listPaymentGatewaysApi) | **GET** /api/v1/payment-gateways/ | 
[**oauthAuthorizeApi**](PaymentGatewayApi.md#oauthAuthorizeApi) | **POST** /api/v1/payment-gateways/oauth/authorize | 
[**oauthCallbackApi**](PaymentGatewayApi.md#oauthCallbackApi) | **POST** /api/v1/payment-gateways/oauth/callback | 
[**updatePaymentGatewayApi**](PaymentGatewayApi.md#updatePaymentGatewayApi) | **PUT** /api/v1/payment-gateways/{gateway_id} | 



## createPaymentGatewayApi

> PaymentGateway createPaymentGatewayApi(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentGatewayApi;

PaymentGatewayApi apiInstance = new PaymentGatewayApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    PaymentGateway result = apiInstance.createPaymentGatewayApi(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentGatewayApi#createPaymentGatewayApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePaymentGatewayApi

> deletePaymentGatewayApi(gatewayId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentGatewayApi;

PaymentGatewayApi apiInstance = new PaymentGatewayApi();
String gatewayId = null; // String | 
try {
    apiInstance.deletePaymentGatewayApi(gatewayId);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentGatewayApi#deletePaymentGatewayApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gatewayId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPaymentGatewaysApi

> List&lt;PaymentGateway&gt; listPaymentGatewaysApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentGatewayApi;

PaymentGatewayApi apiInstance = new PaymentGatewayApi();
try {
    List<PaymentGateway> result = apiInstance.listPaymentGatewaysApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentGatewayApi#listPaymentGatewaysApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PaymentGateway&gt;**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## oauthAuthorizeApi

> GatewayOAuthAuthorizeResponse oauthAuthorizeApi(gatewayOAuthAuthorizeRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentGatewayApi;

PaymentGatewayApi apiInstance = new PaymentGatewayApi();
GatewayOAuthAuthorizeRequest gatewayOAuthAuthorizeRequest = new GatewayOAuthAuthorizeRequest(); // GatewayOAuthAuthorizeRequest | 
try {
    GatewayOAuthAuthorizeResponse result = apiInstance.oauthAuthorizeApi(gatewayOAuthAuthorizeRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentGatewayApi#oauthAuthorizeApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gatewayOAuthAuthorizeRequest** | [**GatewayOAuthAuthorizeRequest**](GatewayOAuthAuthorizeRequest.md)|  |

### Return type

[**GatewayOAuthAuthorizeResponse**](GatewayOAuthAuthorizeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## oauthCallbackApi

> PaymentGateway oauthCallbackApi(gatewayOAuthCallbackRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentGatewayApi;

PaymentGatewayApi apiInstance = new PaymentGatewayApi();
GatewayOAuthCallbackRequest gatewayOAuthCallbackRequest = new GatewayOAuthCallbackRequest(); // GatewayOAuthCallbackRequest | 
try {
    PaymentGateway result = apiInstance.oauthCallbackApi(gatewayOAuthCallbackRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentGatewayApi#oauthCallbackApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gatewayOAuthCallbackRequest** | [**GatewayOAuthCallbackRequest**](GatewayOAuthCallbackRequest.md)|  |

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updatePaymentGatewayApi

> PaymentGateway updatePaymentGatewayApi(gatewayId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentGatewayApi;

PaymentGatewayApi apiInstance = new PaymentGatewayApi();
String gatewayId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    PaymentGateway result = apiInstance.updatePaymentGatewayApi(gatewayId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentGatewayApi#updatePaymentGatewayApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gatewayId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**PaymentGateway**](PaymentGateway.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

