
# ComplianceTraining

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **assignable** | **kotlin.Boolean** | Whether HR can assign this training as required for employees. |  [optional] |
| **code** | **kotlin.String** | Stable code used by plugins and frontend players (e.g. \&quot;data_privacy\&quot;). |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **passScore** | **kotlin.Int** | Minimum score (0–100) required to pass. |  [optional] |
| **pluginPlatform** | **kotlin.String** | Marketplace plugin platform id when source &#x3D; Plugin. |  [optional] |
| **source** | [**TrainingSource**](TrainingSource.md) |  |  [optional] |
| **tenantId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **title** | **kotlin.String** |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **validityMonths** | **kotlin.Int** | Certificate validity in months; null &#x3D; no expiry. |  [optional] |



