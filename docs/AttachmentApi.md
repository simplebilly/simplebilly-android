# AttachmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**attachmentRestore**](AttachmentApi.md#attachmentRestore) | **POST** /api/v1/attachments/{id}/restore | 
[**createAttachment**](AttachmentApi.md#createAttachment) | **POST** /api/v1/attachments | 
[**deleteAttachment**](AttachmentApi.md#deleteAttachment) | **DELETE** /api/v1/attachments/{id} | 
[**getAttachment**](AttachmentApi.md#getAttachment) | **GET** /api/v1/attachments/{id} | 
[**listAttachments**](AttachmentApi.md#listAttachments) | **GET** /api/v1/attachments/ | 
[**saveAttachmentOcrText**](AttachmentApi.md#saveAttachmentOcrText) | **PUT** /api/v1/attachments/{attachment_id}/ocr-text | Persist client-side OCR output for an attachment.



## attachmentRestore

> Attachment attachmentRestore(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentApi;

AttachmentApi apiInstance = new AttachmentApi();
UUID id = null; // UUID | 
try {
    Attachment result = apiInstance.attachmentRestore(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentApi#attachmentRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## createAttachment

> Attachment createAttachment(attachmentCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentApi;

AttachmentApi apiInstance = new AttachmentApi();
AttachmentCreate attachmentCreate = new AttachmentCreate(); // AttachmentCreate | 
try {
    Attachment result = apiInstance.createAttachment(attachmentCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentApi#createAttachment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachmentCreate** | [**AttachmentCreate**](AttachmentCreate.md)|  |

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteAttachment

> deleteAttachment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentApi;

AttachmentApi apiInstance = new AttachmentApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteAttachment(id);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentApi#deleteAttachment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAttachment

> Attachment getAttachment(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentApi;

AttachmentApi apiInstance = new AttachmentApi();
UUID id = null; // UUID | 
try {
    Attachment result = apiInstance.getAttachment(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentApi#getAttachment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listAttachments

> List&lt;Attachment&gt; listAttachments(page, pageSize, contactId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentApi;

AttachmentApi apiInstance = new AttachmentApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String contactId = null; // String | 
try {
    List<Attachment> result = apiInstance.listAttachments(page, pageSize, contactId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentApi#listAttachments");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **contactId** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;Attachment&gt;**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## saveAttachmentOcrText

> Attachment saveAttachmentOcrText(attachmentId, ocrTextRequest)

Persist client-side OCR output for an attachment.

### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentApi;

AttachmentApi apiInstance = new AttachmentApi();
UUID attachmentId = null; // UUID | 
OcrTextRequest ocrTextRequest = new OcrTextRequest(); // OcrTextRequest | 
try {
    Attachment result = apiInstance.saveAttachmentOcrText(attachmentId, ocrTextRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentApi#saveAttachmentOcrText");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachmentId** | **UUID**|  | [default to null]
 **ocrTextRequest** | [**OcrTextRequest**](OcrTextRequest.md)|  |

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

