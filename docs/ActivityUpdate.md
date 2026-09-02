
# ActivityUpdate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **activityType** | [**ActivityType**](ActivityType.md) | One of: call | email | meeting | task | note |  [optional] |
| **assignedTo** | **kotlin.String** | User responsible (&#x60;employee.employee_id&#x60;). |  [optional] |
| **contactId** | **kotlin.String** | Contact this activity belongs to (&#x60;contact.contact_id&#x60;). References the contact entity. |  [optional] |
| **description** | **kotlin.String** |  |  [optional] |
| **dueDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Follow-up / Wiedervorlage date. Open activities with a due date in the past are overdue. |  [optional] |
| **reminderDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | When to remind about the follow-up. |  [optional] |
| **status** | [**ActivityStatus**](ActivityStatus.md) | One of: open | done | cancelled |  [optional] |
| **subject** | **kotlin.String** | Short subject line. |  [optional] |



