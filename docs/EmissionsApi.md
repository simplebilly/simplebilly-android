# EmissionsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createEmissionEntryApi**](EmissionsApi.md#createEmissionEntryApi) | **POST** /api/v1/bookkeeping/emissions/entries | 
[**createEmissionTargetApi**](EmissionsApi.md#createEmissionTargetApi) | **POST** /api/v1/bookkeeping/emissions/targets | 
[**deleteEmissionEntryApi**](EmissionsApi.md#deleteEmissionEntryApi) | **DELETE** /api/v1/bookkeeping/emissions/entries/{id} | 
[**deleteEmissionTargetApi**](EmissionsApi.md#deleteEmissionTargetApi) | **DELETE** /api/v1/bookkeeping/emissions/targets/{id} | 
[**emissionsEntriesApi**](EmissionsApi.md#emissionsEntriesApi) | **GET** /api/v1/bookkeeping/emissions/entries | 
[**emissionsExportApi**](EmissionsApi.md#emissionsExportApi) | **GET** /api/v1/bookkeeping/emissions/export | 
[**emissionsFactorsApi**](EmissionsApi.md#emissionsFactorsApi) | **GET** /api/v1/bookkeeping/emissions/factors | 
[**emissionsReportApi**](EmissionsApi.md#emissionsReportApi) | **GET** /api/v1/bookkeeping/emissions/report | 
[**emissionsTargetsApi**](EmissionsApi.md#emissionsTargetsApi) | **GET** /api/v1/bookkeeping/emissions/targets | 



## createEmissionEntryApi

> EmissionEntry createEmissionEntryApi(createEmissionEntry)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
CreateEmissionEntry createEmissionEntry = new CreateEmissionEntry(); // CreateEmissionEntry | 
try {
    EmissionEntry result = apiInstance.createEmissionEntryApi(createEmissionEntry);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#createEmissionEntryApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createEmissionEntry** | [**CreateEmissionEntry**](CreateEmissionEntry.md)|  |

### Return type

[**EmissionEntry**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createEmissionTargetApi

> EmissionTarget createEmissionTargetApi(createEmissionTarget)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
CreateEmissionTarget createEmissionTarget = new CreateEmissionTarget(); // CreateEmissionTarget | 
try {
    EmissionTarget result = apiInstance.createEmissionTargetApi(createEmissionTarget);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#createEmissionTargetApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createEmissionTarget** | [**CreateEmissionTarget**](CreateEmissionTarget.md)|  |

### Return type

[**EmissionTarget**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteEmissionEntryApi

> deleteEmissionEntryApi(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteEmissionEntryApi(id);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#deleteEmissionEntryApi");
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


## deleteEmissionTargetApi

> deleteEmissionTargetApi(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteEmissionTargetApi(id);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#deleteEmissionTargetApi");
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


## emissionsEntriesApi

> List&lt;EmissionEntry&gt; emissionsEntriesApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
Integer year = null; // Integer | 
try {
    List<EmissionEntry> result = apiInstance.emissionsEntriesApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#emissionsEntriesApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**List&lt;EmissionEntry&gt;**](EmissionEntry.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsExportApi

> EmissionsExportResponse emissionsExportApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
Integer year = null; // Integer | 
try {
    EmissionsExportResponse result = apiInstance.emissionsExportApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#emissionsExportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**EmissionsExportResponse**](EmissionsExportResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsFactorsApi

> List&lt;EmissionFactorResponse&gt; emissionsFactorsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
try {
    List<EmissionFactorResponse> result = apiInstance.emissionsFactorsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#emissionsFactorsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;EmissionFactorResponse&gt;**](EmissionFactorResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsReportApi

> EmissionsReport emissionsReportApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
Integer year = null; // Integer | 
try {
    EmissionsReport result = apiInstance.emissionsReportApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#emissionsReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**EmissionsReport**](EmissionsReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## emissionsTargetsApi

> List&lt;EmissionTarget&gt; emissionsTargetsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmissionsApi;

EmissionsApi apiInstance = new EmissionsApi();
try {
    List<EmissionTarget> result = apiInstance.emissionsTargetsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmissionsApi#emissionsTargetsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;EmissionTarget&gt;**](EmissionTarget.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

