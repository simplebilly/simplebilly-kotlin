
# Model

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **backupCodes** | **kotlin.collections.List&lt;kotlin.String&gt;** |  |  |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **email** | **kotlin.String** |  |  |
| **emailVerified** | **kotlin.Boolean** |  |  |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  |
| **isActive** | **kotlin.Boolean** |  |  |
| **isTotpEnabled** | **kotlin.Boolean** |  |  |
| **name** | **kotlin.String** |  |  |
| **passwordHash** | **kotlin.String** |  |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **lastLogin** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **oauthId** | **kotlin.String** |  |  [optional] |
| **oauthProvider** | **kotlin.String** |  |  [optional] |
| **passwordChangedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Set on password change; auth/refresh tokens issued before this timestamp are rejected by the auth middleware. |  [optional] |
| **picture** | **kotlin.String** |  |  [optional] |
| **privacyAcceptedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | When the user accepted the data privacy policy (GDPR consent record). |  [optional] |
| **totpSecret** | **kotlin.String** |  |  [optional] |



