
# JobPostingUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **currency** | **kotlin.String** |  |  [optional] |
| **department** | **kotlin.String** |  |  [optional] |
| **description** | **kotlin.String** | What the job is; markdown/HTML. |  [optional] |
| **employmentType** | [**EmploymentType**](EmploymentType.md) | full_time | part_time | contract | internship | temporary |  [optional] |
| **location** | **kotlin.String** |  |  [optional] |
| **remote** | **kotlin.Boolean** |  |  [optional] |
| **requiredSkills** | [**kotlin.Any**](.md) | List of required skill names (JSON array of strings). |  [optional] |
| **requirements** | **kotlin.String** | Structured profile of the required candidate (skills, experience). |  [optional] |
| **salaryMax** | **kotlin.Int** |  |  [optional] |
| **salaryMin** | **kotlin.Int** |  |  [optional] |
| **status** | [**JobPostingStatus**](JobPostingStatus.md) | draft | published | closed |  [optional] |
| **title** | **kotlin.String** |  |  [optional] |



