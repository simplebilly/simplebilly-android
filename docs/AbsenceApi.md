# AbsenceApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createAbsence**](AbsenceApi.md#createAbsence) | **POST** /api/v1/absences | 
[**deleteAbsence**](AbsenceApi.md#deleteAbsence) | **DELETE** /api/v1/absences/{id} | 
[**getAbsence**](AbsenceApi.md#getAbsence) | **GET** /api/v1/absences/{id} | 
[**getAbsences**](AbsenceApi.md#getAbsences) | **GET** /api/v1/absences/ | 
[**updateAbsence**](AbsenceApi.md#updateAbsence) | **PUT** /api/v1/absences/{id} | 



## createAbsence

> Absence createAbsence(absenceCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AbsenceApi;

AbsenceApi apiInstance = new AbsenceApi();
AbsenceCreate absenceCreate = new AbsenceCreate(); // AbsenceCreate | 
try {
    Absence result = apiInstance.createAbsence(absenceCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AbsenceApi#createAbsence");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **absenceCreate** | [**AbsenceCreate**](AbsenceCreate.md)|  |

### Return type

[**Absence**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteAbsence

> deleteAbsence(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AbsenceApi;

AbsenceApi apiInstance = new AbsenceApi();
UUID id = null; // UUID | 
try {
    apiInstance.deleteAbsence(id);
} catch (ApiException e) {
    System.err.println("Exception when calling AbsenceApi#deleteAbsence");
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


## getAbsence

> Absence getAbsence(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AbsenceApi;

AbsenceApi apiInstance = new AbsenceApi();
UUID id = null; // UUID | 
try {
    Absence result = apiInstance.getAbsence(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AbsenceApi#getAbsence");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**Absence**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getAbsences

> List&lt;Absence&gt; getAbsences(page, pageSize, search, includeDeleted)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AbsenceApi;

AbsenceApi apiInstance = new AbsenceApi();
Integer page = 1; // Integer | 
Integer pageSize = null; // Integer | 
String search = null; // String | 
Boolean includeDeleted = null; // Boolean | Soft-delete entities: set true to include rows with `deleted_at` set.
try {
    List<Absence> result = apiInstance.getAbsences(page, pageSize, search, includeDeleted);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AbsenceApi#getAbsences");
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

[**List&lt;Absence&gt;**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateAbsence

> Absence updateAbsence(id, absenceUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AbsenceApi;

AbsenceApi apiInstance = new AbsenceApi();
UUID id = null; // UUID | 
AbsenceUpdate absenceUpdate = new AbsenceUpdate(); // AbsenceUpdate | 
try {
    Absence result = apiInstance.updateAbsence(id, absenceUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AbsenceApi#updateAbsence");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **absenceUpdate** | [**AbsenceUpdate**](AbsenceUpdate.md)|  |

### Return type

[**Absence**](Absence.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

