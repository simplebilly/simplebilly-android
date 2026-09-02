# AutomationsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listAutomations**](AutomationsApi.md#listAutomations) | **GET** /api/v1/automations | 
[**triggerAutomation**](AutomationsApi.md#triggerAutomation) | **POST** /api/v1/automations/{key}/trigger | 
[**updateAutomation**](AutomationsApi.md#updateAutomation) | **PUT** /api/v1/automations/{key} | 



## listAutomations

> List&lt;AutomationDto&gt; listAutomations()



### Example

```java
// Import classes:
//import org.openapitools.client.api.AutomationsApi;

AutomationsApi apiInstance = new AutomationsApi();
try {
    List<AutomationDto> result = apiInstance.listAutomations();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AutomationsApi#listAutomations");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;AutomationDto&gt;**](AutomationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## triggerAutomation

> Object triggerAutomation(key)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AutomationsApi;

AutomationsApi apiInstance = new AutomationsApi();
String key = null; // String | 
try {
    Object result = apiInstance.triggerAutomation(key);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AutomationsApi#triggerAutomation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **String**|  | [default to null]

### Return type

**Object**

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateAutomation

> AutomationDto updateAutomation(key, updateAutomation)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AutomationsApi;

AutomationsApi apiInstance = new AutomationsApi();
String key = null; // String | 
UpdateAutomation updateAutomation = new UpdateAutomation(); // UpdateAutomation | 
try {
    AutomationDto result = apiInstance.updateAutomation(key, updateAutomation);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AutomationsApi#updateAutomation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **key** | **String**|  | [default to null]
 **updateAutomation** | [**UpdateAutomation**](UpdateAutomation.md)|  |

### Return type

[**AutomationDto**](AutomationDto.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

