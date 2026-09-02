# ProductApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductApi**](ProductApi.md#createProductApi) | **POST** /api/v1/products | 
[**deleteProductApi**](ProductApi.md#deleteProductApi) | **DELETE** /api/v1/products/{product_id} | 
[**getProductApi**](ProductApi.md#getProductApi) | **GET** /api/v1/products/{product_id} | 
[**getProductStockApi**](ProductApi.md#getProductStockApi) | **GET** /api/v1/products/{product_id}/stock | 
[**getProductsApi**](ProductApi.md#getProductsApi) | **GET** /api/v1/products/ | 
[**listLowStockProductsApi**](ProductApi.md#listLowStockProductsApi) | **GET** /api/v1/products/low-stock | 
[**productRestore**](ProductApi.md#productRestore) | **POST** /api/v1/products/{product_id}/restore | 
[**updateProductApi**](ProductApi.md#updateProductApi) | **PUT** /api/v1/products/{product_id} | 
[**updateProductStockApi**](ProductApi.md#updateProductStockApi) | **PUT** /api/v1/products/{product_id}/stock | 



## createProductApi

> Product createProductApi(productCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
ProductCreate productCreate = new ProductCreate(); // ProductCreate | 
try {
    Product result = apiInstance.createProductApi(productCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#createProductApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productCreate** | [**ProductCreate**](ProductCreate.md)|  |

### Return type

[**Product**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductApi

> deleteProductApi(productId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
UUID productId = null; // UUID | 
try {
    apiInstance.deleteProductApi(productId);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#deleteProductApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductApi

> Product getProductApi(productId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
UUID productId = null; // UUID | 
try {
    Product result = apiInstance.getProductApi(productId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#getProductApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]

### Return type

[**Product**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductStockApi

> ProductStock getProductStockApi(productId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
UUID productId = null; // UUID | 
try {
    ProductStock result = apiInstance.getProductStockApi(productId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#getProductStockApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]

### Return type

[**ProductStock**](ProductStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getProductsApi

> List&lt;Product&gt; getProductsApi(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Product> result = apiInstance.getProductsApi(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#getProductsApi");
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

[**List&lt;Product&gt;**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listLowStockProductsApi

> List&lt;ProductStock&gt; listLowStockProductsApi(threshold)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
Long threshold = null; // Long | 
try {
    List<ProductStock> result = apiInstance.listLowStockProductsApi(threshold);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#listLowStockProductsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **threshold** | **Long**|  | [optional] [default to null]

### Return type

[**List&lt;ProductStock&gt;**](ProductStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## productRestore

> Product productRestore(productId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
UUID productId = null; // UUID | 
try {
    Product result = apiInstance.productRestore(productId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#productRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]

### Return type

[**Product**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductApi

> Product updateProductApi(productId, productUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
UUID productId = null; // UUID | 
ProductUpdate productUpdate = new ProductUpdate(); // ProductUpdate | 
try {
    Product result = apiInstance.updateProductApi(productId, productUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#updateProductApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]
 **productUpdate** | [**ProductUpdate**](ProductUpdate.md)|  |

### Return type

[**Product**](Product.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateProductStockApi

> ProductStock updateProductStockApi(productId, stockUpdateRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductApi;

ProductApi apiInstance = new ProductApi();
UUID productId = null; // UUID | 
StockUpdateRequest stockUpdateRequest = new StockUpdateRequest(); // StockUpdateRequest | 
try {
    ProductStock result = apiInstance.updateProductStockApi(productId, stockUpdateRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductApi#updateProductStockApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productId** | **UUID**|  | [default to null]
 **stockUpdateRequest** | [**StockUpdateRequest**](StockUpdateRequest.md)|  |

### Return type

[**ProductStock**](ProductStock.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

