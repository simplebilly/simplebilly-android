# TrainingAssignmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTrainingAssignment**](TrainingAssignmentApi.md#createTrainingAssignment) | **POST** /api/v1/training-assignments | 
[**deleteTrainingAssignment**](TrainingAssignmentApi.md#deleteTrainingAssignment) | **DELETE** /api/v1/training-assignments/{id} | 
[**getTrainingAssignment**](TrainingAssignmentApi.md#getTrainingAssignment) | **GET** /api/v1/training-assignments/{id} | 
[**getTrainingAssignments**](TrainingAssignmentApi.md#getTrainingAssignments) | **GET** /api/v1/training-assignments/ | 
[**updateTrainingAssignment**](TrainingAssignmentApi.md#updateTrainingAssignment) | **PUT** /api/v1/training-assignments/{id} | 



## createTrainingAssignment

> TrainingAssignment createTrainingAssignment(trainingAssignmentCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingAssignmentApi;

TrainingAssignmentApi apiInstance = new TrainingAssignmentApi();
TrainingAssignmentCreate trainingAssignmentCreate = new TrainingAssignmentCreate(); // TrainingAssignmentCreate | 
try {
    TrainingAssignment result = apiInstance.createTrainingAssignment(trainingAssignmentCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingAssignmentApi#createTrainingAssignment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **trainingAssignmentCreate** | [**TrainingAssignmentCreate**](TrainingAssignmentCreate.md)|  |

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteTrainingAssignment

> deleteTrainingAssignment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingAssignmentApi;

TrainingAssignmentApi apiInstance = new TrainingAssignmentApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteTrainingAssignment(id);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingAssignmentApi#deleteTrainingAssignment");
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


## getTrainingAssignment

> TrainingAssignment getTrainingAssignment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingAssignmentApi;

TrainingAssignmentApi apiInstance = new TrainingAssignmentApi();
UUID id = null; // UUID | 
try {
    TrainingAssignment result = apiInstance.getTrainingAssignment(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingAssignmentApi#getTrainingAssignment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTrainingAssignments

> List&lt;TrainingAssignment&gt; getTrainingAssignments(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingAssignmentApi;

TrainingAssignmentApi apiInstance = new TrainingAssignmentApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<TrainingAssignment> result = apiInstance.getTrainingAssignments(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingAssignmentApi#getTrainingAssignments");
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

[**List&lt;TrainingAssignment&gt;**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTrainingAssignment

> TrainingAssignment updateTrainingAssignment(id, trainingAssignmentUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingAssignmentApi;

TrainingAssignmentApi apiInstance = new TrainingAssignmentApi();
UUID id = null; // UUID | 
TrainingAssignmentUpdate trainingAssignmentUpdate = new TrainingAssignmentUpdate(); // TrainingAssignmentUpdate | 
try {
    TrainingAssignment result = apiInstance.updateTrainingAssignment(id, trainingAssignmentUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingAssignmentApi#updateTrainingAssignment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **trainingAssignmentUpdate** | [**TrainingAssignmentUpdate**](TrainingAssignmentUpdate.md)|  |

### Return type

[**TrainingAssignment**](TrainingAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

