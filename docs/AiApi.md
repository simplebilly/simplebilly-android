# AiApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**aiSuggestApi**](AiApi.md#aiSuggestApi) | **POST** /api/v1/support/ai/suggest | 
[**createWorkerApi**](AiApi.md#createWorkerApi) | **POST** /api/v1/support/ai/workers | 
[**listWorkersApi**](AiApi.md#listWorkersApi) | **GET** /api/v1/support/ai/workers | 
[**runWorkerApi**](AiApi.md#runWorkerApi) | **POST** /api/v1/support/ai/workers/{worker_id}/run | 



## aiSuggestApi

> AiSuggestion aiSuggestApi(aiSuggestionRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AiApi;

AiApi apiInstance = new AiApi();
AiSuggestionRequest aiSuggestionRequest = new AiSuggestionRequest(); // AiSuggestionRequest | 
try {
    AiSuggestion result = apiInstance.aiSuggestApi(aiSuggestionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AiApi#aiSuggestApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aiSuggestionRequest** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  |

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## createWorkerApi

> AiWorkerConfig createWorkerApi(aiConfigDto)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AiApi;

AiApi apiInstance = new AiApi();
AiConfigDto aiConfigDto = new AiConfigDto(); // AiConfigDto | 
try {
    AiWorkerConfig result = apiInstance.createWorkerApi(aiConfigDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AiApi#createWorkerApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **aiConfigDto** | [**AiConfigDto**](AiConfigDto.md)|  |

### Return type

[**AiWorkerConfig**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listWorkersApi

> List&lt;AiWorkerConfig&gt; listWorkersApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.AiApi;

AiApi apiInstance = new AiApi();
try {
    List<AiWorkerConfig> result = apiInstance.listWorkersApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AiApi#listWorkersApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;AiWorkerConfig&gt;**](AiWorkerConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## runWorkerApi

> AiSuggestion runWorkerApi(workerId, aiSuggestionRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AiApi;

AiApi apiInstance = new AiApi();
UUID workerId = null; // UUID | 
AiSuggestionRequest aiSuggestionRequest = new AiSuggestionRequest(); // AiSuggestionRequest | 
try {
    AiSuggestion result = apiInstance.runWorkerApi(workerId, aiSuggestionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AiApi#runWorkerApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workerId** | **UUID**|  | [default to null]
 **aiSuggestionRequest** | [**AiSuggestionRequest**](AiSuggestionRequest.md)|  |

### Return type

[**AiSuggestion**](AiSuggestion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

