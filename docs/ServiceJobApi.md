# ServiceJobApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createServiceJob**](ServiceJobApi.md#createServiceJob) | **POST** /api/v1/service-jobs | 
[**deleteServiceJob**](ServiceJobApi.md#deleteServiceJob) | **DELETE** /api/v1/service-jobs/{id} | 
[**getServiceJob**](ServiceJobApi.md#getServiceJob) | **GET** /api/v1/service-jobs/{id} | 
[**getServiceJobs**](ServiceJobApi.md#getServiceJobs) | **GET** /api/v1/service-jobs/ | 
[**updateServiceJob**](ServiceJobApi.md#updateServiceJob) | **PUT** /api/v1/service-jobs/{id} | 



## createServiceJob

> ServiceJob createServiceJob(serviceJobCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceJobApi;

ServiceJobApi apiInstance = new ServiceJobApi();
ServiceJobCreate serviceJobCreate = new ServiceJobCreate(); // ServiceJobCreate | 
try {
    ServiceJob result = apiInstance.createServiceJob(serviceJobCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceJobApi#createServiceJob");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **serviceJobCreate** | [**ServiceJobCreate**](ServiceJobCreate.md)|  |

### Return type

[**ServiceJob**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteServiceJob

> deleteServiceJob(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceJobApi;

ServiceJobApi apiInstance = new ServiceJobApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteServiceJob(id);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceJobApi#deleteServiceJob");
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


## getServiceJob

> ServiceJob getServiceJob(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceJobApi;

ServiceJobApi apiInstance = new ServiceJobApi();
UUID id = null; // UUID | 
try {
    ServiceJob result = apiInstance.getServiceJob(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceJobApi#getServiceJob");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**ServiceJob**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getServiceJobs

> List&lt;ServiceJob&gt; getServiceJobs(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceJobApi;

ServiceJobApi apiInstance = new ServiceJobApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<ServiceJob> result = apiInstance.getServiceJobs(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceJobApi#getServiceJobs");
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

[**List&lt;ServiceJob&gt;**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateServiceJob

> ServiceJob updateServiceJob(id, serviceJobUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ServiceJobApi;

ServiceJobApi apiInstance = new ServiceJobApi();
UUID id = null; // UUID | 
ServiceJobUpdate serviceJobUpdate = new ServiceJobUpdate(); // ServiceJobUpdate | 
try {
    ServiceJob result = apiInstance.updateServiceJob(id, serviceJobUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ServiceJobApi#updateServiceJob");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **serviceJobUpdate** | [**ServiceJobUpdate**](ServiceJobUpdate.md)|  |

### Return type

[**ServiceJob**](ServiceJob.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

