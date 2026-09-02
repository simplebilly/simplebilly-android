# TaxApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTaxRate**](TaxApi.md#createTaxRate) | **POST** /api/v1/tax-rates | Create a tax rate (&#x60;admin:settings&#x60;).
[**deleteTaxRate**](TaxApi.md#deleteTaxRate) | **DELETE** /api/v1/tax-rates/{id} | Delete a tax rate by id (&#x60;admin:settings&#x60;).
[**listTaxRates**](TaxApi.md#listTaxRates) | **GET** /api/v1/tax-rates | List the calling tenant&#39;s tax rates.
[**updateTaxRate**](TaxApi.md#updateTaxRate) | **PUT** /api/v1/tax-rates/{id} | Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.



## createTaxRate

> createTaxRate(taxRateCreate)

Create a tax rate (&#x60;admin:settings&#x60;).

### Example

```java
// Import classes:
//import org.openapitools.client.api.TaxApi;

TaxApi apiInstance = new TaxApi();
TaxRateCreate taxRateCreate = new TaxRateCreate(); // TaxRateCreate | 
try {
    apiInstance.createTaxRate(taxRateCreate);
} catch (ApiException e) {
    System.err.println("Exception when calling TaxApi#createTaxRate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **taxRateCreate** | [**TaxRateCreate**](TaxRateCreate.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## deleteTaxRate

> deleteTaxRate(id)

Delete a tax rate by id (&#x60;admin:settings&#x60;).

### Example

```java
// Import classes:
//import org.openapitools.client.api.TaxApi;

TaxApi apiInstance = new TaxApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteTaxRate(id);
} catch (ApiException e) {
    System.err.println("Exception when calling TaxApi#deleteTaxRate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## listTaxRates

> listTaxRates()

List the calling tenant&#39;s tax rates.

### Example

```java
// Import classes:
//import org.openapitools.client.api.TaxApi;

TaxApi apiInstance = new TaxApi();
try {
    apiInstance.listTaxRates();
} catch (ApiException e) {
    System.err.println("Exception when calling TaxApi#listTaxRates");
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


## updateTaxRate

> updateTaxRate(id, taxRateCreate)

Update a tax rate by id (&#x60;admin:settings&#x60;). Replaces all body fields.

### Example

```java
// Import classes:
//import org.openapitools.client.api.TaxApi;

TaxApi apiInstance = new TaxApi();
UUID id = null; // UUID | 
TaxRateCreate taxRateCreate = new TaxRateCreate(); // TaxRateCreate | 
try {
    apiInstance.updateTaxRate(id, taxRateCreate);
} catch (ApiException e) {
    System.err.println("Exception when calling TaxApi#updateTaxRate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **taxRateCreate** | [**TaxRateCreate**](TaxRateCreate.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

