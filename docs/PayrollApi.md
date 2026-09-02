# PayrollApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**payrollApprove**](PayrollApi.md#payrollApprove) | **POST** /api/v1/payroll/{id}/approve | 
[**payrollAutopay**](PayrollApi.md#payrollAutopay) | **POST** /api/v1/payroll/{id}/autopay | 
[**payrollCalculate**](PayrollApi.md#payrollCalculate) | **POST** /api/v1/payroll/{id}/calculate | 
[**payrollCreate**](PayrollApi.md#payrollCreate) | **POST** /api/v1/payroll | 
[**payrollDelete**](PayrollApi.md#payrollDelete) | **DELETE** /api/v1/payroll/{id} | 
[**payrollElsterExport**](PayrollApi.md#payrollElsterExport) | **POST** /api/v1/payroll/{id}/elster-export | 
[**payrollEmail**](PayrollApi.md#payrollEmail) | **POST** /api/v1/payroll/{id}/email | 
[**payrollEntryPdf**](PayrollApi.md#payrollEntryPdf) | **GET** /api/v1/payroll/{id}/entries/{entry_id}/pdf | 
[**payrollGet**](PayrollApi.md#payrollGet) | **GET** /api/v1/payroll/{id} | 
[**payrollList**](PayrollApi.md#payrollList) | **GET** /api/v1/payroll | 
[**payrollPay**](PayrollApi.md#payrollPay) | **POST** /api/v1/payroll/{id}/pay | 
[**payrollPdf**](PayrollApi.md#payrollPdf) | **GET** /api/v1/payroll/{id}/pdf | 
[**payrollSummary**](PayrollApi.md#payrollSummary) | **GET** /api/v1/payroll/summary/{year} | 
[**payrollSvMeldungen**](PayrollApi.md#payrollSvMeldungen) | **POST** /api/v1/payroll/{id}/sv-meldungen | 



## payrollApprove

> PayrollRunApi payrollApprove(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
try {
    PayrollRunApi result = apiInstance.payrollApprove(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollApprove");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payrollAutopay

> OasAnyTypeNotMapped payrollAutopay(id, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
String id = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.payrollAutopay(id, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollAutopay");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  | [optional]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## payrollCalculate

> PayrollRunApi payrollCalculate(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
try {
    PayrollRunApi result = apiInstance.payrollCalculate(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollCalculate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payrollCreate

> PayrollRunApi payrollCreate(payrollCreatePayload)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
PayrollCreatePayload payrollCreatePayload = new PayrollCreatePayload(); // PayrollCreatePayload | 
try {
    PayrollRunApi result = apiInstance.payrollCreate(payrollCreatePayload);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollCreate");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **payrollCreatePayload** | [**PayrollCreatePayload**](PayrollCreatePayload.md)|  |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## payrollDelete

> payrollDelete(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
try {
    apiInstance.payrollDelete(id);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollDelete");
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
- **Accept**: Not defined


## payrollElsterExport

> payrollElsterExport(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
try {
    apiInstance.payrollElsterExport(id);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollElsterExport");
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
- **Accept**: Not defined


## payrollEmail

> OasAnyTypeNotMapped payrollEmail(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
String id = null; // String | 
try {
    OasAnyTypeNotMapped result = apiInstance.payrollEmail(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollEmail");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payrollEntryPdf

> payrollEntryPdf(id, entryId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
String id = null; // String | 
String entryId = null; // String | 
try {
    apiInstance.payrollEntryPdf(id, entryId);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollEntryPdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]
 **entryId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf


## payrollGet

> PayrollRunApi payrollGet(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
try {
    PayrollRunApi result = apiInstance.payrollGet(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollGet");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payrollList

> List&lt;PayrollRunApi&gt; payrollList(year, status)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
Integer year = null; // Integer | 
String status = null; // String | 
try {
    List<PayrollRunApi> result = apiInstance.payrollList(year, status);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollList");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;PayrollRunApi&gt;**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payrollPay

> PayrollRunApi payrollPay(id, payrollPayPayload)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
PayrollPayPayload payrollPayPayload = new PayrollPayPayload(); // PayrollPayPayload | 
try {
    PayrollRunApi result = apiInstance.payrollPay(id, payrollPayPayload);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollPay");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]
 **payrollPayPayload** | [**PayrollPayPayload**](PayrollPayPayload.md)|  |

### Return type

[**PayrollRunApi**](PayrollRunApi.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## payrollPdf

> payrollPdf(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
String id = null; // String | 
try {
    apiInstance.payrollPdf(id);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollPdf");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/pdf


## payrollSummary

> YearlyPayrollSummary payrollSummary(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
Integer year = null; // Integer | 
try {
    YearlyPayrollSummary result = apiInstance.payrollSummary(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollSummary");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**YearlyPayrollSummary**](YearlyPayrollSummary.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## payrollSvMeldungen

> OasAnyTypeNotMapped payrollSvMeldungen(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PayrollApi;

PayrollApi apiInstance = new PayrollApi();
UUID id = null; // UUID | 
try {
    OasAnyTypeNotMapped result = apiInstance.payrollSvMeldungen(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PayrollApi#payrollSvMeldungen");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

