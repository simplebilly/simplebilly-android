# PosApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**posBilling**](PosApi.md#posBilling) | **GET** /api/pos/billing | 
[**posCreateOrder**](PosApi.md#posCreateOrder) | **POST** /api/pos/orders | 
[**posCreateRegister**](PosApi.md#posCreateRegister) | **POST** /api/pos/registers | 
[**posCreateTable**](PosApi.md#posCreateTable) | **POST** /api/pos/tables | 
[**posDisableRegister**](PosApi.md#posDisableRegister) | **POST** /api/pos/registers/{id}/disable | 
[**posFreeTable**](PosApi.md#posFreeTable) | **POST** /api/pos/tables/{id}/free | 
[**posKasseClosing**](PosApi.md#posKasseClosing) | **POST** /api/pos/kasse/closing | 
[**posKasseEntries**](PosApi.md#posKasseEntries) | **GET** /api/pos/kasse/entries | 
[**posKasseExport**](PosApi.md#posKasseExport) | **GET** /api/pos/kasse/export | 
[**posKassePayInOut**](PosApi.md#posKassePayInOut) | **POST** /api/pos/kasse/pay-in-out | 
[**posListOrders**](PosApi.md#posListOrders) | **GET** /api/pos/orders | 
[**posListProducts**](PosApi.md#posListProducts) | **GET** /api/pos/products | 
[**posListRegisters**](PosApi.md#posListRegisters) | **GET** /api/pos/registers | 
[**posListTables**](PosApi.md#posListTables) | **GET** /api/pos/tables | 
[**posOrderPrint**](PosApi.md#posOrderPrint) | **GET** /api/pos/orders/{order_number}/print | 
[**posOrderReceipt**](PosApi.md#posOrderReceipt) | **GET** /api/pos/orders/{order_number}/receipt | 
[**posPayOrder**](PosApi.md#posPayOrder) | **POST** /api/pos/orders/{order_number}/pay | 
[**posSumupCheckout**](PosApi.md#posSumupCheckout) | **POST** /api/pos/sumup/checkout | 



## posBilling

> OasAnyTypeNotMapped posBilling()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
try {
    OasAnyTypeNotMapped result = apiInstance.posBilling();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posBilling");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posCreateOrder

> OasAnyTypeNotMapped posCreateOrder(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.posCreateOrder(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posCreateOrder");
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


## posCreateRegister

> PosRegister posCreateRegister(posRegisterCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
PosRegisterCreate posRegisterCreate = new PosRegisterCreate(); // PosRegisterCreate | 
try {
    PosRegister result = apiInstance.posCreateRegister(posRegisterCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posCreateRegister");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **posRegisterCreate** | [**PosRegisterCreate**](PosRegisterCreate.md)|  |

### Return type

[**PosRegister**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## posCreateTable

> PosTable posCreateTable(posTableCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
PosTableCreate posTableCreate = new PosTableCreate(); // PosTableCreate | 
try {
    PosTable result = apiInstance.posCreateTable(posTableCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posCreateTable");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **posTableCreate** | [**PosTableCreate**](PosTableCreate.md)|  |

### Return type

[**PosTable**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## posDisableRegister

> PosRegister posDisableRegister(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
UUID id = null; // UUID | 
try {
    PosRegister result = apiInstance.posDisableRegister(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posDisableRegister");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**PosRegister**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posFreeTable

> PosTable posFreeTable(id)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
UUID id = null; // UUID | 
try {
    PosTable result = apiInstance.posFreeTable(id);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posFreeTable");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **id** | **UUID**|  | [default to null]

### Return type

[**PosTable**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posKasseClosing

> OasAnyTypeNotMapped posKasseClosing(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.posKasseClosing(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posKasseClosing");
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


## posKasseEntries

> OasAnyTypeNotMapped posKasseEntries()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
try {
    OasAnyTypeNotMapped result = apiInstance.posKasseEntries();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posKasseEntries");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posKasseExport

> OasAnyTypeNotMapped posKasseExport()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
try {
    OasAnyTypeNotMapped result = apiInstance.posKasseExport();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posKasseExport");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posKassePayInOut

> OasAnyTypeNotMapped posKassePayInOut(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.posKassePayInOut(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posKassePayInOut");
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


## posListOrders

> OasAnyTypeNotMapped posListOrders(status)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
String status = null; // String | Filter by order status
try {
    OasAnyTypeNotMapped result = apiInstance.posListOrders(status);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posListOrders");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **status** | **String**| Filter by order status | [optional] [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posListProducts

> OasAnyTypeNotMapped posListProducts(q)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
String q = null; // String | Product search
try {
    OasAnyTypeNotMapped result = apiInstance.posListProducts(q);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posListProducts");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **q** | **String**| Product search | [optional] [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posListRegisters

> List&lt;PosRegister&gt; posListRegisters()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
try {
    List<PosRegister> result = apiInstance.posListRegisters();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posListRegisters");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PosRegister&gt;**](PosRegister.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posListTables

> List&lt;PosTable&gt; posListTables()



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
try {
    List<PosTable> result = apiInstance.posListTables();
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posListTables");
    e.printStackTrace();
}
```

### Parameters

This endpoint does not need any parameter.

### Return type

[**List&lt;PosTable&gt;**](PosTable.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posOrderPrint

> OasAnyTypeNotMapped posOrderPrint(orderNumber)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
String orderNumber = null; // String | 
try {
    OasAnyTypeNotMapped result = apiInstance.posOrderPrint(orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posOrderPrint");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posOrderReceipt

> OasAnyTypeNotMapped posOrderReceipt(orderNumber)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
String orderNumber = null; // String | 
try {
    OasAnyTypeNotMapped result = apiInstance.posOrderReceipt(orderNumber);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posOrderReceipt");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## posPayOrder

> OasAnyTypeNotMapped posPayOrder(orderNumber, body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
String orderNumber = null; // String | 
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.posPayOrder(orderNumber, body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posPayOrder");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **orderNumber** | **String**|  | [default to null]
 **body** | **OasAnyTypeNotMapped**|  |

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## posSumupCheckout

> OasAnyTypeNotMapped posSumupCheckout(body)



### Example

```java
// Import classes:
//import org.openapitools.client.api.PosApi;

PosApi apiInstance = new PosApi();
OasAnyTypeNotMapped body = new OasAnyTypeNotMapped(); // OasAnyTypeNotMapped | 
try {
    OasAnyTypeNotMapped result = apiInstance.posSumupCheckout(body);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling PosApi#posSumupCheckout");
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

