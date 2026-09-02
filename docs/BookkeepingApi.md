# BookkeepingApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**allocatePaymentApi**](BookkeepingApi.md#allocatePaymentApi) | **POST** /api/v1/payments/allocate | Allocate a payment to an invoice
[**bwaReportApi**](BookkeepingApi.md#bwaReportApi) | **GET** /api/v1/bookkeeping/bwa | Get BWA (Betriebswirtschaftliche Auswertung) report
[**elsterStatusApi**](BookkeepingApi.md#elsterStatusApi) | **GET** /api/v1/bookkeeping/elster/status | 
[**elsterValidateApi**](BookkeepingApi.md#elsterValidateApi) | **POST** /api/v1/bookkeeping/ustva/elster-validate | 
[**elsterXmlApi**](BookkeepingApi.md#elsterXmlApi) | **GET** /api/v1/bookkeeping/ustva/elster-xml | 
[**getCashflow**](BookkeepingApi.md#getCashflow) | **GET** /api/v1/bookkeeping/cashflow | GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.
[**getLiquidity**](BookkeepingApi.md#getLiquidity) | **GET** /api/v1/bookkeeping/liquidity | GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.
[**getOpenInvoicesApi**](BookkeepingApi.md#getOpenInvoicesApi) | **GET** /api/v1/payments/open-invoices/{customer_id} | Get open invoices for a customer
[**getVerfahrensdokumentation**](BookkeepingApi.md#getVerfahrensdokumentation) | **GET** /api/v1/bookkeeping/verfahrensdokumentation | GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.
[**runDunningApi**](BookkeepingApi.md#runDunningApi) | **POST** /api/v1/bookkeeping/dunning | 



## allocatePaymentApi

> allocatePaymentApi(allocatePaymentRequest)

Allocate a payment to an invoice

### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
AllocatePaymentRequest allocatePaymentRequest = new AllocatePaymentRequest(); // AllocatePaymentRequest | 
try {
    apiInstance.allocatePaymentApi(allocatePaymentRequest);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#allocatePaymentApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **allocatePaymentRequest** | [**AllocatePaymentRequest**](AllocatePaymentRequest.md)|  |

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## bwaReportApi

> BWAReport bwaReportApi(year, month)

Get BWA (Betriebswirtschaftliche Auswertung) report

### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
try {
    BWAReport result = apiInstance.bwaReportApi(year, month);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#bwaReportApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **month** | **Integer**|  | [optional] [default to null]

### Return type

[**BWAReport**](BWAReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## elsterStatusApi

> ElsterStatus elsterStatusApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
try {
    ElsterStatus result = apiInstance.elsterStatusApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#elsterStatusApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**ElsterStatus**](ElsterStatus.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## elsterValidateApi

> elsterValidateApi(zeitraum)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
String zeitraum = null; // String | 
try {
    apiInstance.elsterValidateApi(zeitraum);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#elsterValidateApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zeitraum** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## elsterXmlApi

> elsterXmlApi(zeitraum)



### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
String zeitraum = null; // String | 
try {
    apiInstance.elsterXmlApi(zeitraum);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#elsterXmlApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **zeitraum** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: Not defined


## getCashflow

> CashflowReport getCashflow(year, month)

GET /api/v1/bookkeeping/cashflow Returns operating, investing, and financing cashflow for the given period.

### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
Integer year = null; // Integer | 
Integer month = null; // Integer | 
try {
    CashflowReport result = apiInstance.getCashflow(year, month);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#getCashflow");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [optional] [default to null]
 **month** | **Integer**|  | [optional] [default to null]

### Return type

[**CashflowReport**](CashflowReport.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getLiquidity

> LiquidityPosition getLiquidity()

GET /api/v1/bookkeeping/liquidity Returns current liquidity position with ratios.

### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
try {
    LiquidityPosition result = apiInstance.getLiquidity();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#getLiquidity");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**LiquidityPosition**](LiquidityPosition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getOpenInvoicesApi

> List&lt;Invoice&gt; getOpenInvoicesApi(customerId)

Get open invoices for a customer

### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
String customerId = null; // String | 
try {
    List<Invoice> result = apiInstance.getOpenInvoicesApi(customerId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#getOpenInvoicesApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **customerId** | **String**|  | [default to null]

### Return type

[**List&lt;Invoice&gt;**](Invoice.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getVerfahrensdokumentation

> Verfahrensdokumentation getVerfahrensdokumentation()

GET /api/v1/bookkeeping/verfahrensdokumentation Returns the complete compliance catalog of all documented modules.

### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
try {
    Verfahrensdokumentation result = apiInstance.getVerfahrensdokumentation();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#getVerfahrensdokumentation");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**Verfahrensdokumentation**](Verfahrensdokumentation.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## runDunningApi

> DunningResult runDunningApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.BookkeepingApi;

BookkeepingApi apiInstance = new BookkeepingApi();
try {
    DunningResult result = apiInstance.runDunningApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling BookkeepingApi#runDunningApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**DunningResult**](DunningResult.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

