# ShopApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**shopEditorSave**](ShopApi.md#shopEditorSave) | **POST** /api/v1/shop/editor | 



## shopEditorSave

> OasAnyTypeNotMapped shopEditorSave(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShopApi;

ShopApi apiInstance = new ShopApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.shopEditorSave(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShopApi#shopEditorSave");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

