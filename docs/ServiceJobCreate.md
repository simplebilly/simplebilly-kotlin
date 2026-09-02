
# ServiceJobCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **address** | **kotlin.String** | Street + zip + city of the job location. |  [optional] |
| **customerEmail** | **kotlin.String** | Customer email for email notifications. |  [optional] |
| **customerId** | [**java.util.UUID**](java.util.UUID.md) | References the customer entity. |  [optional] |
| **customerName** | **kotlin.String** | Denormalized customer name for quick display. |  [optional] |
| **customerPhone** | **kotlin.String** | Customer phone for SMS notifications later. |  [optional] |
| **description** | **kotlin.String** | What work needs to be done. |  [optional] |
| **estimatedDurationMinutes** | **kotlin.Int** | Estimated time for the job in minutes. |  [optional] |
| **lat** | **kotlin.Double** | Latitude for map display (OpenStreetMap). |  [optional] |
| **lng** | **kotlin.Double** | Longitude for map display (OpenStreetMap). |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **status** | [**ServiceJobStatus**](ServiceJobStatus.md) | Dispatch status: \&quot;pending\&quot;, \&quot;assigned\&quot;, \&quot;en_route\&quot;, \&quot;in_progress\&quot;, \&quot;completed\&quot;, \&quot;cancelled\&quot;. |  [optional] |



