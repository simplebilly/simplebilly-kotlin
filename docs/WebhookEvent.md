
# WebhookEvent

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **direction** | [**WebhookDirection**](WebhookDirection.md) | inbound | outbound |  |
| **eventType** | **kotlin.String** |  |  |
| **attempts** | **kotlin.Int** |  |  [optional] |
| **channel** | **kotlin.String** | source for inbound, target URL for outbound. |  [optional] |
| **lastError** | **kotlin.String** |  |  [optional] |
| **payload** | [**kotlin.Any**](.md) |  |  [optional] |
| **status** | [**WebhookEventStatus**](WebhookEventStatus.md) | accepted | delivered | failed |  [optional] |



