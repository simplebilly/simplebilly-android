# AttachmentVersionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAttachmentVersion**](AttachmentVersionApi.md#createAttachmentVersion) | **POST** /api/v1/attachments/{attachment_id}/versions | 
[**listAttachmentVersions**](AttachmentVersionApi.md#listAttachmentVersions) | **GET** /api/v1/attachments/{attachment_id}/versions | 
[**restoreAttachmentVersion**](AttachmentVersionApi.md#restoreAttachmentVersion) | **POST** /api/v1/attachments/{attachment_id}/versions/{version_id}/restore | 



## createAttachmentVersion

> AttachmentVersion createAttachmentVersion(attachmentId, newVersionRequest)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentVersionApi;

AttachmentVersionApi apiInstance = new AttachmentVersionApi();
UUID attachmentId = null; // UUID | 
NewVersionRequest newVersionRequest = new NewVersionRequest(); // NewVersionRequest | 
try {
    AttachmentVersion result = apiInstance.createAttachmentVersion(attachmentId, newVersionRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentVersionApi#createAttachmentVersion");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachmentId** | **UUID**|  | [default to null]
 **newVersionRequest** | [**NewVersionRequest**](NewVersionRequest.md)|  |

### Return type

[**AttachmentVersion**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## listAttachmentVersions

> List&lt;AttachmentVersion&gt; listAttachmentVersions(attachmentId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentVersionApi;

AttachmentVersionApi apiInstance = new AttachmentVersionApi();
UUID attachmentId = null; // UUID | 
try {
    List<AttachmentVersion> result = apiInstance.listAttachmentVersions(attachmentId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentVersionApi#listAttachmentVersions");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachmentId** | **UUID**|  | [default to null]

### Return type

[**List&lt;AttachmentVersion&gt;**](AttachmentVersion.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## restoreAttachmentVersion

> Attachment restoreAttachmentVersion(attachmentId, versionId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AttachmentVersionApi;

AttachmentVersionApi apiInstance = new AttachmentVersionApi();
UUID attachmentId = null; // UUID | 
UUID versionId = null; // UUID | 
try {
    Attachment result = apiInstance.restoreAttachmentVersion(attachmentId, versionId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AttachmentVersionApi#restoreAttachmentVersion");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **attachmentId** | **UUID**|  | [default to null]
 **versionId** | **UUID**|  | [default to null]

### Return type

[**Attachment**](Attachment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

