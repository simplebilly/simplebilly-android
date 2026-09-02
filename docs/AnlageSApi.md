# AnlageSApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**anlageSApi**](AnlageSApi.md#anlageSApi) | **GET** /api/v1/bookkeeping/anlage-s | 



## anlageSApi

> AnlageSErgebnis anlageSApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AnlageSApi;

AnlageSApi apiInstance = new AnlageSApi();
Integer year = null; // Integer | 
try {
    AnlageSErgebnis result = apiInstance.anlageSApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnlageSApi#anlageSApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**AnlageSErgebnis**](AnlageSErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

