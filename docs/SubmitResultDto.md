
# SubmitResultDto

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **answers** | **kotlin.collections.List&lt;kotlin.Int&gt;** | Selected answer indices (required for scored builtin trainings). |  |
| **score** | **kotlin.Int** | Score 0–100. Only trusted for plugin trainings without server-side scoring; builtin trainings are always re-scored from &#x60;answers&#x60;. |  |
| **trainingCode** | **kotlin.String** |  |  |
| **assignmentId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |



