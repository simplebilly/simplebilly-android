# TicketMessageApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listMessagesApi**](TicketMessageApi.md#listMessagesApi) | **GET** /api/v1/support/tickets/{ticket_id}/messages | 
[**sendMessageApi**](TicketMessageApi.md#sendMessageApi) | **POST** /api/v1/support/tickets/{ticket_id}/messages | 



## listMessagesApi

> List&lt;TicketMessage&gt; listMessagesApi(ticketId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TicketMessageApi;

TicketMessageApi apiInstance = new TicketMessageApi();
UUID ticketId = null; // UUID | 
try {
    List<TicketMessage> result = apiInstance.listMessagesApi(ticketId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TicketMessageApi#listMessagesApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticketId** | **UUID**|  | [default to null]

### Return type

[**List&lt;TicketMessage&gt;**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## sendMessageApi

> TicketMessage sendMessageApi(ticketId, sendMessageDto)



### Example

```java
// Import classes:
//import org.openapitools.client.api.TicketMessageApi;

TicketMessageApi apiInstance = new TicketMessageApi();
UUID ticketId = null; // UUID | 
SendMessageDto sendMessageDto = new SendMessageDto(); // SendMessageDto | 
try {
    TicketMessage result = apiInstance.sendMessageApi(ticketId, sendMessageDto);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling TicketMessageApi#sendMessageApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ticketId** | **UUID**|  | [default to null]
 **sendMessageDto** | [**SendMessageDto**](SendMessageDto.md)|  |

### Return type

[**TicketMessage**](TicketMessage.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

