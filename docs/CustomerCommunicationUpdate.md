
# CustomerCommunicationUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **body** | **kotlin.String** | The message body, call summary or note text. |  [optional] |
| **channel** | [**CommunicationChannel**](CommunicationChannel.md) |  |  [optional] |
| **contactId** | **kotlin.String** | The contact (customer/supplier) this communication belongs to. References the contact entity. |  [optional] |
| **counterparty** | **kotlin.String** | Email/phone of the counterparty, if applicable. |  [optional] |
| **direction** | [**CommunicationDirection**](CommunicationDirection.md) |  |  [optional] |
| **occurredAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the communication happened (defaults to now on create). |  [optional] |
| **subject** | **kotlin.String** |  |  [optional] |
| **tags** | [**kotlin.Any**](.md) | Free-form tags, e.g. &#x60;[\&quot;follow-up-required\&quot;]&#x60;. |  [optional] |



