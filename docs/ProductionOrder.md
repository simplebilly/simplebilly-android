

# ProductionOrder

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**bomId** | [**UUID**](UUID.md) | References the BOM entity. |  [optional]
**components** | [**OasAnyTypeNotMapped**](.md) | JSON snapshot of the BOM components at creation time. |  [optional]
**endDate** | [**Date**](Date.md) |  |  [optional]
**notes** | **String** |  |  [optional]
**orderNumber** | **String** |  | 
**productId** | [**UUID**](UUID.md) | The finished product to manufacture. References the product entity. | 
**quantity** | **Long** | Quantity of finished product to produce. | 
**sourceWarehouseId** | **String** | Warehouse components are consumed from. References the warehouse entity. |  [optional]
**startDate** | [**Date**](Date.md) |  |  [optional]
**status** | [**ProductionOrderStatus**](ProductionOrderStatus.md) | One of: planned | in_production | completed | cancelled |  [optional]
**targetWarehouseId** | **String** | Warehouse the finished product is added to. References the warehouse entity. |  [optional]




