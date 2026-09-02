# AnlageGApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**anlageGApi**](AnlageGApi.md#anlageGApi) | **GET** /api/v1/bookkeeping/anlage-g | 



## anlageGApi

> AnlageGErgebnis anlageGApi(year)



### Example

```java
// Import classes:
//import org.openapitools.client.api.AnlageGApi;

AnlageGApi apiInstance = new AnlageGApi();
Integer year = null; // Integer | 
try {
    AnlageGErgebnis result = apiInstance.anlageGApi(year);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling AnlageGApi#anlageGApi");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **year** | **Integer**|  | [default to null]

### Return type

[**AnlageGErgebnis**](AnlageGErgebnis.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

