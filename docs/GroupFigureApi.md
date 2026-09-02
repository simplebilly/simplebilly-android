# GroupFigureApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createGroupFigure**](GroupFigureApi.md#createGroupFigure) | **POST** /api/v1/group-figures | 
[**deleteGroupFigure**](GroupFigureApi.md#deleteGroupFigure) | **DELETE** /api/v1/group-figures/{year} | 
[**getGroupFigure**](GroupFigureApi.md#getGroupFigure) | **GET** /api/v1/group-figures/{year} | 
[**getGroupFigures**](GroupFigureApi.md#getGroupFigures) | **GET** /api/v1/group-figures/ | 
[**updateGroupFigure**](GroupFigureApi.md#updateGroupFigure) | **PUT** /api/v1/group-figures/{year} | 



## createGroupFigure

> GroupFigure createGroupFigure(groupFigureCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GroupFigureApi;

GroupFigureApi apiInstance = new GroupFigureApi();
GroupFigureCreate groupFigureCreate = new GroupFigureCreate(); // GroupFigureCreate | 
try {
    GroupFigure result = apiInstance.createGroupFigure(groupFigureCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupFigureApi#createGroupFigure");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **groupFigureCreate** | [**GroupFigureCreate**](GroupFigureCreate.md)|  |

### Return type

[**GroupFigure**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteGroupFigure

> deleteGroupFigure(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GroupFigureApi;

GroupFigureApi apiInstance = new GroupFigureApi();
Integer year = null; // Integer | 
try {
    apiInstance.deleteGroupFigure(year);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupFigureApi#deleteGroupFigure");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getGroupFigure

> GroupFigure getGroupFigure(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GroupFigureApi;

GroupFigureApi apiInstance = new GroupFigureApi();
Integer year = null; // Integer | 
try {
    GroupFigure result = apiInstance.getGroupFigure(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupFigureApi#getGroupFigure");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**GroupFigure**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getGroupFigures

> List&lt;GroupFigure&gt; getGroupFigures(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GroupFigureApi;

GroupFigureApi apiInstance = new GroupFigureApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<GroupFigure> result = apiInstance.getGroupFigures(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupFigureApi#getGroupFigures");
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

[**List&lt;GroupFigure&gt;**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateGroupFigure

> GroupFigure updateGroupFigure(year, groupFigureUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GroupFigureApi;

GroupFigureApi apiInstance = new GroupFigureApi();
Integer year = null; // Integer | 
GroupFigureUpdate groupFigureUpdate = new GroupFigureUpdate(); // GroupFigureUpdate | 
try {
    GroupFigure result = apiInstance.updateGroupFigure(year, groupFigureUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GroupFigureApi#updateGroupFigure");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]
 **groupFigureUpdate** | [**GroupFigureUpdate**](GroupFigureUpdate.md)|  |

### Return type

[**GroupFigure**](GroupFigure.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

