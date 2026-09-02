# ProductCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductCategory**](ProductCategoryApi.md#createProductCategory) | **POST** /api/v1/product-categories | 
[**deleteProductCategory**](ProductCategoryApi.md#deleteProductCategory) | **DELETE** /api/v1/product-categories/{category_id} | 
[**getProductCategory**](ProductCategoryApi.md#getProductCategory) | **GET** /api/v1/product-categories/{category_id} | 
[**listProductCategories**](ProductCategoryApi.md#listProductCategories) | **GET** /api/v1/product-categories | 
[**updateProductCategory**](ProductCategoryApi.md#updateProductCategory) | **PUT** /api/v1/product-categories/{category_id} | 



## createProductCategory

> ProductCategory createProductCategory(productCategory)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductCategoryApi;

ProductCategoryApi apiInstance = new ProductCategoryApi();
ProductCategory productCategory = new ProductCategory(); // ProductCategory | 
try {
    ProductCategory result = apiInstance.createProductCategory(productCategory);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductCategoryApi#createProductCategory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productCategory** | [**ProductCategory**](ProductCategory.md)|  |

### Return type

[**ProductCategory**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductCategory

> deleteProductCategory(categoryId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductCategoryApi;

ProductCategoryApi apiInstance = new ProductCategoryApi();
String categoryId = null; // String | 
try {
    apiInstance.deleteProductCategory(categoryId);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductCategoryApi#deleteProductCategory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductCategory

> ProductCategory getProductCategory(categoryId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductCategoryApi;

ProductCategoryApi apiInstance = new ProductCategoryApi();
String categoryId = null; // String | 
try {
    ProductCategory result = apiInstance.getProductCategory(categoryId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductCategoryApi#getProductCategory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **String**|  | [default to null]

### Return type

[**ProductCategory**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductCategories

> List&lt;ProductCategory&gt; listProductCategories()



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductCategoryApi;

ProductCategoryApi apiInstance = new ProductCategoryApi();
try {
    List<ProductCategory> result = apiInstance.listProductCategories();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductCategoryApi#listProductCategories");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;ProductCategory&gt;**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductCategory

> ProductCategory updateProductCategory(categoryId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductCategoryApi;

ProductCategoryApi apiInstance = new ProductCategoryApi();
String categoryId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    ProductCategory result = apiInstance.updateProductCategory(categoryId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductCategoryApi#updateProductCategory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**ProductCategory**](ProductCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

