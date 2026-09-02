# ProductAttributeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductAttribute**](ProductAttributeApi.md#createProductAttribute) | **POST** /api/v1/product-attributes | 
[**deleteProductAttribute**](ProductAttributeApi.md#deleteProductAttribute) | **DELETE** /api/v1/product-attributes/{attribute_id} | 
[**getProductAttribute**](ProductAttributeApi.md#getProductAttribute) | **GET** /api/v1/product-attributes/{attribute_id} | 
[**listProductAttributes**](ProductAttributeApi.md#listProductAttributes) | **GET** /api/v1/product-attributes/ | 
[**updateProductAttribute**](ProductAttributeApi.md#updateProductAttribute) | **PUT** /api/v1/product-attributes/{attribute_id} | 



## createProductAttribute

> ProductAttribute createProductAttribute(productAttributeCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductAttributeApi;

ProductAttributeApi apiInstance = new ProductAttributeApi();
ProductAttributeCreate productAttributeCreate = new ProductAttributeCreate(); // ProductAttributeCreate | 
try {
    ProductAttribute result = apiInstance.createProductAttribute(productAttributeCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductAttributeApi#createProductAttribute");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productAttributeCreate** | [**ProductAttributeCreate**](ProductAttributeCreate.md)|  |

### Return type

[**ProductAttribute**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductAttribute

> deleteProductAttribute(attributeId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductAttributeApi;

ProductAttributeApi apiInstance = new ProductAttributeApi();
String attributeId = null; // String | 
try {
    apiInstance.deleteProductAttribute(attributeId);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductAttributeApi#deleteProductAttribute");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attributeId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductAttribute

> ProductAttribute getProductAttribute(attributeId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductAttributeApi;

ProductAttributeApi apiInstance = new ProductAttributeApi();
String attributeId = null; // String | 
try {
    ProductAttribute result = apiInstance.getProductAttribute(attributeId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductAttributeApi#getProductAttribute");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attributeId** | **String**|  | [default to null]

### Return type

[**ProductAttribute**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductAttributes

> List&lt;ProductAttribute&gt; listProductAttributes(page, pageSize, productId, isFilterable, search)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductAttributeApi;

ProductAttributeApi apiInstance = new ProductAttributeApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
UUID productId = null; // UUID | 
Boolean isFilterable = null; // Boolean | 
String search = null; // String | 
try {
    List<ProductAttribute> result = apiInstance.listProductAttributes(page, pageSize, productId, isFilterable, search);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductAttributeApi#listProductAttributes");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **productId** | **UUID**|  | [optional] [default to null]
 **isFilterable** | **Boolean**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;ProductAttribute&gt;**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductAttribute

> ProductAttribute updateProductAttribute(attributeId, productAttributeUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductAttributeApi;

ProductAttributeApi apiInstance = new ProductAttributeApi();
String attributeId = null; // String | 
ProductAttributeUpdate productAttributeUpdate = new ProductAttributeUpdate(); // ProductAttributeUpdate | 
try {
    ProductAttribute result = apiInstance.updateProductAttribute(attributeId, productAttributeUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductAttributeApi#updateProductAttribute");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attributeId** | **String**|  | [default to null]
 **productAttributeUpdate** | [**ProductAttributeUpdate**](ProductAttributeUpdate.md)|  |

### Return type

[**ProductAttribute**](ProductAttribute.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

