# DeclarationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeclaration**](DeclarationApi.md#createDeclaration) | **POST** /api/v1/declarations | 
[**declarationRestore**](DeclarationApi.md#declarationRestore) | **POST** /api/v1/declarations/{id}/restore | 
[**deleteDeclaration**](DeclarationApi.md#deleteDeclaration) | **DELETE** /api/v1/declarations/{id} | 
[**getDeclaration**](DeclarationApi.md#getDeclaration) | **GET** /api/v1/declarations/{id} | 
[**getDeclarations**](DeclarationApi.md#getDeclarations) | **GET** /api/v1/declarations/ | 
[**updateDeclaration**](DeclarationApi.md#updateDeclaration) | **PUT** /api/v1/declarations/{id} | 



## createDeclaration

> Declaration createDeclaration(declarationCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeclarationApi;

DeclarationApi apiInstance = new DeclarationApi();
DeclarationCreate declarationCreate = new DeclarationCreate(); // DeclarationCreate | 
try {
    Declaration result = apiInstance.createDeclaration(declarationCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeclarationApi#createDeclaration");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **declarationCreate** | [**DeclarationCreate**](DeclarationCreate.md)|  |

### Return type

[**Declaration**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## declarationRestore

> Declaration declarationRestore(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeclarationApi;

DeclarationApi apiInstance = new DeclarationApi();
UUID id = null; // UUID | 
try {
    Declaration result = apiInstance.declarationRestore(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeclarationApi#declarationRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Declaration**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## deleteDeclaration

> deleteDeclaration(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeclarationApi;

DeclarationApi apiInstance = new DeclarationApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteDeclaration(id);
} catch (ApiException e) {
    System.err.println("Exception when calling DeclarationApi#deleteDeclaration");
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


## getDeclaration

> Declaration getDeclaration(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeclarationApi;

DeclarationApi apiInstance = new DeclarationApi();
UUID id = null; // UUID | 
try {
    Declaration result = apiInstance.getDeclaration(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeclarationApi#getDeclaration");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Declaration**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeclarations

> List&lt;Declaration&gt; getDeclarations(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeclarationApi;

DeclarationApi apiInstance = new DeclarationApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Declaration> result = apiInstance.getDeclarations(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeclarationApi#getDeclarations");
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

[**List&lt;Declaration&gt;**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateDeclaration

> Declaration updateDeclaration(id, declarationUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeclarationApi;

DeclarationApi apiInstance = new DeclarationApi();
UUID id = null; // UUID | 
DeclarationUpdate declarationUpdate = new DeclarationUpdate(); // DeclarationUpdate | 
try {
    Declaration result = apiInstance.updateDeclaration(id, declarationUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeclarationApi#updateDeclaration");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **declarationUpdate** | [**DeclarationUpdate**](DeclarationUpdate.md)|  |

### Return type

[**Declaration**](Declaration.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

