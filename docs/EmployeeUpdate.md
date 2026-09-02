
# EmployeeUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **address** | **kotlin.String** |  |  [optional] |
| **backupEmployeeId** | [**java.util.UUID**](java.util.UUID.md) | References another employee who covers when this employee is absent. |  [optional] |
| **bic** | **kotlin.String** |  |  [optional] |
| **city** | **kotlin.String** |  |  [optional] |
| **country** | [**CountryCode**](CountryCode.md) |  |  [optional] |
| **dateOfBirth** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **departmentId** | [**java.util.UUID**](java.util.UUID.md) | References the department entity. |  [optional] |
| **email** | **kotlin.String** |  |  [optional] |
| **firstName** | **kotlin.String** |  |  [optional] |
| **gender** | [**Gender**](Gender.md) | Gender for pay-transparency reporting: \&quot;male\&quot;, \&quot;female\&quot; or \&quot;diverse\&quot;. |  [optional] |
| **hireDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  [optional] |
| **hourlyCost** | **kotlin.String** | Hourly cost rate in EUR for labor-cost reporting; when unset the rate is derived from &#x60;monthly_salary / (weekly_hours * 4.33)&#x60;. |  [optional] |
| **iban** | **kotlin.String** |  |  [optional] |
| **jobTitle** | **kotlin.String** |  |  [optional] |
| **lastLogin** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **lastName** | **kotlin.String** |  |  [optional] |
| **lastUpdated** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **monthlySalary** | **kotlin.String** | Gross monthly salary in EUR for pay-transparency reporting. |  [optional] |
| **phone** | **kotlin.String** |  |  [optional] |
| **state** | **kotlin.String** |  |  [optional] |
| **status** | [**EmployeeStatus**](EmployeeStatus.md) |  |  [optional] |
| **userId** | [**java.util.UUID**](java.util.UUID.md) | References the user entity. |  [optional] |
| **weeklyHours** | **kotlin.String** | Contractual weekly working hours for pay-transparency normalization. |  [optional] |
| **zip** | **kotlin.String** |  |  [optional] |



