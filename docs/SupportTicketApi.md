# SupportTicketApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createTicketApi**](SupportTicketApi.md#createTicketApi) | **POST** /api/v1/support/tickets | 
[**deleteTicketApi**](SupportTicketApi.md#deleteTicketApi) | **DELETE** /api/v1/support/tickets/{ticket_id} | 
[**getTicketApi**](SupportTicketApi.md#getTicketApi) | **GET** /api/v1/support/tickets/{ticket_id} | 
[**listTicketsApi**](SupportTicketApi.md#listTicketsApi) | **GET** /api/v1/support/tickets | 
[**updateTicketApi**](SupportTicketApi.md#updateTicketApi) | **PUT** /api/v1/support/tickets/{ticket_id} | 



## createTicketApi

> SupportTicket createTicketApi(createTicketRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportTicketApi;

SupportTicketApi apiInstance = new SupportTicketApi();
CreateTicketRequest createTicketRequest = new CreateTicketRequest(); // CreateTicketRequest | 
try {
    SupportTicket result = apiInstance.createTicketApi(createTicketRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportTicketApi#createTicketApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **createTicketRequest** | [**CreateTicketRequest**](CreateTicketRequest.md)|  |

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteTicketApi

> deleteTicketApi(ticketId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportTicketApi;

SupportTicketApi apiInstance = new SupportTicketApi();
UUID ticketId = null; // UUID | 
try {
    apiInstance.deleteTicketApi(ticketId);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportTicketApi#deleteTicketApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticketId** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getTicketApi

> SupportTicket getTicketApi(ticketId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportTicketApi;

SupportTicketApi apiInstance = new SupportTicketApi();
UUID ticketId = null; // UUID | 
try {
    SupportTicket result = apiInstance.getTicketApi(ticketId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportTicketApi#getTicketApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticketId** | **UUID**|  | [default to null]

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listTicketsApi

> List&lt;SupportTicket&gt; listTicketsApi(status, priority, assignedTo, channelType, customerId, search, page, pageSize)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportTicketApi;

SupportTicketApi apiInstance = new SupportTicketApi();
String status = null; // String | 
String priority = null; // String | 
UUID assignedTo = null; // UUID | 
String channelType = null; // String | 
String customerId = null; // String | 
String search = null; // String | 
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
try {
    List<SupportTicket> result = apiInstance.listTicketsApi(status, priority, assignedTo, channelType, customerId, search, page, pageSize);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportTicketApi#listTicketsApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**|  | [optional] [default to null]
 **priority** | **String**|  | [optional] [default to null]
 **assignedTo** | **UUID**|  | [optional] [default to null]
 **channelType** | **String**|  | [optional] [default to null]
 **customerId** | **String**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]

### Return type

[**List&lt;SupportTicket&gt;**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateTicketApi

> SupportTicket updateTicketApi(ticketId, supportTicketUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.SupportTicketApi;

SupportTicketApi apiInstance = new SupportTicketApi();
UUID ticketId = null; // UUID | 
SupportTicketUpdate supportTicketUpdate = new SupportTicketUpdate(); // SupportTicketUpdate | 
try {
    SupportTicket result = apiInstance.updateTicketApi(ticketId, supportTicketUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling SupportTicketApi#updateTicketApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticketId** | **UUID**|  | [default to null]
 **supportTicketUpdate** | [**SupportTicketUpdate**](SupportTicketUpdate.md)|  |

### Return type

[**SupportTicket**](SupportTicket.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

