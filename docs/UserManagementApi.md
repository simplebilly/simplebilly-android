# UserManagementApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getUser**](UserManagementApi.md#getUser) | **GET** /api/v1/users/{user_id} | 
[**listUsers**](UserManagementApi.md#listUsers) | **GET** /api/v1/users | 
[**removeUser**](UserManagementApi.md#removeUser) | **DELETE** /api/v1/users/{user_id} | 
[**updateUserPermissions**](UserManagementApi.md#updateUserPermissions) | **PUT** /api/v1/users/{user_id}/permissions | 
[**updateUserRole**](UserManagementApi.md#updateUserRole) | **PUT** /api/v1/users/{user_id}/role | 



## getUser

> TenantUser getUser(userId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.UserManagementApi;

UserManagementApi apiInstance = new UserManagementApi();
UUID userId = null; // UUID | 
try {
    TenantUser result = apiInstance.getUser(userId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserManagementApi#getUser");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **UUID**|  | [default to null]

### Return type

[**TenantUser**](TenantUser.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listUsers

> List&lt;TenantUser&gt; listUsers()



### Example

```java
// Import classes:
//import org.openapitools.client.api.UserManagementApi;

UserManagementApi apiInstance = new UserManagementApi();
try {
    List<TenantUser> result = apiInstance.listUsers();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserManagementApi#listUsers");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;TenantUser&gt;**](TenantUser.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## removeUser

> removeUser(userId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.UserManagementApi;

UserManagementApi apiInstance = new UserManagementApi();
UUID userId = null; // UUID | 
try {
    apiInstance.removeUser(userId);
} catch (ApiException e) {
    System.err.println("Exception when calling UserManagementApi#removeUser");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## updateUserPermissions

> updateUserPermissions(userId, updatePermissionsPayload)



### Example

```java
// Import classes:
//import org.openapitools.client.api.UserManagementApi;

UserManagementApi apiInstance = new UserManagementApi();
UUID userId = null; // UUID | 
UpdatePermissionsPayload updatePermissionsPayload = new UpdatePermissionsPayload(); // UpdatePermissionsPayload | 
try {
    apiInstance.updateUserPermissions(userId, updatePermissionsPayload);
} catch (ApiException e) {
    System.err.println("Exception when calling UserManagementApi#updateUserPermissions");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **UUID**|  | [default to null]
 **updatePermissionsPayload** | [**UpdatePermissionsPayload**](UpdatePermissionsPayload.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## updateUserRole

> updateUserRole(userId, updateRolePayload)



### Example

```java
// Import classes:
//import org.openapitools.client.api.UserManagementApi;

UserManagementApi apiInstance = new UserManagementApi();
UUID userId = null; // UUID | 
UpdateRolePayload updateRolePayload = new UpdateRolePayload(); // UpdateRolePayload | 
try {
    apiInstance.updateUserRole(userId, updateRolePayload);
} catch (ApiException e) {
    System.err.println("Exception when calling UserManagementApi#updateUserRole");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **userId** | **UUID**|  | [default to null]
 **updateRolePayload** | [**UpdateRolePayload**](UpdateRolePayload.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined

