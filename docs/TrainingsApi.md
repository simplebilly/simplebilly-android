# TrainingsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getMyTrainings**](TrainingsApi.md#getMyTrainings) | **GET** /api/v1/trainings/me | 
[**getTrainingContent**](TrainingsApi.md#getTrainingContent) | **GET** /api/v1/trainings/content/{code} | 
[**getTrainingOverview**](TrainingsApi.md#getTrainingOverview) | **GET** /api/v1/trainings/overview | 
[**submitTrainingResult**](TrainingsApi.md#submitTrainingResult) | **POST** /api/v1/trainings/submit-result | 



## getMyTrainings

> List&lt;MyTrainingItem&gt; getMyTrainings()



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingsApi;

TrainingsApi apiInstance = new TrainingsApi();
try {
    List<MyTrainingItem> result = apiInstance.getMyTrainings();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingsApi#getMyTrainings");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;MyTrainingItem&gt;**](MyTrainingItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTrainingContent

> TrainingContent getTrainingContent(code)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingsApi;

TrainingsApi apiInstance = new TrainingsApi();
String code = null; // String | Training code, e.g. data_privacy
try {
    TrainingContent result = apiInstance.getTrainingContent(code);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingsApi#getTrainingContent");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **code** | **String**| Training code, e.g. data_privacy | [default to null]

### Return type

[**TrainingContent**](TrainingContent.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getTrainingOverview

> List&lt;HrTrainingOverview&gt; getTrainingOverview()



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingsApi;

TrainingsApi apiInstance = new TrainingsApi();
try {
    List<HrTrainingOverview> result = apiInstance.getTrainingOverview();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingsApi#getTrainingOverview");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;HrTrainingOverview&gt;**](HrTrainingOverview.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## submitTrainingResult

> SubmitResultResponse submitTrainingResult(submitResultDto)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TrainingsApi;

TrainingsApi apiInstance = new TrainingsApi();
SubmitResultDto submitResultDto = new SubmitResultDto(); // SubmitResultDto | 
try {
    SubmitResultResponse result = apiInstance.submitTrainingResult(submitResultDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TrainingsApi#submitTrainingResult");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **submitResultDto** | [**SubmitResultDto**](SubmitResultDto.md)|  |

### Return type

[**SubmitResultResponse**](SubmitResultResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

