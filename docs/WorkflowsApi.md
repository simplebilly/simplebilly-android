# WorkflowsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listWorkflowsApi**](WorkflowsApi.md#listWorkflowsApi) | **GET** /api/v1/workflows | 
[**setWorkflowEnabledApi**](WorkflowsApi.md#setWorkflowEnabledApi) | **PUT** /api/v1/workflows/{workflow_id}/enabled | 



## listWorkflowsApi

> List&lt;Workflow&gt; listWorkflowsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.WorkflowsApi;

WorkflowsApi apiInstance = new WorkflowsApi();
try {
    List<Workflow> result = apiInstance.listWorkflowsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WorkflowsApi#listWorkflowsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;Workflow&gt;**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## setWorkflowEnabledApi

> Workflow setWorkflowEnabledApi(workflowId, workflowEnabledUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.WorkflowsApi;

WorkflowsApi apiInstance = new WorkflowsApi();
String workflowId = null; // String | 
WorkflowEnabledUpdate workflowEnabledUpdate = new WorkflowEnabledUpdate(); // WorkflowEnabledUpdate | 
try {
    Workflow result = apiInstance.setWorkflowEnabledApi(workflowId, workflowEnabledUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling WorkflowsApi#setWorkflowEnabledApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **workflowId** | **String**|  | [default to null]
 **workflowEnabledUpdate** | [**WorkflowEnabledUpdate**](WorkflowEnabledUpdate.md)|  |

### Return type

[**Workflow**](Workflow.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

