
# SupportTicket

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **firstMessageAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **lastMessageAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **messageCount** | **kotlin.Int** |  |  |
| **priority** | [**TicketPriority**](TicketPriority.md) |  |  |
| **status** | [**SupportTicketStatus**](SupportTicketStatus.md) |  |  |
| **subject** | **kotlin.String** |  |  |
| **tags** | [**kotlin.Any**](.md) |  |  |
| **tenantId** | [**java.util.UUID**](java.util.UUID.md) |  |  |
| **assignedTo** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **channelId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **channelType** | [**SupportChannelType**](SupportChannelType.md) |  |  [optional] |
| **closedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **customerEmail** | **kotlin.String** |  |  [optional] |
| **customerId** | **kotlin.String** | References the customer entity. |  [optional] |
| **customerName** | **kotlin.String** |  |  [optional] |
| **externalId** | **kotlin.String** |  |  [optional] |
| **leadId** | [**java.util.UUID**](java.util.UUID.md) | References the lead entity. |  [optional] |
| **orderRef** | **kotlin.String** |  |  [optional] |
| **resolution** | **kotlin.String** |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



