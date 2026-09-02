# ActivityApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createActivity**](ActivityApi.md#createActivity) | **POST** /api/v1/activities | 
[**deleteActivity**](ActivityApi.md#deleteActivity) | **DELETE** /api/v1/activities/{activity_id} | 
[**getActivity**](ActivityApi.md#getActivity) | **GET** /api/v1/activities/{activity_id} | 
[**listActivities**](ActivityApi.md#listActivities) | **GET** /api/v1/activities/ | 
[**updateActivity**](ActivityApi.md#updateActivity) | **PUT** /api/v1/activities/{activity_id} | 
[**updateActivityStatus**](ActivityApi.md#updateActivityStatus) | **PUT** /api/v1/activities/{activity_id}/status | 



## createActivity

> Activity createActivity(activity)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ActivityApi;

ActivityApi apiInstance = new ActivityApi();
Activity activity = new Activity(); // Activity | 
try {
    Activity result = apiInstance.createActivity(activity);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ActivityApi#createActivity");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activity** | [**Activity**](Activity.md)|  |

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteActivity

> deleteActivity(activityId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ActivityApi;

ActivityApi apiInstance = new ActivityApi();
String activityId = null; // String | 
try {
    apiInstance.deleteActivity(activityId);
} catch (ApiException e) {
    System.err.println("Exception when calling ActivityApi#deleteActivity");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getActivity

> Activity getActivity(activityId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ActivityApi;

ActivityApi apiInstance = new ActivityApi();
String activityId = null; // String | 
try {
    Activity result = apiInstance.getActivity(activityId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ActivityApi#getActivity");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **String**|  | [default to null]

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listActivities

> List&lt;Activity&gt; listActivities(page, pageSize, contactId, activityType, status, assignedTo, overdueOnly)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ActivityApi;

ActivityApi apiInstance = new ActivityApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String contactId = null; // String | 
String activityType = null; // String | 
String status = null; // String | 
String assignedTo = null; // String | 
Boolean overdueOnly = null; // Boolean | Only show overdue follow-ups.
try {
    List<Activity> result = apiInstance.listActivities(page, pageSize, contactId, activityType, status, assignedTo, overdueOnly);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ActivityApi#listActivities");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **contactId** | **String**|  | [optional] [default to null]
 **activityType** | **String**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **assignedTo** | **String**|  | [optional] [default to null]
 **overdueOnly** | **Boolean**| Only show overdue follow-ups. | [optional] [default to null]

### Return type

[**List&lt;Activity&gt;**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateActivity

> Activity updateActivity(activityId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ActivityApi;

ActivityApi apiInstance = new ActivityApi();
String activityId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Activity result = apiInstance.updateActivity(activityId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ActivityApi#updateActivity");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateActivityStatus

> Activity updateActivityStatus(activityId, activityStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ActivityApi;

ActivityApi apiInstance = new ActivityApi();
String activityId = null; // String | 
ActivityStatusUpdate activityStatusUpdate = new ActivityStatusUpdate(); // ActivityStatusUpdate | 
try {
    Activity result = apiInstance.updateActivityStatus(activityId, activityStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ActivityApi#updateActivityStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **activityId** | **String**|  | [default to null]
 **activityStatusUpdate** | [**ActivityStatusUpdate**](ActivityStatusUpdate.md)|  |

### Return type

[**Activity**](Activity.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

