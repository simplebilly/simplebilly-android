# InstituteProfileApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getInstituteProfile**](InstituteProfileApi.md#getInstituteProfile) | **GET** /api/v1/institute-profile | Current institute profile (created with defaults when missing).
[**updateInstituteProfile**](InstituteProfileApi.md#updateInstituteProfile) | **PUT** /api/v1/institute-profile | Update the institute profile (institute_type and/or kapitalmarktorientiert).



## getInstituteProfile

> InstituteProfile getInstituteProfile()

Current institute profile (created with defaults when missing).

### Example

```java
// Import classes:
//import org.openapitools.client.api.InstituteProfileApi;

InstituteProfileApi apiInstance = new InstituteProfileApi();
try {
    InstituteProfile result = apiInstance.getInstituteProfile();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InstituteProfileApi#getInstituteProfile");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateInstituteProfile

> InstituteProfile updateInstituteProfile(instituteProfileUpdate)

Update the institute profile (institute_type and/or kapitalmarktorientiert).

### Example

```java
// Import classes:
//import org.openapitools.client.api.InstituteProfileApi;

InstituteProfileApi apiInstance = new InstituteProfileApi();
InstituteProfileUpdate instituteProfileUpdate = new InstituteProfileUpdate(); // InstituteProfileUpdate | 
try {
    InstituteProfile result = apiInstance.updateInstituteProfile(instituteProfileUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling InstituteProfileApi#updateInstituteProfile");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **instituteProfileUpdate** | [**InstituteProfileUpdate**](InstituteProfileUpdate.md)|  |

### Return type

[**InstituteProfile**](InstituteProfile.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

