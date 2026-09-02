

# SupportTicket

## Properties

Name | Type | Description | Notes
------------ | ------------- | ------------- | -------------
**assignedTo** | [**UUID**](UUID.md) |  |  [optional]
**channelId** | [**UUID**](UUID.md) |  |  [optional]
**channelType** | [**SupportChannelType**](SupportChannelType.md) |  |  [optional]
**closedAt** | [**Date**](Date.md) |  |  [optional]
**createdAt** | [**Date**](Date.md) |  | 
**customerEmail** | **String** |  |  [optional]
**customerId** | **String** | References the customer entity. |  [optional]
**customerName** | **String** |  |  [optional]
**externalId** | **String** |  |  [optional]
**firstMessageAt** | [**Date**](Date.md) |  | 
**lastMessageAt** | [**Date**](Date.md) |  | 
**leadId** | [**UUID**](UUID.md) | References the lead entity. |  [optional]
**messageCount** | **Integer** |  | 
**orderRef** | **String** |  |  [optional]
**priority** | [**TicketPriority**](TicketPriority.md) |  | 
**resolution** | **String** |  |  [optional]
**status** | [**SupportTicketStatus**](SupportTicketStatus.md) |  | 
**subject** | **String** |  | 
**tags** | [**OasAnyTypeNotMapped**](.md) |  | 
**tenantId** | [**UUID**](UUID.md) |  | 
**updatedAt** | [**Date**](Date.md) |  |  [optional]




