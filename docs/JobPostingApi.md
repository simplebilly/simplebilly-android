# JobPostingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createJobPosting**](JobPostingApi.md#createJobPosting) | **POST** /api/v1/job-postings | 
[**deleteJobPosting**](JobPostingApi.md#deleteJobPosting) | **DELETE** /api/v1/job-postings/{id} | 
[**getJobPosting**](JobPostingApi.md#getJobPosting) | **GET** /api/v1/job-postings/{id} | 
[**listJobPostings**](JobPostingApi.md#listJobPostings) | **GET** /api/v1/job-postings | 
[**updateJobPosting**](JobPostingApi.md#updateJobPosting) | **PUT** /api/v1/job-postings/{id} | 



## createJobPosting

> JobPosting createJobPosting(jobPostingCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobPostingApi;

JobPostingApi apiInstance = new JobPostingApi();
JobPostingCreate jobPostingCreate = new JobPostingCreate(); // JobPostingCreate | 
try {
    JobPosting result = apiInstance.createJobPosting(jobPostingCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobPostingApi#createJobPosting");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **jobPostingCreate** | [**JobPostingCreate**](JobPostingCreate.md)|  |

### Return type

[**JobPosting**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteJobPosting

> deleteJobPosting(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobPostingApi;

JobPostingApi apiInstance = new JobPostingApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteJobPosting(id);
} catch (ApiException e) {
    System.err.println("Exception when calling JobPostingApi#deleteJobPosting");
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


## getJobPosting

> JobPosting getJobPosting(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobPostingApi;

JobPostingApi apiInstance = new JobPostingApi();
UUID id = null; // UUID | 
try {
    JobPosting result = apiInstance.getJobPosting(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobPostingApi#getJobPosting");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**JobPosting**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listJobPostings

> List&lt;JobPosting&gt; listJobPostings(status, page, pageSize)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobPostingApi;

JobPostingApi apiInstance = new JobPostingApi();
String status = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    List<JobPosting> result = apiInstance.listJobPostings(status, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobPostingApi#listJobPostings");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**List&lt;JobPosting&gt;**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateJobPosting

> JobPosting updateJobPosting(id, jobPostingUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobPostingApi;

JobPostingApi apiInstance = new JobPostingApi();
UUID id = null; // UUID | 
JobPostingUpdate jobPostingUpdate = new JobPostingUpdate(); // JobPostingUpdate | 
try {
    JobPosting result = apiInstance.updateJobPosting(id, jobPostingUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobPostingApi#updateJobPosting");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **jobPostingUpdate** | [**JobPostingUpdate**](JobPostingUpdate.md)|  |

### Return type

[**JobPosting**](JobPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

