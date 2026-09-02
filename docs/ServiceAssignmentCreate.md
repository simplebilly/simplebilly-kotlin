
# ServiceAssignmentCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **employeeId** | [**java.util.UUID**](java.util.UUID.md) | References the employees entity. |  [optional] |
| **jobId** | [**java.util.UUID**](java.util.UUID.md) | References the service_jobs entity. |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **scheduledDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Work day the assignment is scheduled for. |  [optional] |
| **scheduledEnd** | **kotlin.String** | Planned end time of the assignment. |  [optional] |
| **scheduledStart** | **kotlin.String** | Planned start time of the assignment. |  [optional] |
| **status** | [**ServiceAssignmentStatus**](ServiceAssignmentStatus.md) | Assignment lifecycle status: \&quot;planned\&quot;, \&quot;confirmed\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot; or \&quot;cancelled\&quot;. |  [optional] |



