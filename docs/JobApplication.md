
# JobApplication

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **source** | **kotlin.String** | website | email | board |  |
| **status** | [**ApplicationStatus**](ApplicationStatus.md) | new | reviewing | interview | hired | rejected |  |
| **cvFile** | **kotlin.String** | Relative path of the stored CV file under the upload dir. |  [optional] |
| **cvText** | **kotlin.String** | Extracted CV text, used for match-scoring. |  [optional] |
| **email** | **kotlin.String** |  |  [optional] |
| **matchReason** | **kotlin.String** |  |  [optional] |
| **matchScore** | **kotlin.Int** | 0-100 LLM match score against the posting&#39;s required profile. |  [optional] |
| **name** | **kotlin.String** |  |  [optional] |
| **phone** | **kotlin.String** |  |  [optional] |
| **postingId** | [**java.util.UUID**](java.util.UUID.md) | References the job_posting entity. |  [optional] |



