# ProposeAssignmentsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**proposeAssignmentsApi**](ProposeAssignmentsApi.md#proposeAssignmentsApi) | **GET** /api/v1/bookkeeping/propose-assignments | 



## proposeAssignmentsApi

> List&lt;ProposedAssignment&gt; proposeAssignmentsApi(minConfidence, customerId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ProposeAssignmentsApi;

ProposeAssignmentsApi apiInstance = new ProposeAssignmentsApi();
Double minConfidence = null; // Double | 
String customerId = null; // String | 
try {
    List<ProposedAssignment> result = apiInstance.proposeAssignmentsApi(minConfidence, customerId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ProposeAssignmentsApi#proposeAssignmentsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **minConfidence** | **Double**|  | [optional] [default to null]
 **customerId** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;ProposedAssignment&gt;**](ProposedAssignment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

