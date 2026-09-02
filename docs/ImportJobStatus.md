
# ImportJobStatus

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **jobId** | **kotlin.String** |  |  |
| **processed** | **kotlin.Long** |  |  |
| **progress** | **kotlin.Int** | 0–100 |  |
| **stage** | **kotlin.String** | queued | fetching | downloading | importing | done |  |
| **status** | **kotlin.String** | pending | running | done | failed |  |
| **total** | **kotlin.Long** |  |  |
| **error** | **kotlin.String** | Set only when the job failed. |  [optional] |
| **provider** | **kotlin.String** | Which competitor the import came from (lexoffice | billbee); the frontend uses it to label the job. Absent for legacy jobs. |  [optional] |



