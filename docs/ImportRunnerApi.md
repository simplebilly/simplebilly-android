# ImportRunnerApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getImportStatus**](ImportRunnerApi.md#getImportStatus) | **GET** /api/v1/import/{job_id} | 
[**startImport**](ImportRunnerApi.md#startImport) | **POST** /api/v1/import/start | 
[**testImportConnection**](ImportRunnerApi.md#testImportConnection) | **POST** /api/v1/import/test | 



## getImportStatus

> ImportJobStatus getImportStatus(jobId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ImportRunnerApi;

ImportRunnerApi apiInstance = new ImportRunnerApi();
String jobId = null; // String | 
try {
    ImportJobStatus result = apiInstance.getImportStatus(jobId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ImportRunnerApi#getImportStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jobId** | **String**|  | [default to null]

### Return type

[**ImportJobStatus**](ImportJobStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## startImport

> ImportStartResponse startImport(importStartRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ImportRunnerApi;

ImportRunnerApi apiInstance = new ImportRunnerApi();
ImportStartRequest importStartRequest = new ImportStartRequest(); // ImportStartRequest | 
try {
    ImportStartResponse result = apiInstance.startImport(importStartRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ImportRunnerApi#startImport");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **importStartRequest** | [**ImportStartRequest**](ImportStartRequest.md)|  |

### Return type

[**ImportStartResponse**](ImportStartResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## testImportConnection

> ImportTestResponse testImportConnection(importTestRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ImportRunnerApi;

ImportRunnerApi apiInstance = new ImportRunnerApi();
ImportTestRequest importTestRequest = new ImportTestRequest(); // ImportTestRequest | 
try {
    ImportTestResponse result = apiInstance.testImportConnection(importTestRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ImportRunnerApi#testImportConnection");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **importTestRequest** | [**ImportTestRequest**](ImportTestRequest.md)|  |

### Return type

[**ImportTestResponse**](ImportTestResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

