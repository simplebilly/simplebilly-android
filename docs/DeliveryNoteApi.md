# DeliveryNoteApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeliveryNote**](DeliveryNoteApi.md#createDeliveryNote) | **POST** /api/v1/delivery-notes | 
[**deleteDeliveryNote**](DeliveryNoteApi.md#deleteDeliveryNote) | **DELETE** /api/v1/delivery-notes/{delivery_note_id} | 
[**deliverynoteRestore**](DeliveryNoteApi.md#deliverynoteRestore) | **POST** /api/v1/delivery-notes/{delivery_note_id}/restore | 
[**downloadDeliveryNotePdf**](DeliveryNoteApi.md#downloadDeliveryNotePdf) | **GET** /api/v1/delivery-notes/{delivery_note_id}/pdf | 
[**getDeliveryNote**](DeliveryNoteApi.md#getDeliveryNote) | **GET** /api/v1/delivery-notes/{delivery_note_id} | 
[**listDeliveryNotes**](DeliveryNoteApi.md#listDeliveryNotes) | **GET** /api/v1/delivery-notes/ | 
[**pursueDeliveryNote**](DeliveryNoteApi.md#pursueDeliveryNote) | **POST** /api/v1/delivery-notes/{delivery_note_id}/pursue | 



## createDeliveryNote

> DeliveryNote createDeliveryNote(deliveryNoteCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
DeliveryNoteCreate deliveryNoteCreate = new DeliveryNoteCreate(); // DeliveryNoteCreate | 
try {
    DeliveryNote result = apiInstance.createDeliveryNote(deliveryNoteCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#createDeliveryNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryNoteCreate** | [**DeliveryNoteCreate**](DeliveryNoteCreate.md)|  |

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteDeliveryNote

> deleteDeliveryNote(deliveryNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
String deliveryNoteId = null; // String | 
try {
    apiInstance.deleteDeliveryNote(deliveryNoteId);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#deleteDeliveryNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryNoteId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## deliverynoteRestore

> DeliveryNote deliverynoteRestore(deliveryNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
String deliveryNoteId = null; // String | 
try {
    DeliveryNote result = apiInstance.deliverynoteRestore(deliveryNoteId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#deliverynoteRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryNoteId** | **String**|  | [default to null]

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## downloadDeliveryNotePdf

> downloadDeliveryNotePdf(deliveryNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
String deliveryNoteId = null; // String | 
try {
    apiInstance.downloadDeliveryNotePdf(deliveryNoteId);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#downloadDeliveryNotePdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryNoteId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf, application/json


## getDeliveryNote

> DeliveryNote getDeliveryNote(deliveryNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
String deliveryNoteId = null; // String | 
try {
    DeliveryNote result = apiInstance.getDeliveryNote(deliveryNoteId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#getDeliveryNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryNoteId** | **String**|  | [default to null]

### Return type

[**DeliveryNote**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDeliveryNotes

> List&lt;DeliveryNote&gt; listDeliveryNotes(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<DeliveryNote> result = apiInstance.listDeliveryNotes(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#listDeliveryNotes");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **search** | **String**|  | [optional] [default to null]
 **includeDeleted** | **Boolean**| Soft-delete entities: set true to include rows with &#x60;deleted_at&#x60; set. | [optional] [default to null]

### Return type

[**List&lt;DeliveryNote&gt;**](DeliveryNote.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## pursueDeliveryNote

> Invoice pursueDeliveryNote(deliveryNoteId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryNoteApi;

DeliveryNoteApi apiInstance = new DeliveryNoteApi();
String deliveryNoteId = null; // String | 
try {
    Invoice result = apiInstance.pursueDeliveryNote(deliveryNoteId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryNoteApi#pursueDeliveryNote");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryNoteId** | **String**|  | [default to null]

### Return type

[**Invoice**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

