# TenantSettingsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getTenantSettings**](TenantSettingsApi.md#getTenantSettings) | **GET** /api/v1/settings/tenant | 
[**updateTenantSettings**](TenantSettingsApi.md#updateTenantSettings) | **PUT** /api/v1/settings/tenant | 



## getTenantSettings

> TenantSettings getTenantSettings()



### Example

```java
// Import classes:
//import org.openapitools.client.api.TenantSettingsApi;

TenantSettingsApi apiInstance = new TenantSettingsApi();
try {
    TenantSettings result = apiInstance.getTenantSettings();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TenantSettingsApi#getTenantSettings");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**TenantSettings**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTenantSettings

> TenantSettings updateTenantSettings(updateTenantSettings)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TenantSettingsApi;

TenantSettingsApi apiInstance = new TenantSettingsApi();
UpdateTenantSettings updateTenantSettings = new UpdateTenantSettings(); // UpdateTenantSettings | 
try {
    TenantSettings result = apiInstance.updateTenantSettings(updateTenantSettings);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TenantSettingsApi#updateTenantSettings");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **updateTenantSettings** | [**UpdateTenantSettings**](UpdateTenantSettings.md)|  |

### Return type

[**TenantSettings**](TenantSettings.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

