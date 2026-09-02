# EmailTemplateApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createEmailTemplate**](EmailTemplateApi.md#createEmailTemplate) | **POST** /api/v1/email-templates | 
[**deleteEmailTemplate**](EmailTemplateApi.md#deleteEmailTemplate) | **DELETE** /api/v1/email-templates/{email_template_id} | 
[**getEmailTemplate**](EmailTemplateApi.md#getEmailTemplate) | **GET** /api/v1/email-templates/{email_template_id} | 
[**listEmailTemplates**](EmailTemplateApi.md#listEmailTemplates) | **GET** /api/v1/email-templates/ | 
[**renderEmailTemplate**](EmailTemplateApi.md#renderEmailTemplate) | **POST** /api/v1/email-templates/{email_template_id}/render | 
[**updateEmailTemplate**](EmailTemplateApi.md#updateEmailTemplate) | **PUT** /api/v1/email-templates/{email_template_id} | 



## createEmailTemplate

> EmailTemplate createEmailTemplate(emailTemplateCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmailTemplateApi;

EmailTemplateApi apiInstance = new EmailTemplateApi();
EmailTemplateCreate emailTemplateCreate = new EmailTemplateCreate(); // EmailTemplateCreate | 
try {
    EmailTemplate result = apiInstance.createEmailTemplate(emailTemplateCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmailTemplateApi#createEmailTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailTemplateCreate** | [**EmailTemplateCreate**](EmailTemplateCreate.md)|  |

### Return type

[**EmailTemplate**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteEmailTemplate

> deleteEmailTemplate(emailTemplateId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmailTemplateApi;

EmailTemplateApi apiInstance = new EmailTemplateApi();
String emailTemplateId = null; // String | 
try {
    apiInstance.deleteEmailTemplate(emailTemplateId);
} catch (ApiException e) {
    System.err.println("Exception when calling EmailTemplateApi#deleteEmailTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailTemplateId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getEmailTemplate

> EmailTemplate getEmailTemplate(emailTemplateId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmailTemplateApi;

EmailTemplateApi apiInstance = new EmailTemplateApi();
String emailTemplateId = null; // String | 
try {
    EmailTemplate result = apiInstance.getEmailTemplate(emailTemplateId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmailTemplateApi#getEmailTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailTemplateId** | **String**|  | [default to null]

### Return type

[**EmailTemplate**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listEmailTemplates

> List&lt;EmailTemplate&gt; listEmailTemplates(page, pageSize, status, search)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmailTemplateApi;

EmailTemplateApi apiInstance = new EmailTemplateApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String search = null; // String | 
try {
    List<EmailTemplate> result = apiInstance.listEmailTemplates(page, pageSize, status, search);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmailTemplateApi#listEmailTemplates");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;EmailTemplate&gt;**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## renderEmailTemplate

> OasAnyTypeNotMapped renderEmailTemplate(emailTemplateId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmailTemplateApi;

EmailTemplateApi apiInstance = new EmailTemplateApi();
String emailTemplateId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.renderEmailTemplate(emailTemplateId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmailTemplateApi#renderEmailTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailTemplateId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateEmailTemplate

> EmailTemplate updateEmailTemplate(emailTemplateId, emailTemplateUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.EmailTemplateApi;

EmailTemplateApi apiInstance = new EmailTemplateApi();
String emailTemplateId = null; // String | 
EmailTemplateUpdate emailTemplateUpdate = new EmailTemplateUpdate(); // EmailTemplateUpdate | 
try {
    EmailTemplate result = apiInstance.updateEmailTemplate(emailTemplateId, emailTemplateUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling EmailTemplateApi#updateEmailTemplate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **emailTemplateId** | **String**|  | [default to null]
 **emailTemplateUpdate** | [**EmailTemplateUpdate**](EmailTemplateUpdate.md)|  |

### Return type

[**EmailTemplate**](EmailTemplate.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

