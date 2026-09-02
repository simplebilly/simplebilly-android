# ReorderProposalApi

All URIs are relative to *https://demo.simplebilly.com*

Method | HTTP request | Description
------------- | ------------- | -------------
[**applyReorderProposal**](ReorderProposalApi.md#applyReorderProposal) | **POST** /api/v1/reorder-proposals/apply | Convert a reorder proposal into a draft purchase order.
[**getReorderProposal**](ReorderProposalApi.md#getReorderProposal) | **GET** /api/v1/reorder-proposals | 



## applyReorderProposal

> OasAnyTypeNotMapped applyReorderProposal(configuredOnly, warehouseId)

Convert a reorder proposal into a draft purchase order.

Returns the created purchase order id. Suggested line items are generated with the current reorder quantity per product.

### Example

```java
// Import classes:
//import org.openapitools.client.api.ReorderProposalApi;

ReorderProposalApi apiInstance = new ReorderProposalApi();
Boolean configuredOnly = null; // Boolean | Only include products with a reorder point configured (`min_stock`).
String warehouseId = null; // String | Limit to a single warehouse id.
try {
    OasAnyTypeNotMapped result = apiInstance.applyReorderProposal(configuredOnly, warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReorderProposalApi#applyReorderProposal");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **configuredOnly** | **Boolean**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] [default to null]
 **warehouseId** | **String**| Limit to a single warehouse id. | [optional] [default to null]

### Return type

[**OasAnyTypeNotMapped**](OasAnyTypeNotMapped.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json


## getReorderProposal

> ReorderProposalResponse getReorderProposal(configuredOnly, warehouseId)



### Example

```java
// Import classes:
//import org.openapitools.client.api.ReorderProposalApi;

ReorderProposalApi apiInstance = new ReorderProposalApi();
Boolean configuredOnly = null; // Boolean | Only include products with a reorder point configured (`min_stock`).
String warehouseId = null; // String | Limit to a single warehouse id.
try {
    ReorderProposalResponse result = apiInstance.getReorderProposal(configuredOnly, warehouseId);
    System.out.println(result);
} catch (ApiException e) {
    System.err.println("Exception when calling ReorderProposalApi#getReorderProposal");
    e.printStackTrace();
}
```

### Parameters


Name | Type | Description  | Notes
------------- | ------------- | ------------- | -------------
 **configuredOnly** | **Boolean**| Only include products with a reorder point configured (&#x60;min_stock&#x60;). | [optional] [default to null]
 **warehouseId** | **String**| Limit to a single warehouse id. | [optional] [default to null]

### Return type

[**ReorderProposalResponse**](ReorderProposalResponse.md)

### Authorization

[bearer_token](../README.md#bearer_token)

### HTTP request headers

- **Content-Type**: Not defined
- **Accept**: application/json

