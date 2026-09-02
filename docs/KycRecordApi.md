# KycRecordApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createKycRecord**](KycRecordApi.md#createKycRecord) | **POST** /api/v1/kyc-records | 
[**deleteKycRecord**](KycRecordApi.md#deleteKycRecord) | **DELETE** /api/v1/kyc-records/{id} | 
[**getKycRecord**](KycRecordApi.md#getKycRecord) | **GET** /api/v1/kyc-records/{id} | 
[**getKycRecords**](KycRecordApi.md#getKycRecords) | **GET** /api/v1/kyc-records/ | 
[**updateKycRecord**](KycRecordApi.md#updateKycRecord) | **PUT** /api/v1/kyc-records/{id} | 



## createKycRecord

> KycRecord createKycRecord(kycRecordCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KycRecordApi;

KycRecordApi apiInstance = new KycRecordApi();
KycRecordCreate kycRecordCreate = new KycRecordCreate(); // KycRecordCreate | 
try {
    KycRecord result = apiInstance.createKycRecord(kycRecordCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KycRecordApi#createKycRecord");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **kycRecordCreate** | [**KycRecordCreate**](KycRecordCreate.md)|  |

### Return type

[**KycRecord**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteKycRecord

> deleteKycRecord(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KycRecordApi;

KycRecordApi apiInstance = new KycRecordApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteKycRecord(id);
} catch (ApiException e) {
    System.err.println("Exception when calling KycRecordApi#deleteKycRecord");
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


## getKycRecord

> KycRecord getKycRecord(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KycRecordApi;

KycRecordApi apiInstance = new KycRecordApi();
UUID id = null; // UUID | 
try {
    KycRecord result = apiInstance.getKycRecord(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KycRecordApi#getKycRecord");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**KycRecord**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getKycRecords

> List&lt;KycRecord&gt; getKycRecords(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KycRecordApi;

KycRecordApi apiInstance = new KycRecordApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<KycRecord> result = apiInstance.getKycRecords(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KycRecordApi#getKycRecords");
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

[**List&lt;KycRecord&gt;**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateKycRecord

> KycRecord updateKycRecord(id, kycRecordUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.KycRecordApi;

KycRecordApi apiInstance = new KycRecordApi();
UUID id = null; // UUID | 
KycRecordUpdate kycRecordUpdate = new KycRecordUpdate(); // KycRecordUpdate | 
try {
    KycRecord result = apiInstance.updateKycRecord(id, kycRecordUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling KycRecordApi#updateKycRecord");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **kycRecordUpdate** | [**KycRecordUpdate**](KycRecordUpdate.md)|  |

### Return type

[**KycRecord**](KycRecord.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

