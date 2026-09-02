# CreateSepaDirectDebitApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createSepaDirectDebitApi**](CreateSepaDirectDebitApi.md#createSepaDirectDebitApi) | **POST** /api/v1/bookkeeping/sepa-direct-debit | 



## createSepaDirectDebitApi

> SepaDirectDebitResponse createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, creditorBic, debtorBic, description)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CreateSepaDirectDebitApi;

CreateSepaDirectDebitApi apiInstance = new CreateSepaDirectDebitApi();
String creditorName = null; // String | 
String creditorIban = null; // String | 
String creditorId = null; // String | 
String mandateId = null; // String | 
String mandateDate = null; // String | 
String debtorName = null; // String | 
String debtorIban = null; // String | 
String amount = null; // String | 
String collectionDate = null; // String | 
String creditorBic = null; // String | 
String debtorBic = null; // String | 
String description = null; // String | 
try {
    SepaDirectDebitResponse result = apiInstance.createSepaDirectDebitApi(creditorName, creditorIban, creditorId, mandateId, mandateDate, debtorName, debtorIban, amount, collectionDate, creditorBic, debtorBic, description);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CreateSepaDirectDebitApi#createSepaDirectDebitApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **creditorName** | **String**|  | [default to null]
 **creditorIban** | **String**|  | [default to null]
 **creditorId** | **String**|  | [default to null]
 **mandateId** | **String**|  | [default to null]
 **mandateDate** | **String**|  | [default to null]
 **debtorName** | **String**|  | [default to null]
 **debtorIban** | **String**|  | [default to null]
 **amount** | **String**|  | [default to null]
 **collectionDate** | **String**|  | [default to null]
 **creditorBic** | **String**|  | [optional] [default to null]
 **debtorBic** | **String**|  | [optional] [default to null]
 **description** | **String**|  | [optional] [default to null]

### Return type

[**SepaDirectDebitResponse**](SepaDirectDebitResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

