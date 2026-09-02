# SilentPartnerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSilentPartner**](SilentPartnerApi.md#createSilentPartner) | **POST** /api/v1/silent-partners | 
[**deleteSilentPartner**](SilentPartnerApi.md#deleteSilentPartner) | **DELETE** /api/v1/silent-partners/{id} | 
[**getSilentPartner**](SilentPartnerApi.md#getSilentPartner) | **GET** /api/v1/silent-partners/{id} | 
[**getSilentPartners**](SilentPartnerApi.md#getSilentPartners) | **GET** /api/v1/silent-partners/ | 
[**updateSilentPartner**](SilentPartnerApi.md#updateSilentPartner) | **PUT** /api/v1/silent-partners/{id} | 



## createSilentPartner

> SilentPartner createSilentPartner(silentPartnerCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SilentPartnerApi;

SilentPartnerApi apiInstance = new SilentPartnerApi();
SilentPartnerCreate silentPartnerCreate = new SilentPartnerCreate(); // SilentPartnerCreate | 
try {
    SilentPartner result = apiInstance.createSilentPartner(silentPartnerCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SilentPartnerApi#createSilentPartner");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **silentPartnerCreate** | [**SilentPartnerCreate**](SilentPartnerCreate.md)|  |

### Return type

[**SilentPartner**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteSilentPartner

> deleteSilentPartner(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SilentPartnerApi;

SilentPartnerApi apiInstance = new SilentPartnerApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteSilentPartner(id);
} catch (ApiException e) {
    System.err.println("Exception when calling SilentPartnerApi#deleteSilentPartner");
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
- **Accept**: application/json


## getSilentPartner

> SilentPartner getSilentPartner(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SilentPartnerApi;

SilentPartnerApi apiInstance = new SilentPartnerApi();
UUID id = null; // UUID | 
try {
    SilentPartner result = apiInstance.getSilentPartner(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SilentPartnerApi#getSilentPartner");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**SilentPartner**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getSilentPartners

> List&lt;SilentPartner&gt; getSilentPartners(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SilentPartnerApi;

SilentPartnerApi apiInstance = new SilentPartnerApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<SilentPartner> result = apiInstance.getSilentPartners(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SilentPartnerApi#getSilentPartners");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **includeDeleted** | **Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] [default to null]

### Return type

[**List&lt;SilentPartner&gt;**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateSilentPartner

> SilentPartner updateSilentPartner(id, silentPartnerUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SilentPartnerApi;

SilentPartnerApi apiInstance = new SilentPartnerApi();
UUID id = null; // UUID | 
SilentPartnerUpdate silentPartnerUpdate = new SilentPartnerUpdate(); // SilentPartnerUpdate | 
try {
    SilentPartner result = apiInstance.updateSilentPartner(id, silentPartnerUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SilentPartnerApi#updateSilentPartner");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **silentPartnerUpdate** | [**SilentPartnerUpdate**](SilentPartnerUpdate.md)|  |

### Return type

[**SilentPartner**](SilentPartner.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

