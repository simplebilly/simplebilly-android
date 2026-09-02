# CouponApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**couponRestore**](CouponApi.md#couponRestore) | **POST** /api/v1/coupons/{coupon_id}/restore | 
[**createCoupon**](CouponApi.md#createCoupon) | **POST** /api/v1/coupons | 
[**deleteCoupon**](CouponApi.md#deleteCoupon) | **DELETE** /api/v1/coupons/{coupon_id} | 
[**getCoupon**](CouponApi.md#getCoupon) | **GET** /api/v1/coupons/{coupon_id} | 
[**listCoupons**](CouponApi.md#listCoupons) | **GET** /api/v1/coupons/ | 
[**updateCoupon**](CouponApi.md#updateCoupon) | **PUT** /api/v1/coupons/{coupon_id} | 



## couponRestore

> Coupon couponRestore(couponId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CouponApi;

CouponApi apiInstance = new CouponApi();
String couponId = null; // String | 
try {
    Coupon result = apiInstance.couponRestore(couponId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CouponApi#couponRestore");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **couponId** | **String**|  | [default to null]

### Return type

[**Coupon**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## createCoupon

> Coupon createCoupon(couponCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CouponApi;

CouponApi apiInstance = new CouponApi();
CouponCreate couponCreate = new CouponCreate(); // CouponCreate | 
try {
    Coupon result = apiInstance.createCoupon(couponCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CouponApi#createCoupon");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **couponCreate** | [**CouponCreate**](CouponCreate.md)|  |

### Return type

[**Coupon**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteCoupon

> deleteCoupon(couponId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CouponApi;

CouponApi apiInstance = new CouponApi();
String couponId = null; // String | 
try {
    apiInstance.deleteCoupon(couponId);
} catch (ApiException e) {
    System.err.println("Exception when calling CouponApi#deleteCoupon");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **couponId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getCoupon

> Coupon getCoupon(couponId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CouponApi;

CouponApi apiInstance = new CouponApi();
String couponId = null; // String | 
try {
    Coupon result = apiInstance.getCoupon(couponId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CouponApi#getCoupon");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **couponId** | **String**|  | [default to null]

### Return type

[**Coupon**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listCoupons

> List&lt;Coupon&gt; listCoupons(page, pageSize, isActive, code, discountType)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CouponApi;

CouponApi apiInstance = new CouponApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
Boolean isActive = null; // Boolean | 
String code = null; // String | 
String discountType = null; // String | 
try {
    List<Coupon> result = apiInstance.listCoupons(page, pageSize, isActive, code, discountType);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CouponApi#listCoupons");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **isActive** | **Boolean**|  | [optional] [default to null]
 **code** | **String**|  | [optional] [default to null]
 **discountType** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;Coupon&gt;**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateCoupon

> Coupon updateCoupon(couponId, couponUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.CouponApi;

CouponApi apiInstance = new CouponApi();
String couponId = null; // String | 
CouponUpdate couponUpdate = new CouponUpdate(); // CouponUpdate | 
try {
    Coupon result = apiInstance.updateCoupon(couponId, couponUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling CouponApi#updateCoupon");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **couponId** | **String**|  | [default to null]
 **couponUpdate** | [**CouponUpdate**](CouponUpdate.md)|  |

### Return type

[**Coupon**](Coupon.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

