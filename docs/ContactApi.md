# ContactApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**contactSchema**](ContactApi.md#contactSchema) | **GET** /api/v1/contacts/schema | Serve JSON Schema for client-side validation
[**contactTimeline**](ContactApi.md#contactTimeline) | **GET** /api/v1/contacts/{contact_id}/timeline | Get the full per-contact timeline (Xentral §4.6/4.7).
[**createContact**](ContactApi.md#createContact) | **POST** /api/v1/contacts | Create contact
[**deleteContact**](ContactApi.md#deleteContact) | **DELETE** /api/v1/contacts/{contact_id} | Soft-delete contact
[**getContact**](ContactApi.md#getContact) | **GET** /api/v1/contacts/{contact_id} | Get single contact
[**listContacts**](ContactApi.md#listContacts) | **GET** /api/v1/contacts | List contacts with search, type filter, and pagination
[**salesVolume**](ContactApi.md#salesVolume) | **GET** /api/v1/contacts/sales-volume | Sales volume per contact
[**updateContact**](ContactApi.md#updateContact) | **PUT** /api/v1/contacts/{contact_id} | Update contact



## contactSchema

> OasAnyTypeNotMapped contactSchema()

Serve JSON Schema for client-side validation

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
try {
    OasAnyTypeNotMapped result = apiInstance.contactSchema();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#contactSchema");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## contactTimeline

> ContactTimelineResponse contactTimeline(contactId)

Get the full per-contact timeline (Xentral §4.6/4.7).

Aggregates communications, quotations, orders, invoices and uploaded documents for a contact, merged into a single reverse-chronological feed.

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
String contactId = null; // String | 
try {
    ContactTimelineResponse result = apiInstance.contactTimeline(contactId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#contactTimeline");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contactId** | **String**|  | [default to null]

### Return type

[**ContactTimelineResponse**](ContactTimelineResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## createContact

> Contact createContact(body)

Create contact

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Contact result = apiInstance.createContact(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#createContact");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Contact**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteContact

> deleteContact(contactId)

Soft-delete contact

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
String contactId = null; // String | 
try {
    apiInstance.deleteContact(contactId);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#deleteContact");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contactId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getContact

> Contact getContact(contactId)

Get single contact

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
String contactId = null; // String | 
try {
    Contact result = apiInstance.getContact(contactId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#getContact");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contactId** | **String**|  | [default to null]

### Return type

[**Contact**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listContacts

> List&lt;Contact&gt; listContacts(page, pageSize, search, contactType, tag)

List contacts with search, type filter, and pagination

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
String contactType = null; // String | 
String tag = null; // String | 
try {
    List<Contact> result = apiInstance.listContacts(page, pageSize, search, contactType, tag);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#listContacts");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **contactType** | **String**|  | [optional] [default to null]
 **tag** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;Contact&gt;**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## salesVolume

> SalesVolumeReport salesVolume(page, pageSize, search, contactType, tag)

Sales volume per contact

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
String contactType = null; // String | 
String tag = null; // String | 
try {
    SalesVolumeReport result = apiInstance.salesVolume(page, pageSize, search, contactType, tag);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#salesVolume");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **contactType** | **String**|  | [optional] [default to null]
 **tag** | **String**|  | [optional] [default to null]

### Return type

[**SalesVolumeReport**](SalesVolumeReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateContact

> Contact updateContact(contactId, body)

Update contact

### Example

```java
// Import classes:
//import org.openapitools.client.api.ContactApi;

ContactApi apiInstance = new ContactApi();
String contactId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Contact result = apiInstance.updateContact(contactId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ContactApi#updateContact");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **contactId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Contact**](Contact.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

