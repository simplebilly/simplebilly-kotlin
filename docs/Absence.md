
# Absence

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **absenceType** | [**AbsenceType**](AbsenceType.md) | One of \&quot;vacation\&quot;, \&quot;sick\&quot;, \&quot;sabbatical\&quot;, \&quot;parental\&quot;, \&quot;other\&quot;. |  [optional] |
| **approvedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **approvedBy** | [**java.util.UUID**](java.util.UUID.md) | References the user entity. |  [optional] |
| **createdAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **deletedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **employeeId** | [**java.util.UUID**](java.util.UUID.md) | References the employee entity. |  [optional] |
| **endDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **id** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **startDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **status** | [**AbsenceStatus**](AbsenceStatus.md) | One of \&quot;pending\&quot;, \&quot;approved\&quot;, \&quot;rejected\&quot;, \&quot;cancelled\&quot;. |  [optional] |
| **tenantId** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



