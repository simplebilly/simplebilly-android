# PriceTierApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPriceTier**](PriceTierApi.md#createPriceTier) | **POST** /api/v1/price-tiers | 
[**deletePriceTier**](PriceTierApi.md#deletePriceTier) | **DELETE** /api/v1/price-tiers/{price_tier_id} | 
[**getPriceTier**](PriceTierApi.md#getPriceTier) | **GET** /api/v1/price-tiers/{price_tier_id} | 
[**getResolvedPrice**](PriceTierApi.md#getResolvedPrice) | **GET** /api/v1/price-tiers/resolved | 
[**listPriceTiers**](PriceTierApi.md#listPriceTiers) | **GET** /api/v1/price-tiers/ | 
[**updatePriceTier**](PriceTierApi.md#updatePriceTier) | **PUT** /api/v1/price-tiers/{price_tier_id} | 



## createPriceTier

> PriceTier createPriceTier(priceTierCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PriceTierApi;

PriceTierApi apiInstance = new PriceTierApi();
PriceTierCreate priceTierCreate = new PriceTierCreate(); // PriceTierCreate | 
try {
    PriceTier result = apiInstance.createPriceTier(priceTierCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PriceTierApi#createPriceTier");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **priceTierCreate** | [**PriceTierCreate**](PriceTierCreate.md)|  |

### Return type

[**PriceTier**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePriceTier

> deletePriceTier(priceTierId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PriceTierApi;

PriceTierApi apiInstance = new PriceTierApi();
String priceTierId = null; // String | 
try {
    apiInstance.deletePriceTier(priceTierId);
} catch (ApiException e) {
    System.err.println("Exception when calling PriceTierApi#deletePriceTier");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **priceTierId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPriceTier

> PriceTier getPriceTier(priceTierId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PriceTierApi;

PriceTierApi apiInstance = new PriceTierApi();
String priceTierId = null; // String | 
try {
    PriceTier result = apiInstance.getPriceTier(priceTierId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PriceTierApi#getPriceTier");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **priceTierId** | **String**|  | [default to null]

### Return type

[**PriceTier**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getResolvedPrice

> ResolvedPriceResponse getResolvedPrice(productId, quantity, contactId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PriceTierApi;

PriceTierApi apiInstance = new PriceTierApi();
UUID productId = null; // UUID | 
Long quantity = null; // Long | 
String contactId = null; // String | Contact used to match customer-group-scoped tiers.
try {
    ResolvedPriceResponse result = apiInstance.getResolvedPrice(productId, quantity, contactId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PriceTierApi#getResolvedPrice");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]
 **quantity** | **Long**|  | [optional] [default to null]
 **contactId** | **String**| Contact used to match customer-group-scoped tiers. | [optional] [default to null]

### Return type

[**ResolvedPriceResponse**](ResolvedPriceResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPriceTiers

> List&lt;PriceTier&gt; listPriceTiers(page, pageSize, productId, customerGroupId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PriceTierApi;

PriceTierApi apiInstance = new PriceTierApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
UUID productId = null; // UUID | 
String customerGroupId = null; // String | 
try {
    List<PriceTier> result = apiInstance.listPriceTiers(page, pageSize, productId, customerGroupId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PriceTierApi#listPriceTiers");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **productId** | **UUID**|  | [optional] [default to null]
 **customerGroupId** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;PriceTier&gt;**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updatePriceTier

> PriceTier updatePriceTier(priceTierId, priceTierUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PriceTierApi;

PriceTierApi apiInstance = new PriceTierApi();
String priceTierId = null; // String | 
PriceTierUpdate priceTierUpdate = new PriceTierUpdate(); // PriceTierUpdate | 
try {
    PriceTier result = apiInstance.updatePriceTier(priceTierId, priceTierUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PriceTierApi#updatePriceTier");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **priceTierId** | **String**|  | [default to null]
 **priceTierUpdate** | [**PriceTierUpdate**](PriceTierUpdate.md)|  |

### Return type

[**PriceTier**](PriceTier.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

