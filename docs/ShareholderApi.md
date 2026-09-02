# ShareholderApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShareholder**](ShareholderApi.md#createShareholder) | **POST** /api/v1/shareholders | 
[**deleteShareholder**](ShareholderApi.md#deleteShareholder) | **DELETE** /api/v1/shareholders/{id} | 
[**getShareholder**](ShareholderApi.md#getShareholder) | **GET** /api/v1/shareholders/{id} | 
[**getShareholders**](ShareholderApi.md#getShareholders) | **GET** /api/v1/shareholders/ | 
[**updateShareholder**](ShareholderApi.md#updateShareholder) | **PUT** /api/v1/shareholders/{id} | 



## createShareholder

> Shareholder createShareholder(shareholderCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShareholderApi;

ShareholderApi apiInstance = new ShareholderApi();
ShareholderCreate shareholderCreate = new ShareholderCreate(); // ShareholderCreate | 
try {
    Shareholder result = apiInstance.createShareholder(shareholderCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShareholderApi#createShareholder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shareholderCreate** | [**ShareholderCreate**](ShareholderCreate.md)|  |

### Return type

[**Shareholder**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShareholder

> deleteShareholder(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShareholderApi;

ShareholderApi apiInstance = new ShareholderApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteShareholder(id);
} catch (ApiException e) {
    System.err.println("Exception when calling ShareholderApi#deleteShareholder");
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


## getShareholder

> Shareholder getShareholder(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShareholderApi;

ShareholderApi apiInstance = new ShareholderApi();
UUID id = null; // UUID | 
try {
    Shareholder result = apiInstance.getShareholder(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShareholderApi#getShareholder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Shareholder**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShareholders

> List&lt;Shareholder&gt; getShareholders(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShareholderApi;

ShareholderApi apiInstance = new ShareholderApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Shareholder> result = apiInstance.getShareholders(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShareholderApi#getShareholders");
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

[**List&lt;Shareholder&gt;**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShareholder

> Shareholder updateShareholder(id, shareholderUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShareholderApi;

ShareholderApi apiInstance = new ShareholderApi();
UUID id = null; // UUID | 
ShareholderUpdate shareholderUpdate = new ShareholderUpdate(); // ShareholderUpdate | 
try {
    Shareholder result = apiInstance.updateShareholder(id, shareholderUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShareholderApi#updateShareholder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **shareholderUpdate** | [**ShareholderUpdate**](ShareholderUpdate.md)|  |

### Return type

[**Shareholder**](Shareholder.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

