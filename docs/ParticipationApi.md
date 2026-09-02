# ParticipationApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createParticipation**](ParticipationApi.md#createParticipation) | **POST** /api/v1/participations | 
[**deleteParticipation**](ParticipationApi.md#deleteParticipation) | **DELETE** /api/v1/participations/{id} | 
[**getParticipation**](ParticipationApi.md#getParticipation) | **GET** /api/v1/participations/{id} | 
[**getParticipations**](ParticipationApi.md#getParticipations) | **GET** /api/v1/participations/ | 
[**updateParticipation**](ParticipationApi.md#updateParticipation) | **PUT** /api/v1/participations/{id} | 



## createParticipation

> Participation createParticipation(participationCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ParticipationApi;

ParticipationApi apiInstance = new ParticipationApi();
ParticipationCreate participationCreate = new ParticipationCreate(); // ParticipationCreate | 
try {
    Participation result = apiInstance.createParticipation(participationCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParticipationApi#createParticipation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **participationCreate** | [**ParticipationCreate**](ParticipationCreate.md)|  |

### Return type

[**Participation**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteParticipation

> deleteParticipation(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ParticipationApi;

ParticipationApi apiInstance = new ParticipationApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteParticipation(id);
} catch (ApiException e) {
    System.err.println("Exception when calling ParticipationApi#deleteParticipation");
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


## getParticipation

> Participation getParticipation(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ParticipationApi;

ParticipationApi apiInstance = new ParticipationApi();
UUID id = null; // UUID | 
try {
    Participation result = apiInstance.getParticipation(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParticipationApi#getParticipation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Participation**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getParticipations

> List&lt;Participation&gt; getParticipations(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ParticipationApi;

ParticipationApi apiInstance = new ParticipationApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Participation> result = apiInstance.getParticipations(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParticipationApi#getParticipations");
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

[**List&lt;Participation&gt;**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateParticipation

> Participation updateParticipation(id, participationUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ParticipationApi;

ParticipationApi apiInstance = new ParticipationApi();
UUID id = null; // UUID | 
ParticipationUpdate participationUpdate = new ParticipationUpdate(); // ParticipationUpdate | 
try {
    Participation result = apiInstance.updateParticipation(id, participationUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ParticipationApi#updateParticipation");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **participationUpdate** | [**ParticipationUpdate**](ParticipationUpdate.md)|  |

### Return type

[**Participation**](Participation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

