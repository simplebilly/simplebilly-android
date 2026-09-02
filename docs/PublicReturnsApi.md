# PublicReturnsApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**getPublicReturnStatus**](PublicReturnsApi.md#getPublicReturnStatus) | **GET** /api/v1/public/returns/status | Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.
[**listPublicReturns**](PublicReturnsApi.md#listPublicReturns) | **GET** /api/v1/public/returns/list | List all returns for an order (public, no auth).
[**requestPublicReturn**](PublicReturnsApi.md#requestPublicReturn) | **POST** /api/v1/public/returns/request | Customer requests a return for an order (public, no auth).



## getPublicReturnStatus

> PublicReturnStatusResponse getPublicReturnStatus(email, returnNumber, returnOrderId, orderNumber)

Customer checks the status of a return (public, no auth). The return is only revealed when its linked order&#39;s email matches.

### Example

```java
// Import classes:
//import org.openapitools.client.api.PublicReturnsApi;

PublicReturnsApi apiInstance = new PublicReturnsApi();
String email = null; // String | 
String returnNumber = null; // String | Either return_number or return_order_id must be provided.
String returnOrderId = null; // String | 
String orderNumber = null; // String | 
try {
    PublicReturnStatusResponse result = apiInstance.getPublicReturnStatus(email, returnNumber, returnOrderId, orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PublicReturnsApi#getPublicReturnStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **email** | **String**|  | [default to null]
 **returnNumber** | **String**| Either return_number or return_order_id must be provided. | [optional] [default to null]
 **returnOrderId** | **String**|  | [optional] [default to null]
 **orderNumber** | **String**|  | [optional] [default to null]

### Return type

[**PublicReturnStatusResponse**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listPublicReturns

> List&lt;PublicReturnStatusResponse&gt; listPublicReturns(orderNumber, email)

List all returns for an order (public, no auth).

### Example

```java
// Import classes:
//import org.openapitools.client.api.PublicReturnsApi;

PublicReturnsApi apiInstance = new PublicReturnsApi();
String orderNumber = null; // String | 
String email = null; // String | 
try {
    List<PublicReturnStatusResponse> result = apiInstance.listPublicReturns(orderNumber, email);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PublicReturnsApi#listPublicReturns");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]
 **email** | **String**|  | [default to null]

### Return type

[**List&lt;PublicReturnStatusResponse&gt;**](PublicReturnStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## requestPublicReturn

> PublicReturnResponse requestPublicReturn(publicReturnRequest)

Customer requests a return for an order (public, no auth).

### Example

```java
// Import classes:
//import org.openapitools.client.api.PublicReturnsApi;

PublicReturnsApi apiInstance = new PublicReturnsApi();
PublicReturnRequest publicReturnRequest = new PublicReturnRequest(); // PublicReturnRequest | 
try {
    PublicReturnResponse result = apiInstance.requestPublicReturn(publicReturnRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PublicReturnsApi#requestPublicReturn");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **publicReturnRequest** | [**PublicReturnRequest**](PublicReturnRequest.md)|  |

### Return type

[**PublicReturnResponse**](PublicReturnResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

