
# DeliveryAppointment

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **email** | **kotlin.String** |  |  |
| **requestedDate** | [**java.time.LocalDate**](java.time.LocalDate.md) |  |  |
| **status** | [**DeliveryAppointmentStatus**](DeliveryAppointmentStatus.md) | One of: requested | confirmed | arrived | cancelled | completed |  |
| **supplierName** | **kotlin.String** |  |  |
| **warehouseId** | **kotlin.String** | References the warehouse entity. |  |
| **notes** | **kotlin.String** |  |  [optional] |
| **phone** | **kotlin.String** |  |  [optional] |
| **timeSlot** | **kotlin.String** | e.g. \&quot;08:00-10:00\&quot; |  [optional] |



