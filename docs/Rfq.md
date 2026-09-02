

# Rfq

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**currency** | **String** |  |  [optional]
**lineItems** | [**OasAnyTypeNotMapped**](.md) | JSON array of &#x60;{product_id, name, sku, quantity, requested_unit_price?, quoted_unit_price?}&#x60;. | 
**notes** | **String** |  |  [optional]
**requestedDate** | [**Date**](Date.md) |  | 
**responseDate** | [**Date**](Date.md) |  |  [optional]
**rfqNumber** | **String** |  | 
**status** | [**RfqStatus**](RfqStatus.md) | One of: draft | sent | offer_received | rejected | converted | 
**supplierContactId** | **String** | References the supplier entity. |  [optional]
**supplierName** | **String** |  |  [optional]




