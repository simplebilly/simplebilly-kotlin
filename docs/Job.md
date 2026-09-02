
# Job

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **jobType** | **kotlin.String** | Discriminator the worker dispatches on (e.g. \&quot;webhook.deliver\&quot;). |  |
| **maxAttempts** | **kotlin.Int** |  |  |
| **status** | [**JobStatus**](JobStatus.md) | pending | running | done | failed |  |
| **attempts** | **kotlin.Int** |  |  [optional] |
| **payload** | [**kotlin.Any**](.md) |  |  [optional] |
| **runAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) | Earliest execution time; None &#x3D; run now. |  [optional] |



