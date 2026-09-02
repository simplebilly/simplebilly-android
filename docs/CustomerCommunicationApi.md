# CustomerCommunicationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createCommunication**](CustomerCommunicationApi.md#createCommunication) | **POST** /api/v1/communications | 
[**customercommunicationRestore**](CustomerCommunicationApi.md#customercommunicationRestore) | **POST** /api/v1/communications/{communication_id}/restore | 
[**deleteCommunication**](CustomerCommunicationApi.md#deleteCommunication) | **DELETE** /api/v1/communications/{communication_id} | 
[**getCommunication**](CustomerCommunicationApi.md#getCommunication) | **GET** /api/v1/communications/{communication_id} | 
[**getContactHistory**](CustomerCommunicationApi.md#getContactHistory) | **GET** /api/v1/contacts/{contact_id}/communications | 
[**listCommunications**](CustomerCommunicationApi.md#listCommunications) | **GET** /api/v1/communications/ | 
[**updateCommunication**](CustomerCommunicationApi.md#updateCommunication) | **PUT** /api/v1/communications/{communication_id} | 



## createCommunication

> CustomerCommunication createCommunication(customerCommunicationCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
CustomerCommunicationCreate customerCommunicationCreate = new CustomerCommunicationCreate(); // CustomerCommunicationCreate | 
try {
    CustomerCommunication result = apiInstance.createCommunication(customerCommunicationCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#createCommunication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerCommunicationCreate** | [**CustomerCommunicationCreate**](CustomerCommunicationCreate.md)|  |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## customercommunicationRestore

> CustomerCommunication customercommunicationRestore(communicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
String communicationId = null; // String | 
try {
    CustomerCommunication result = apiInstance.customercommunicationRestore(communicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#customercommunicationRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communicationId** | **String**|  | [default to null]

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## deleteCommunication

> deleteCommunication(communicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
String communicationId = null; // String | 
try {
    apiInstance.deleteCommunication(communicationId);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#deleteCommunication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communicationId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCommunication

> CustomerCommunication getCommunication(communicationId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
String communicationId = null; // String | 
try {
    CustomerCommunication result = apiInstance.getCommunication(communicationId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#getCommunication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communicationId** | **String**|  | [default to null]

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getContactHistory

> ContactHistoryResponse getContactHistory(contactId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
String contactId = null; // String | 
try {
    ContactHistoryResponse result = apiInstance.getContactHistory(contactId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#getContactHistory");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contactId** | **String**|  | [default to null]

### Return type

[**ContactHistoryResponse**](ContactHistoryResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listCommunications

> List&lt;CustomerCommunication&gt; listCommunications(page, pageSize, contactId, channel, direction, from, to)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String contactId = null; // String | Filter history to a single contact.
CommunicationChannel channel = null; // CommunicationChannel | 
CommunicationDirection direction = null; // CommunicationDirection | 
Date from = null; // Date | Only include communications after this ISO date (inclusive).
Date to = null; // Date | Only include communications before this ISO date (inclusive).
try {
    List<CustomerCommunication> result = apiInstance.listCommunications(page, pageSize, contactId, channel, direction, from, to);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#listCommunications");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **contactId** | **String**| Filter history to a single contact. | [optional] [default to null]
 **channel** | [**CommunicationChannel**](.md)|  | [optional] [default to null] [enum: email, call, meeting, chat, note]
 **direction** | [**CommunicationDirection**](.md)|  | [optional] [default to null] [enum: inbound, outbound]
 **from** | **Date**| Only include communications after this ISO date (inclusive). | [optional] [default to null]
 **to** | **Date**| Only include communications before this ISO date (inclusive). | [optional] [default to null]

### Return type

[**List&lt;CustomerCommunication&gt;**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCommunication

> CustomerCommunication updateCommunication(communicationId, customerCommunicationUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CustomerCommunicationApi;

CustomerCommunicationApi apiInstance = new CustomerCommunicationApi();
String communicationId = null; // String | 
CustomerCommunicationUpdate customerCommunicationUpdate = new CustomerCommunicationUpdate(); // CustomerCommunicationUpdate | 
try {
    CustomerCommunication result = apiInstance.updateCommunication(communicationId, customerCommunicationUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CustomerCommunicationApi#updateCommunication");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **communicationId** | **String**|  | [default to null]
 **customerCommunicationUpdate** | [**CustomerCommunicationUpdate**](CustomerCommunicationUpdate.md)|  |

### Return type

[**CustomerCommunication**](CustomerCommunication.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

