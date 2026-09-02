# OnlineshopApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getSmtpConfigApi**](OnlineshopApi.md#getSmtpConfigApi) | **GET** /api/v1/settings/smtp | 
[**saveSmtpConfigApi**](OnlineshopApi.md#saveSmtpConfigApi) | **PUT** /api/v1/settings/smtp | 



## getSmtpConfigApi

> SmtpConfig getSmtpConfigApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.OnlineshopApi;

OnlineshopApi apiInstance = new OnlineshopApi();
try {
    SmtpConfig result = apiInstance.getSmtpConfigApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OnlineshopApi#getSmtpConfigApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## saveSmtpConfigApi

> SmtpConfig saveSmtpConfigApi(smtpConfig)



### Example

```java
// Import classes:
//import org.openapitools.client.api.OnlineshopApi;

OnlineshopApi apiInstance = new OnlineshopApi();
SmtpConfig smtpConfig = new SmtpConfig(); // SmtpConfig | 
try {
    SmtpConfig result = apiInstance.saveSmtpConfigApi(smtpConfig);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling OnlineshopApi#saveSmtpConfigApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **smtpConfig** | [**SmtpConfig**](SmtpConfig.md)|  | [optional]

### Return type

[**SmtpConfig**](SmtpConfig.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

