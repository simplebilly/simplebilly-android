# VoucherApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createVoucher**](VoucherApi.md#createVoucher) | **POST** /api/v1/vouchers | 
[**deleteVoucher**](VoucherApi.md#deleteVoucher) | **DELETE** /api/v1/vouchers/{voucher_id} | 
[**getVoucher**](VoucherApi.md#getVoucher) | **GET** /api/v1/vouchers/{voucher_id} | 
[**listVouchers**](VoucherApi.md#listVouchers) | **GET** /api/v1/vouchers/ | 
[**updateVoucher**](VoucherApi.md#updateVoucher) | **PUT** /api/v1/vouchers/{voucher_id} | 
[**voucherRestore**](VoucherApi.md#voucherRestore) | **POST** /api/v1/vouchers/{voucher_id}/restore | 



## createVoucher

> Voucher createVoucher(voucherCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.VoucherApi;

VoucherApi apiInstance = new VoucherApi();
VoucherCreate voucherCreate = new VoucherCreate(); // VoucherCreate | 
try {
    Voucher result = apiInstance.createVoucher(voucherCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling VoucherApi#createVoucher");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherCreate** | [**VoucherCreate**](VoucherCreate.md)|  |

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteVoucher

> deleteVoucher(voucherId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.VoucherApi;

VoucherApi apiInstance = new VoucherApi();
String voucherId = null; // String | 
try {
    apiInstance.deleteVoucher(voucherId);
} catch (ApiException e) {
    System.err.println("Exception when calling VoucherApi#deleteVoucher");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getVoucher

> Voucher getVoucher(voucherId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.VoucherApi;

VoucherApi apiInstance = new VoucherApi();
String voucherId = null; // String | 
try {
    Voucher result = apiInstance.getVoucher(voucherId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling VoucherApi#getVoucher");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | [default to null]

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listVouchers

> List&lt;Voucher&gt; listVouchers(page, pageSize, voucherType, voucherStatus, contactName, dateFrom, dateTo)



### Example

```java
// Import classes:
//import org.openapitools.client.api.VoucherApi;

VoucherApi apiInstance = new VoucherApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String voucherType = null; // String | 
String voucherStatus = null; // String | 
String contactName = null; // String | 
Date dateFrom = null; // Date | 
Date dateTo = null; // Date | 
try {
    List<Voucher> result = apiInstance.listVouchers(page, pageSize, voucherType, voucherStatus, contactName, dateFrom, dateTo);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling VoucherApi#listVouchers");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **voucherType** | **String**|  | [optional] [default to null]
 **voucherStatus** | **String**|  | [optional] [default to null]
 **contactName** | **String**|  | [optional] [default to null]
 **dateFrom** | **Date**|  | [optional] [default to null]
 **dateTo** | **Date**|  | [optional] [default to null]

### Return type

[**List&lt;Voucher&gt;**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateVoucher

> Voucher updateVoucher(voucherId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.VoucherApi;

VoucherApi apiInstance = new VoucherApi();
String voucherId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Voucher result = apiInstance.updateVoucher(voucherId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling VoucherApi#updateVoucher");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## voucherRestore

> Voucher voucherRestore(voucherId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.VoucherApi;

VoucherApi apiInstance = new VoucherApi();
String voucherId = null; // String | 
try {
    Voucher result = apiInstance.voucherRestore(voucherId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling VoucherApi#voucherRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **voucherId** | **String**|  | [default to null]

### Return type

[**Voucher**](Voucher.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

