# BankingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**bankLookupApi**](BankingApi.md#bankLookupApi) | **GET** /api/v1/bookkeeping/banking/lookup | 
[**bankTransactionsApi**](BankingApi.md#bankTransactionsApi) | **GET** /api/v1/bookkeeping/banking/transactions | 
[**hebesatzLookupApi**](BankingApi.md#hebesatzLookupApi) | **GET** /api/v1/bookkeeping/hebesatz | 



## bankLookupApi

> BankLookup bankLookupApi(iban)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BankingApi;

BankingApi apiInstance = new BankingApi();
String iban = null; // String | 
try {
    BankLookup result = apiInstance.bankLookupApi(iban);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BankingApi#bankLookupApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iban** | **String**|  | [default to null]

### Return type

[**BankLookup**](BankLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## bankTransactionsApi

> bankTransactionsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.BankingApi;

BankingApi apiInstance = new BankingApi();
try {
    apiInstance.bankTransactionsApi();
} catch (ApiException e) {
    System.err.println("Exception when calling BankingApi#bankTransactionsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## hebesatzLookupApi

> List&lt;HebesatzLookup&gt; hebesatzLookupApi(gemeindeschluessel, plz, name, stichtag, countryCode)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BankingApi;

BankingApi apiInstance = new BankingApi();
String gemeindeschluessel = null; // String | 
String plz = null; // String | 
String name = null; // String | 
String stichtag = null; // String | Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from <= date <= valid_to.
String countryCode = null; // String | 
try {
    List<HebesatzLookup> result = apiInstance.hebesatzLookupApi(gemeindeschluessel, plz, name, stichtag, countryCode);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BankingApi#hebesatzLookupApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **gemeindeschluessel** | **String**|  | [optional] [default to null]
 **plz** | **String**|  | [optional] [default to null]
 **name** | **String**|  | [optional] [default to null]
 **stichtag** | **String**| Stichtag for validity (YYYY-MM-DD); defaults to today. Picks row where valid_from &lt;&#x3D; date &lt;&#x3D; valid_to. | [optional] [default to null]
 **countryCode** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;HebesatzLookup&gt;**](HebesatzLookup.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

