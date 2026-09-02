# ShippingRuleApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**createShippingRule**](ShippingRuleApi.md#createShippingRule) | **POST** /api/v1/shipping-rules | 
[**deleteShippingRule**](ShippingRuleApi.md#deleteShippingRule) | **DELETE** /api/v1/shipping-rules/{rule_id} | 
[**getShippingRule**](ShippingRuleApi.md#getShippingRule) | **GET** /api/v1/shipping-rules/{rule_id} | 
[**listShippingRules**](ShippingRuleApi.md#listShippingRules) | **GET** /api/v1/shipping-rules/ | 
[**updateShippingRule**](ShippingRuleApi.md#updateShippingRule) | **PUT** /api/v1/shipping-rules/{rule_id} | 



## createShippingRule

> ShippingRule createShippingRule(shippingRuleCreate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingRuleApi;

ShippingRuleApi apiInstance = new ShippingRuleApi();
ShippingRuleCreate shippingRuleCreate = new ShippingRuleCreate(); // ShippingRuleCreate | 
try {
    ShippingRule result = apiInstance.createShippingRule(shippingRuleCreate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingRuleApi#createShippingRule");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **shippingRuleCreate** | [**ShippingRuleCreate**](ShippingRuleCreate.md)|  |

### Return type

[**ShippingRule**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json


## deleteShippingRule

> deleteShippingRule(ruleId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingRuleApi;

ShippingRuleApi apiInstance = new ShippingRuleApi();
String ruleId = null; // String | 
try {
    apiInstance.deleteShippingRule(ruleId);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingRuleApi#deleteShippingRule");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruleId** | **String**|  | [default to null]

### Return type

null (empty response body)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getShippingRule

> ShippingRule getShippingRule(ruleId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingRuleApi;

ShippingRuleApi apiInstance = new ShippingRuleApi();
String ruleId = null; // String | 
try {
    ShippingRule result = apiInstance.getShippingRule(ruleId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingRuleApi#getShippingRule");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruleId** | **String**|  | [default to null]

### Return type

[**ShippingRule**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## listShippingRules

> List&lt;ShippingRule&gt; listShippingRules(page, pageSize, country)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingRuleApi;

ShippingRuleApi apiInstance = new ShippingRuleApi();
Integer page = null; // Integer | 
Integer pageSize = null; // Integer | 
String country = null; // String | 
try {
    List<ShippingRule> result = apiInstance.listShippingRules(page, pageSize, country);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingRuleApi#listShippingRules");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **page** | **Integer**|  | [optional] [default to null]
 **pageSize** | **Integer**|  | [optional] [default to null]
 **country** | **String**|  | [optional] [default to null]

### Return type

[**List&lt;ShippingRule&gt;**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## updateShippingRule

> ShippingRule updateShippingRule(ruleId, shippingRuleUpdate)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ShippingRuleApi;

ShippingRuleApi apiInstance = new ShippingRuleApi();
String ruleId = null; // String | 
ShippingRuleUpdate shippingRuleUpdate = new ShippingRuleUpdate(); // ShippingRuleUpdate | 
try {
    ShippingRule result = apiInstance.updateShippingRule(ruleId, shippingRuleUpdate);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ShippingRuleApi#updateShippingRule");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **ruleId** | **String**|  | [default to null]
 **shippingRuleUpdate** | [**ShippingRuleUpdate**](ShippingRuleUpdate.md)|  |

### Return type

[**ShippingRule**](ShippingRule.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: application/json
- **Accept**: application/json

