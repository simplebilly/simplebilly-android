# JobApplicationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**applyPublic**](JobApplicationApi.md#applyPublic) | **POST** /api/v1/public/jobs/{posting_id}/apply | 
[**deleteJobApplication**](JobApplicationApi.md#deleteJobApplication) | **DELETE** /api/v1/job-applications/{application_id} | 
[**downloadCv**](JobApplicationApi.md#downloadCv) | **GET** /api/v1/job-applications/{application_id}/cv | 
[**getJobApplication**](JobApplicationApi.md#getJobApplication) | **GET** /api/v1/job-applications/{application_id} | 
[**inboundEmail**](JobApplicationApi.md#inboundEmail) | **POST** /api/v1/public/jobs/inbound-email | Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox.
[**listJobApplications**](JobApplicationApi.md#listJobApplications) | **GET** /api/v1/job-applications | 
[**listPublicPostings**](JobApplicationApi.md#listPublicPostings) | **GET** /api/v1/public/jobs | 
[**scoreJobApplication**](JobApplicationApi.md#scoreJobApplication) | **POST** /api/v1/job-applications/{application_id}/score | 
[**updateJobApplicationStatus**](JobApplicationApi.md#updateJobApplicationStatus) | **PATCH** /api/v1/job-applications/{application_id}/status | 



## applyPublic

> applyPublic(postingId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID postingId = null; // UUID | 
try {
    apiInstance.applyPublic(postingId);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#applyPublic");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **postingId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## deleteJobApplication

> JobApplication deleteJobApplication(applicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID applicationId = null; // UUID | 
try {
    JobApplication result = apiInstance.deleteJobApplication(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#deleteJobApplication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | **UUID**|  | [default to null]

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## downloadCv

> downloadCv(applicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID applicationId = null; // UUID | 
try {
    apiInstance.downloadCv(applicationId);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#downloadCv");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getJobApplication

> JobApplication getJobApplication(applicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID applicationId = null; // UUID | 
try {
    JobApplication result = apiInstance.getJobApplication(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#getJobApplication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | **UUID**|  | [default to null]

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## inboundEmail

> inboundEmail()

Inbound CV email, mailgun/sendgrid inbound-parse style: multipart form with &#x60;from&#x60;, &#x60;subject&#x60;, &#x60;body-plain&#x60; and one or more &#x60;attachment-N&#x60; file fields. The subject may reference a posting as &#x60;[JOB-&lt;posting_id&gt;]&#x60;; without one the application lands in the general inbox.

### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
try {
    apiInstance.inboundEmail();
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#inboundEmail");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## listJobApplications

> List&lt;JobApplication&gt; listJobApplications(postingId, status, page, pageSize)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID postingId = null; // UUID | 
String status = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    List<JobApplication> result = apiInstance.listJobApplications(postingId, status, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#listJobApplications");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **postingId** | **UUID**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**List&lt;JobApplication&gt;**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPublicPostings

> List&lt;PublicPosting&gt; listPublicPostings()



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
try {
    List<PublicPosting> result = apiInstance.listPublicPostings();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#listPublicPostings");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PublicPosting&gt;**](PublicPosting.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## scoreJobApplication

> JobApplication scoreJobApplication(applicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID applicationId = null; // UUID | 
try {
    JobApplication result = apiInstance.scoreJobApplication(applicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#scoreJobApplication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | **UUID**|  | [default to null]

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateJobApplicationStatus

> JobApplication updateJobApplicationStatus(applicationId, applicationStatusDto)



### Example

```java
// Import classes:
//import org.openapitools.client.api.JobApplicationApi;

JobApplicationApi apiInstance = new JobApplicationApi();
UUID applicationId = null; // UUID | 
ApplicationStatusDto applicationStatusDto = new ApplicationStatusDto(); // ApplicationStatusDto | 
try {
    JobApplication result = apiInstance.updateJobApplicationStatus(applicationId, applicationStatusDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling JobApplicationApi#updateJobApplicationStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **applicationId** | **UUID**|  | [default to null]
 **applicationStatusDto** | [**ApplicationStatusDto**](ApplicationStatusDto.md)|  |

### Return type

[**JobApplication**](JobApplication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

