# RfqApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**convertRfq**](RfqApi.md#convertRfq) | **POST** /api/v1/rfqs/{rfq_id}/convert | Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;.
[**createRfq**](RfqApi.md#createRfq) | **POST** /api/v1/rfqs | 
[**deleteRfq**](RfqApi.md#deleteRfq) | **DELETE** /api/v1/rfqs/{rfq_id} | 
[**getRfq**](RfqApi.md#getRfq) | **GET** /api/v1/rfqs/{rfq_id} | 
[**listRfqs**](RfqApi.md#listRfqs) | **GET** /api/v1/rfqs/ | 
[**updateRfq**](RfqApi.md#updateRfq) | **PUT** /api/v1/rfqs/{rfq_id} | 
[**updateRfqStatus**](RfqApi.md#updateRfqStatus) | **PUT** /api/v1/rfqs/{rfq_id}/status | 



## convertRfq

> OasAnyTypeNotMapped convertRfq(rfqId)

Convert an RFQ into a draft purchase order using the quoted unit prices (falling back to the requested prices, then leaving them blank). Marks the RFQ as &#x60;converted&#x60;.

### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
String rfqId = null; // String | 
try {
    OasAnyTypeNotMapped result = apiInstance.convertRfq(rfqId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#convertRfq");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rfqId** | **String**|  | [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## createRfq

> Rfq createRfq(rfq)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
Rfq rfq = new Rfq(); // Rfq | 
try {
    Rfq result = apiInstance.createRfq(rfq);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#createRfq");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rfq** | [**Rfq**](Rfq.md)|  |

### Return type

[**Rfq**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteRfq

> deleteRfq(rfqId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
String rfqId = null; // String | 
try {
    apiInstance.deleteRfq(rfqId);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#deleteRfq");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rfqId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getRfq

> Rfq getRfq(rfqId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
String rfqId = null; // String | 
try {
    Rfq result = apiInstance.getRfq(rfqId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#getRfq");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rfqId** | **String**|  | [default to null]

### Return type

[**Rfq**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listRfqs

> List&lt;Rfq&gt; listRfqs(page, pageSize, status, supplierName)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String supplierName = null; // String | 
try {
    List<Rfq> result = apiInstance.listRfqs(page, pageSize, status, supplierName);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#listRfqs");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **supplierName** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;Rfq&gt;**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateRfq

> Rfq updateRfq(rfqId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
String rfqId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    Rfq result = apiInstance.updateRfq(rfqId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#updateRfq");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rfqId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**Rfq**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateRfqStatus

> Rfq updateRfqStatus(rfqId, rfqStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.RfqApi;

RfqApi apiInstance = new RfqApi();
String rfqId = null; // String | 
RfqStatusUpdate rfqStatusUpdate = new RfqStatusUpdate(); // RfqStatusUpdate | 
try {
    Rfq result = apiInstance.updateRfqStatus(rfqId, rfqStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling RfqApi#updateRfqStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **rfqId** | **String**|  | [default to null]
 **rfqStatusUpdate** | [**RfqStatusUpdate**](RfqStatusUpdate.md)|  |

### Return type

[**Rfq**](Rfq.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

