# ServiceAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createServiceAssignment**](ServiceAssignmentApi.md#createServiceAssignment) | **POST** /api/v1/service-assignments | 
[**deleteServiceAssignment**](ServiceAssignmentApi.md#deleteServiceAssignment) | **DELETE** /api/v1/service-assignments/{id} | 
[**getServiceAssignment**](ServiceAssignmentApi.md#getServiceAssignment) | **GET** /api/v1/service-assignments/{id} | 
[**getServiceAssignments**](ServiceAssignmentApi.md#getServiceAssignments) | **GET** /api/v1/service-assignments/ | 
[**updateServiceAssignment**](ServiceAssignmentApi.md#updateServiceAssignment) | **PUT** /api/v1/service-assignments/{id} | 



## createServiceAssignment

> ServiceAssignment createServiceAssignment(serviceAssignmentCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceAssignmentApi;

ServiceAssignmentApi apiInstance = new ServiceAssignmentApi();
ServiceAssignmentCreate serviceAssignmentCreate = new ServiceAssignmentCreate(); // ServiceAssignmentCreate | 
try {
    ServiceAssignment result = apiInstance.createServiceAssignment(serviceAssignmentCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceAssignmentApi#createServiceAssignment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **serviceAssignmentCreate** | [**ServiceAssignmentCreate**](ServiceAssignmentCreate.md)|  |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteServiceAssignment

> deleteServiceAssignment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceAssignmentApi;

ServiceAssignmentApi apiInstance = new ServiceAssignmentApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteServiceAssignment(id);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceAssignmentApi#deleteServiceAssignment");
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


## getServiceAssignment

> ServiceAssignment getServiceAssignment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceAssignmentApi;

ServiceAssignmentApi apiInstance = new ServiceAssignmentApi();
UUID id = null; // UUID | 
try {
    ServiceAssignment result = apiInstance.getServiceAssignment(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceAssignmentApi#getServiceAssignment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getServiceAssignments

> List&lt;ServiceAssignment&gt; getServiceAssignments(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceAssignmentApi;

ServiceAssignmentApi apiInstance = new ServiceAssignmentApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<ServiceAssignment> result = apiInstance.getServiceAssignments(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceAssignmentApi#getServiceAssignments");
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

[**List&lt;ServiceAssignment&gt;**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateServiceAssignment

> ServiceAssignment updateServiceAssignment(id, serviceAssignmentUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceAssignmentApi;

ServiceAssignmentApi apiInstance = new ServiceAssignmentApi();
UUID id = null; // UUID | 
ServiceAssignmentUpdate serviceAssignmentUpdate = new ServiceAssignmentUpdate(); // ServiceAssignmentUpdate | 
try {
    ServiceAssignment result = apiInstance.updateServiceAssignment(id, serviceAssignmentUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceAssignmentApi#updateServiceAssignment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **serviceAssignmentUpdate** | [**ServiceAssignmentUpdate**](ServiceAssignmentUpdate.md)|  |

### Return type

[**ServiceAssignment**](ServiceAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

