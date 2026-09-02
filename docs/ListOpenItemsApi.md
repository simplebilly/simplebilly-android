# ListOpenItemsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listOpenItemsApi**](ListOpenItemsApi.md#listOpenItemsApi) | **GET** /api/v1/bookkeeping/open-items | 



## listOpenItemsApi

> List&lt;OpenItem&gt; listOpenItemsApi(reminderLevel1Days, reminderLevel2Days, reminderLevel3Days, customerId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ListOpenItemsApi;

ListOpenItemsApi apiInstance = new ListOpenItemsApi();
Long reminderLevel1Days = null; // Long | 
Long reminderLevel2Days = null; // Long | 
Long reminderLevel3Days = null; // Long | 
String customerId = null; // String | 
try {
    List<OpenItem> result = apiInstance.listOpenItemsApi(reminderLevel1Days, reminderLevel2Days, reminderLevel3Days, customerId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ListOpenItemsApi#listOpenItemsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **reminderLevel1Days** | **Long**|  | [optional] [default to null]
 **reminderLevel2Days** | **Long**|  | [optional] [default to null]
 **reminderLevel3Days** | **Long**|  | [optional] [default to null]
 **customerId** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;OpenItem&gt;**](OpenItem.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

