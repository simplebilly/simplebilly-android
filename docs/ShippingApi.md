# ShippingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getCredentialsApi**](ShippingApi.md#getCredentialsApi) | **GET** /api/v1/shipping/credentials | 
[**getRatesApi**](ShippingApi.md#getRatesApi) | **POST** /api/v1/shipping/rates | 
[**listProvidersApi**](ShippingApi.md#listProvidersApi) | **GET** /api/v1/shipping/providers | 
[**saveCredentialsApi**](ShippingApi.md#saveCredentialsApi) | **PUT** /api/v1/shipping/credentials | 



## getCredentialsApi

> ShippingCredentials getCredentialsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingApi;

ShippingApi apiInstance = new ShippingApi();
try {
    ShippingCredentials result = apiInstance.getCredentialsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingApi#getCredentialsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ShippingCredentials**](ShippingCredentials.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getRatesApi

> RateResponse getRatesApi(rateRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingApi;

ShippingApi apiInstance = new ShippingApi();
RateRequest rateRequest = new RateRequest(); // RateRequest | 
try {
    RateResponse result = apiInstance.getRatesApi(rateRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingApi#getRatesApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rateRequest** | [**RateRequest**](RateRequest.md)|  |

### Return type

[**RateResponse**](RateResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listProvidersApi

> List&lt;ProviderInfo&gt; listProvidersApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingApi;

ShippingApi apiInstance = new ShippingApi();
try {
    List<ProviderInfo> result = apiInstance.listProvidersApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingApi#listProvidersApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;ProviderInfo&gt;**](ProviderInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## saveCredentialsApi

> ShippingCredentials saveCredentialsApi(shippingCredentials)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingApi;

ShippingApi apiInstance = new ShippingApi();
ShippingCredentials shippingCredentials = new ShippingCredentials(); // ShippingCredentials | 
try {
    ShippingCredentials result = apiInstance.saveCredentialsApi(shippingCredentials);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingApi#saveCredentialsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shippingCredentials** | [**ShippingCredentials**](ShippingCredentials.md)|  |

### Return type

[**ShippingCredentials**](ShippingCredentials.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

