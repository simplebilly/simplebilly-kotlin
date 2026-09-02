
# JobPostingCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **description** | **kotlin.String** | What the job is; markdown/HTML. |  |
| **remote** | **kotlin.Boolean** |  |  |
| **requiredSkills** | [**kotlin.Any**](.md) | List of required skill names (JSON array of strings). |  |
| **status** | [**JobPostingStatus**](JobPostingStatus.md) | draft | published | closed |  |
| **title** | **kotlin.String** |  |  |
| **currency** | **kotlin.String** |  |  [optional] |
| **department** | **kotlin.String** |  |  [optional] |
| **employmentType** | [**EmploymentType**](EmploymentType.md) | full_time | part_time | contract | internship | temporary |  [optional] |
| **location** | **kotlin.String** |  |  [optional] |
| **requirements** | **kotlin.String** | Structured profile of the required candidate (skills, experience). |  [optional] |
| **salaryMax** | **kotlin.Int** |  |  [optional] |
| **salaryMin** | **kotlin.Int** |  |  [optional] |



