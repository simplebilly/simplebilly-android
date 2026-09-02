

# DeliveryDate

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**customerId** | **String** | References the customer entity. |  [optional]
**fulfilledDate** | [**Date**](Date.md) | Date actually delivered (set on fulfillment). |  [optional]
**note** | **String** |  |  [optional]
**orderNumber** | **String** | Sales order number (&#x60;order.order_number&#x60;). | 
**originalDate** | [**Date**](Date.md) | Original date promised before rescheduling. |  [optional]
**productId** | **String** | Product line item this date applies to, if per-item. References the product entity. |  [optional]
**promisedDate** | [**Date**](Date.md) | Date promised to the customer. | 
**status** | [**DeliveryDateStatus**](DeliveryDateStatus.md) | One of: promised | confirmed | rescheduled | fulfilled | late | cancelled | 




