# GenerateQrcodeApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**generateQrcodeApi**](GenerateQrcodeApi.md#generateQrcodeApi) | **GET** /api/v1/invoices/{id}/qrcode | 



## generateQrcodeApi

> QRCodeResponse generateQrcodeApi(iban, id, holderName, bic, amount, reference, purpose)



### Example

```java
// Import classes:
//import org.openapitools.client.api.GenerateQrcodeApi;

GenerateQrcodeApi apiInstance = new GenerateQrcodeApi();
String iban = null; // String | 
String id = null; // String | 
String holderName = null; // String | 
String bic = null; // String | 
String amount = null; // String | 
String reference = null; // String | 
String purpose = null; // String | 
try {
    QRCodeResponse result = apiInstance.generateQrcodeApi(iban, id, holderName, bic, amount, reference, purpose);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling GenerateQrcodeApi#generateQrcodeApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **iban** | **String**|  | [default to null]
 **id** | **String**|  | [default to null]
 **holderName** | **String**|  | [optional] [default to null]
 **bic** | **String**|  | [optional] [default to null]
 **amount** | **String**|  | [optional] [default to null]
 **reference** | **String**|  | [optional] [default to null]
 **purpose** | **String**|  | [optional] [default to null]

### Return type

[**QRCodeResponse**](QRCodeResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

