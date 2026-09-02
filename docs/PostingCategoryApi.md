# PostingCategoryApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createPostingCategory**](PostingCategoryApi.md#createPostingCategory) | **POST** /api/v1/posting-categories | 
[**deletePostingCategory**](PostingCategoryApi.md#deletePostingCategory) | **DELETE** /api/v1/posting-categories/{category_id} | 
[**listPostingCategories**](PostingCategoryApi.md#listPostingCategories) | **GET** /api/v1/posting-categories | 
[**seedPostingCategories**](PostingCategoryApi.md#seedPostingCategories) | **POST** /api/v1/posting-categories/seed/{skr_version} | 
[**updatePostingCategory**](PostingCategoryApi.md#updatePostingCategory) | **PUT** /api/v1/posting-categories/{category_id} | 



## createPostingCategory

> PostingCategory createPostingCategory(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PostingCategoryApi;

PostingCategoryApi apiInstance = new PostingCategoryApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    PostingCategory result = apiInstance.createPostingCategory(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PostingCategoryApi#createPostingCategory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**PostingCategory**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deletePostingCategory

> deletePostingCategory(categoryId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PostingCategoryApi;

PostingCategoryApi apiInstance = new PostingCategoryApi();
String categoryId = null; // String | 
try {
    apiInstance.deletePostingCategory(categoryId);
} catch (ApiException e) {
    System.err.println("Exception when calling PostingCategoryApi#deletePostingCategory");
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


## listPostingCategories

> List&lt;PostingCategory&gt; listPostingCategories()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PostingCategoryApi;

PostingCategoryApi apiInstance = new PostingCategoryApi();
try {
    List<PostingCategory> result = apiInstance.listPostingCategories();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PostingCategoryApi#listPostingCategories");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PostingCategory&gt;**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## seedPostingCategories

> seedPostingCategories(skrVersion)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PostingCategoryApi;

PostingCategoryApi apiInstance = new PostingCategoryApi();
String skrVersion = null; // String | 
try {
    apiInstance.seedPostingCategories(skrVersion);
} catch (ApiException e) {
    System.err.println("Exception when calling PostingCategoryApi#seedPostingCategories");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **skrVersion** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updatePostingCategory

> PostingCategory updatePostingCategory(categoryId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PostingCategoryApi;

PostingCategoryApi apiInstance = new PostingCategoryApi();
String categoryId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    PostingCategory result = apiInstance.updatePostingCategory(categoryId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PostingCategoryApi#updatePostingCategory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **categoryId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**PostingCategory**](PostingCategory.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

