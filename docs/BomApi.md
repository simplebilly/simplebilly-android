# BomApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createBom**](BomApi.md#createBom) | **POST** /api/v1/boms | 
[**deleteBom**](BomApi.md#deleteBom) | **DELETE** /api/v1/boms/{bom_id} | 
[**getBom**](BomApi.md#getBom) | **GET** /api/v1/boms/{bom_id} | 
[**listBoms**](BomApi.md#listBoms) | **GET** /api/v1/boms/ | 
[**updateBom**](BomApi.md#updateBom) | **PUT** /api/v1/boms/{bom_id} | 



## createBom

> Bom createBom(bomCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BomApi;

BomApi apiInstance = new BomApi();
BomCreate bomCreate = new BomCreate(); // BomCreate | 
try {
    Bom result = apiInstance.createBom(bomCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BomApi#createBom");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bomCreate** | [**BomCreate**](BomCreate.md)|  |

### Return type

[**Bom**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteBom

> deleteBom(bomId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BomApi;

BomApi apiInstance = new BomApi();
UUID bomId = null; // UUID | 
try {
    apiInstance.deleteBom(bomId);
} catch (ApiException e) {
    System.err.println("Exception when calling BomApi#deleteBom");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bomId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getBom

> Bom getBom(bomId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BomApi;

BomApi apiInstance = new BomApi();
UUID bomId = null; // UUID | 
try {
    Bom result = apiInstance.getBom(bomId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BomApi#getBom");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bomId** | **UUID**|  | [default to null]

### Return type

[**Bom**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listBoms

> List&lt;Bom&gt; listBoms(page, pageSize, search, productId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BomApi;

BomApi apiInstance = new BomApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
UUID productId = null; // UUID | Filter by finished product id.
try {
    List<Bom> result = apiInstance.listBoms(page, pageSize, search, productId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BomApi#listBoms");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **productId** | **UUID**| Filter by finished product id. | [optional] [default to null]

### Return type

[**List&lt;Bom&gt;**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateBom

> Bom updateBom(bomId, bomUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BomApi;

BomApi apiInstance = new BomApi();
UUID bomId = null; // UUID | 
BomUpdate bomUpdate = new BomUpdate(); // BomUpdate | 
try {
    Bom result = apiInstance.updateBom(bomId, bomUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BomApi#updateBom");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **bomId** | **UUID**|  | [default to null]
 **bomUpdate** | [**BomUpdate**](BomUpdate.md)|  |

### Return type

[**Bom**](Bom.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

