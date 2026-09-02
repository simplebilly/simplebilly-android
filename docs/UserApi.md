# UserApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**changePassword**](UserApi.md#changePassword) | **POST** /user/change-password | Change the current user&#39;s password (requires the current password).
[**createTeam**](UserApi.md#createTeam) | **POST** /user/teams | Create a new team within the current tenant
[**generateApiKey**](UserApi.md#generateApiKey) | **POST** /user/api-key | Generate a new API key for the current user
[**inviteUser**](UserApi.md#inviteUser) | **POST** /user/invite | Invite a user to the current tenant/organization
[**listTeams**](UserApi.md#listTeams) | **GET** /user/teams | List all teams in the current tenant
[**removeUserFromOrg**](UserApi.md#removeUserFromOrg) | **DELETE** /user/remove | Remove a user from the current organization
[**updateProfile**](UserApi.md#updateProfile) | **PUT** /user/profile | Update the current user&#39;s profile
[**userProfile**](UserApi.md#userProfile) | **GET** /user/profile | Get the current user&#39;s profile
[**userTenants**](UserApi.md#userTenants) | **GET** /user/tenants | List all tenants (organizations) the current user belongs to



## changePassword

> changePassword(changePasswordRequest)

Change the current user&#39;s password (requires the current password).

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
ChangePasswordRequest changePasswordRequest = new ChangePasswordRequest(); // ChangePasswordRequest | 
try {
    apiInstance.changePassword(changePasswordRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#changePassword");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **changePasswordRequest** | [**ChangePasswordRequest**](ChangePasswordRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## createTeam

> ApiResponseTeam createTeam(teamCreate)

Create a new team within the current tenant

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
TeamCreate teamCreate = new TeamCreate(); // TeamCreate | 
try {
    ApiResponseTeam result = apiInstance.createTeam(teamCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#createTeam");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **teamCreate** | [**TeamCreate**](TeamCreate.md)|  |

### Return type

[**ApiResponseTeam**](ApiResponseTeam.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## generateApiKey

> ApiResponseString generateApiKey()

Generate a new API key for the current user

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
try {
    ApiResponseString result = apiInstance.generateApiKey();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#generateApiKey");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseString**](ApiResponseString.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## inviteUser

> inviteUser(inviteRequest)

Invite a user to the current tenant/organization

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
InviteRequest inviteRequest = new InviteRequest(); // InviteRequest | 
try {
    apiInstance.inviteUser(inviteRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#inviteUser");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **inviteRequest** | [**InviteRequest**](InviteRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## listTeams

> ApiResponseVecTeam listTeams()

List all teams in the current tenant

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
try {
    ApiResponseVecTeam result = apiInstance.listTeams();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#listTeams");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseVecTeam**](ApiResponseVecTeam.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## removeUserFromOrg

> removeUserFromOrg(removeUserRequest)

Remove a user from the current organization

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
RemoveUserRequest removeUserRequest = new RemoveUserRequest(); // RemoveUserRequest | 
try {
    apiInstance.removeUserFromOrg(removeUserRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#removeUserFromOrg");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **removeUserRequest** | [**RemoveUserRequest**](RemoveUserRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## updateProfile

> updateProfile(updateProfileRequest)

Update the current user&#39;s profile

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
UpdateProfileRequest updateProfileRequest = new UpdateProfileRequest(); // UpdateProfileRequest | 
try {
    apiInstance.updateProfile(updateProfileRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#updateProfile");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateProfileRequest** | [**UpdateProfileRequest**](UpdateProfileRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: Not defined


## userProfile

> ApiResponseUserProfile userProfile()

Get the current user&#39;s profile

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
try {
    ApiResponseUserProfile result = apiInstance.userProfile();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userProfile");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseUserProfile**](ApiResponseUserProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## userTenants

> ApiResponseVecUserTenantInfo userTenants()

List all tenants (organizations) the current user belongs to

### Example

```java
// Import classes:
//import org.openapitools.client.api.UserApi;

UserApi apiInstance = new UserApi();
try {
    ApiResponseVecUserTenantInfo result = apiInstance.userTenants();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling UserApi#userTenants");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ApiResponseVecUserTenantInfo**](ApiResponseVecUserTenantInfo.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

