

# BomUpdate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**components** | [**OasAnyTypeNotMapped**](.md) | JSON array of &#x60;{product_id, name, quantity, unit, scrap_rate}&#x60;. |  [optional]
**description** | **String** |  |  [optional]
**name** | **String** |  |  [optional]
**outputQuantity** | **Long** | Output quantity per production run (defaults to 1). |  [optional]
**productId** | [**UUID**](UUID.md) | The finished product this BOM produces. References the product entity. |  [optional]
**status** | [**BomStatus**](BomStatus.md) | One of: draft | active | archived |  [optional]




