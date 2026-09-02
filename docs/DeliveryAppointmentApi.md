# DeliveryAppointmentApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createDeliveryAppointment**](DeliveryAppointmentApi.md#createDeliveryAppointment) | **POST** /api/v1/delivery-appointments | 
[**deleteDeliveryAppointment**](DeliveryAppointmentApi.md#deleteDeliveryAppointment) | **DELETE** /api/v1/delivery-appointments/{appointment_id} | 
[**getDeliveryAppointment**](DeliveryAppointmentApi.md#getDeliveryAppointment) | **GET** /api/v1/delivery-appointments/{appointment_id} | 
[**getPublicDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#getPublicDeliveryAppointmentStatus) | **GET** /api/v1/public/delivery-appointments/status | Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.
[**listDeliveryAppointments**](DeliveryAppointmentApi.md#listDeliveryAppointments) | **GET** /api/v1/delivery-appointments | 
[**requestPublicDeliveryAppointment**](DeliveryAppointmentApi.md#requestPublicDeliveryAppointment) | **POST** /api/v1/public/delivery-appointments/request | Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.
[**updateDeliveryAppointment**](DeliveryAppointmentApi.md#updateDeliveryAppointment) | **PUT** /api/v1/delivery-appointments/{appointment_id} | 
[**updateDeliveryAppointmentStatus**](DeliveryAppointmentApi.md#updateDeliveryAppointmentStatus) | **PUT** /api/v1/delivery-appointments/{appointment_id}/status | 



## createDeliveryAppointment

> DeliveryAppointment createDeliveryAppointment(deliveryAppointmentCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
DeliveryAppointmentCreate deliveryAppointmentCreate = new DeliveryAppointmentCreate(); // DeliveryAppointmentCreate | 
try {
    DeliveryAppointment result = apiInstance.createDeliveryAppointment(deliveryAppointmentCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#createDeliveryAppointment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **deliveryAppointmentCreate** | [**DeliveryAppointmentCreate**](DeliveryAppointmentCreate.md)|  |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteDeliveryAppointment

> deleteDeliveryAppointment(appointmentId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
String appointmentId = null; // String | 
try {
    apiInstance.deleteDeliveryAppointment(appointmentId);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#deleteDeliveryAppointment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointmentId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getDeliveryAppointment

> DeliveryAppointment getDeliveryAppointment(appointmentId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
String appointmentId = null; // String | 
try {
    DeliveryAppointment result = apiInstance.getDeliveryAppointment(appointmentId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#getDeliveryAppointment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointmentId** | **String**|  | [default to null]

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getPublicDeliveryAppointmentStatus

> PublicDeliveryAppointmentStatusResponse getPublicDeliveryAppointmentStatus(appointmentId, email, token)

Supplier/carrier checks appointment status (public, no auth). The appointment is only revealed when email AND token match.

### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
String appointmentId = null; // String | 
String email = null; // String | 
String token = null; // String | 
try {
    PublicDeliveryAppointmentStatusResponse result = apiInstance.getPublicDeliveryAppointmentStatus(appointmentId, email, token);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#getPublicDeliveryAppointmentStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointmentId** | **String**|  | [default to null]
 **email** | **String**|  | [default to null]
 **token** | **String**|  | [default to null]

### Return type

[**PublicDeliveryAppointmentStatusResponse**](PublicDeliveryAppointmentStatusResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listDeliveryAppointments

> List&lt;DeliveryAppointment&gt; listDeliveryAppointments(page, pageSize, status, warehouseId, from, to)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String status = null; // String | 
String warehouseId = null; // String | 
Date from = null; // Date | 
Date to = null; // Date | 
try {
    List<DeliveryAppointment> result = apiInstance.listDeliveryAppointments(page, pageSize, status, warehouseId, from, to);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#listDeliveryAppointments");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **status** | **String**|  | [optional] [default to null]
 **warehouseId** | **String**|  | [optional] [default to null]
 **from** | **Date**|  | [optional] [default to null]
 **to** | **Date**|  | [optional] [default to null]

### Return type

[**List&lt;DeliveryAppointment&gt;**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## requestPublicDeliveryAppointment

> PublicDeliveryAppointmentResponse requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest)

Supplier/carrier requests an inbound delivery slot (public, no auth). The tenant is derived from the warehouse found by &#x60;code&#x60; — never from the request.

### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
PublicDeliveryAppointmentRequest publicDeliveryAppointmentRequest = new PublicDeliveryAppointmentRequest(); // PublicDeliveryAppointmentRequest | 
try {
    PublicDeliveryAppointmentResponse result = apiInstance.requestPublicDeliveryAppointment(publicDeliveryAppointmentRequest);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#requestPublicDeliveryAppointment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **publicDeliveryAppointmentRequest** | [**PublicDeliveryAppointmentRequest**](PublicDeliveryAppointmentRequest.md)|  |

### Return type

[**PublicDeliveryAppointmentResponse**](PublicDeliveryAppointmentResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateDeliveryAppointment

> DeliveryAppointment updateDeliveryAppointment(appointmentId, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
String appointmentId = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    DeliveryAppointment result = apiInstance.updateDeliveryAppointment(appointmentId, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#updateDeliveryAppointment");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointmentId** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## updateDeliveryAppointmentStatus

> DeliveryAppointment updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.DeliveryAppointmentApi;

DeliveryAppointmentApi apiInstance = new DeliveryAppointmentApi();
String appointmentId = null; // String | 
AppointmentStatusUpdate appointmentStatusUpdate = new AppointmentStatusUpdate(); // AppointmentStatusUpdate | 
try {
    DeliveryAppointment result = apiInstance.updateDeliveryAppointmentStatus(appointmentId, appointmentStatusUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling DeliveryAppointmentApi#updateDeliveryAppointmentStatus");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **appointmentId** | **String**|  | [default to null]
 **appointmentStatusUpdate** | [**AppointmentStatusUpdate**](AppointmentStatusUpdate.md)|  |

### Return type

[**DeliveryAppointment**](DeliveryAppointment.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

