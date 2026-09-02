# ProductVariantApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createProductVariant**](ProductVariantApi.md#createProductVariant) | **POST** /api/v1/product-variants | 
[**deleteProductVariant**](ProductVariantApi.md#deleteProductVariant) | **DELETE** /api/v1/product-variants/{variant_id} | 
[**generateProductVariants**](ProductVariantApi.md#generateProductVariants) | **POST** /api/v1/product-variants/generate | 
[**getProductVariant**](ProductVariantApi.md#getProductVariant) | **GET** /api/v1/product-variants/{variant_id} | 
[**listProductVariants**](ProductVariantApi.md#listProductVariants) | **GET** /api/v1/product-variants/ | 
[**updateProductVariant**](ProductVariantApi.md#updateProductVariant) | **PUT** /api/v1/product-variants/{variant_id} | 



## createProductVariant

> ProductVariant createProductVariant(productVariant)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductVariantApi;

ProductVariantApi apiInstance = new ProductVariantApi();
ProductVariant productVariant = new ProductVariant(); // ProductVariant | 
try {
    ProductVariant result = apiInstance.createProductVariant(productVariant);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductVariantApi#createProductVariant");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **productVariant** | [**ProductVariant**](ProductVariant.md)|  |

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteProductVariant

> deleteProductVariant(variantId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductVariantApi;

ProductVariantApi apiInstance = new ProductVariantApi();
String variantId = null; // String | 
try {
    apiInstance.deleteProductVariant(variantId);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductVariantApi#deleteProductVariant");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variantId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## generateProductVariants

> List&lt;ProductVariant&gt; generateProductVariants(generateVariantsRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductVariantApi;

ProductVariantApi apiInstance = new ProductVariantApi();
GenerateVariantsRequest generateVariantsRequest = new GenerateVariantsRequest(); // GenerateVariantsRequest | 
try {
    List<ProductVariant> result = apiInstance.generateProductVariants(generateVariantsRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductVariantApi#generateProductVariants");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **generateVariantsRequest** | [**GenerateVariantsRequest**](GenerateVariantsRequest.md)|  |

### Return type

[**List&lt;ProductVariant&gt;**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## getProductVariant

> ProductVariant getProductVariant(variantId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductVariantApi;

ProductVariantApi apiInstance = new ProductVariantApi();
String variantId = null; // String | 
try {
    ProductVariant result = apiInstance.getProductVariant(variantId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductVariantApi#getProductVariant");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variantId** | **String**|  | [default to null]

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listProductVariants

> List&lt;ProductVariant&gt; listProductVariants(page, pageSize, productId, isActive)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductVariantApi;

ProductVariantApi apiInstance = new ProductVariantApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
UUID productId = null; // UUID | 
Boolean isActive = null; // Boolean | 
try {
    List<ProductVariant> result = apiInstance.listProductVariants(page, pageSize, productId, isActive);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductVariantApi#listProductVariants");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **productId** | **UUID**|  | [optional] [default to null]
 **isActive** | **Boolean**|  | [optional] [default to null]

### Return type

[**List&lt;ProductVariant&gt;**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateProductVariant

> ProductVariant updateProductVariant(variantId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProductVariantApi;

ProductVariantApi apiInstance = new ProductVariantApi();
String variantId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    ProductVariant result = apiInstance.updateProductVariant(variantId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProductVariantApi#updateProductVariant");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **variantId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**ProductVariant**](ProductVariant.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

