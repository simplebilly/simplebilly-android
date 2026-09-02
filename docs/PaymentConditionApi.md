# PaymentConditionApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**listPaymentConditionsApi**](PaymentConditionApi.md#listPaymentConditionsApi) | **GET** /api/v1/payment-conditions | 



## listPaymentConditionsApi

> List&lt;PaymentCondition&gt; listPaymentConditionsApi()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PaymentConditionApi;

PaymentConditionApi apiInstance = new PaymentConditionApi();
try {
    List<PaymentCondition> result = apiInstance.listPaymentConditionsApi();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PaymentConditionApi#listPaymentConditionsApi");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PaymentCondition&gt;**](PaymentCondition.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

