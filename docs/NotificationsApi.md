# NotificationsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**deleteNotification**](NotificationsApi.md#deleteNotification) | **DELETE** /api/v1/notifications/{id} | 
[**listNotifications**](NotificationsApi.md#listNotifications) | **GET** /api/v1/notifications | 
[**markAllRead**](NotificationsApi.md#markAllRead) | **PUT** /api/v1/notifications/read-all | 
[**markAsRead**](NotificationsApi.md#markAsRead) | **PUT** /api/v1/notifications/{id}/read | 
[**unreadCount**](NotificationsApi.md#unreadCount) | **GET** /api/v1/notifications/unread-count | 



## deleteNotification

> deleteNotification(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.NotificationsApi;

NotificationsApi apiInstance = new NotificationsApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteNotification(id);
} catch (ApiException e) {
    System.err.println("Exception when calling NotificationsApi#deleteNotification");
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
- **Accept**: Not defined


## listNotifications

> List&lt;NotificationDto&gt; listNotifications()



### Example

```java
// Import classes:
//import org.openapitools.client.api.NotificationsApi;

NotificationsApi apiInstance = new NotificationsApi();
try {
    List<NotificationDto> result = apiInstance.listNotifications();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling NotificationsApi#listNotifications");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;NotificationDto&gt;**](NotificationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## markAllRead

> Long markAllRead()



### Example

```java
// Import classes:
//import org.openapitools.client.api.NotificationsApi;

NotificationsApi apiInstance = new NotificationsApi();
try {
    Long result = apiInstance.markAllRead();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling NotificationsApi#markAllRead");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Long**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain


## markAsRead

> markAsRead(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.NotificationsApi;

NotificationsApi apiInstance = new NotificationsApi();
UUID id = null; // UUID | 
try {
    apiInstance.markAsRead(id);
} catch (ApiException e) {
    System.err.println("Exception when calling NotificationsApi#markAsRead");
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
- **Accept**: Not defined


## unreadCount

> Long unreadCount()



### Example

```java
// Import classes:
//import org.openapitools.client.api.NotificationsApi;

NotificationsApi apiInstance = new NotificationsApi();
try {
    Long result = apiInstance.unreadCount();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling NotificationsApi#unreadCount");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

**Long**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: text/plain

