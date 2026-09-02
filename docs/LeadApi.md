# LeadApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listLeadsApi**](LeadApi.md#listLeadsApi) | **GET** /api/v1/support/leads | 
[**updateLeadApi**](LeadApi.md#updateLeadApi) | **PUT** /api/v1/support/leads/{lead_id} | 



## listLeadsApi

> List&lt;Lead&gt; listLeadsApi(status, source, search, page, pageSize)



### Example

```java
// Import classes:
//import org.openapitools.client.api.LeadApi;

LeadApi apiInstance = new LeadApi();
String status = null; // String | 
String source = null; // String | 
String search = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    List<Lead> result = apiInstance.listLeadsApi(status, source, search, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LeadApi#listLeadsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**|  | [optional] [default to null]
 **source** | **String**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**List&lt;Lead&gt;**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateLeadApi

> Lead updateLeadApi(leadId, leadUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.LeadApi;

LeadApi apiInstance = new LeadApi();
UUID leadId = null; // UUID | 
LeadUpdate leadUpdate = new LeadUpdate(); // LeadUpdate | 
try {
    Lead result = apiInstance.updateLeadApi(leadId, leadUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling LeadApi#updateLeadApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **leadId** | **UUID**|  | [default to null]
 **leadUpdate** | [**LeadUpdate**](LeadUpdate.md)|  |

### Return type

[**Lead**](Lead.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

