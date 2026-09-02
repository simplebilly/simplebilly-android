# RecurringTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createRecurringTemplate**](RecurringTemplateApi.md#createRecurringTemplate) | **POST** /api/v1/recurring-templates | 
[**deleteRecurringTemplate**](RecurringTemplateApi.md#deleteRecurringTemplate) | **DELETE** /api/v1/recurring-templates/{template_id} | 
[**getRecurringTemplate**](RecurringTemplateApi.md#getRecurringTemplate) | **GET** /api/v1/recurring-templates/{template_id} | 
[**listRecurringTemplates**](RecurringTemplateApi.md#listRecurringTemplates) | **GET** /api/v1/recurring-templates/ | 



## createRecurringTemplate

> RecurringTemplate createRecurringTemplate(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RecurringTemplateApi;

RecurringTemplateApi apiInstance = new RecurringTemplateApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    RecurringTemplate result = apiInstance.createRecurringTemplate(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RecurringTemplateApi#createRecurringTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**RecurringTemplate**](RecurringTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteRecurringTemplate

> deleteRecurringTemplate(templateId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RecurringTemplateApi;

RecurringTemplateApi apiInstance = new RecurringTemplateApi();
String templateId = null; // String | 
try {
    apiInstance.deleteRecurringTemplate(templateId);
} catch (ApiException e) {
    System.err.println("Exception when calling RecurringTemplateApi#deleteRecurringTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **templateId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getRecurringTemplate

> RecurringTemplate getRecurringTemplate(templateId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RecurringTemplateApi;

RecurringTemplateApi apiInstance = new RecurringTemplateApi();
String templateId = null; // String | 
try {
    RecurringTemplate result = apiInstance.getRecurringTemplate(templateId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RecurringTemplateApi#getRecurringTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **templateId** | **String**|  | [default to null]

### Return type

[**RecurringTemplate**](RecurringTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listRecurringTemplates

> List&lt;RecurringTemplate&gt; listRecurringTemplates()



### Example

```java
// Import classes:
//import org.openapitools.client.api.RecurringTemplateApi;

RecurringTemplateApi apiInstance = new RecurringTemplateApi();
try {
    List<RecurringTemplate> result = apiInstance.listRecurringTemplates();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RecurringTemplateApi#listRecurringTemplates");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;RecurringTemplate&gt;**](RecurringTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

