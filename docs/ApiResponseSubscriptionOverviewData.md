
# ApiResponseSubscriptionOverviewData

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **features** | [**PlanFeatures**](PlanFeatures.md) |  |  |
| **isTrialing** | **kotlin.Boolean** |  |  |
| **limits** | [**PlanLimits**](PlanLimits.md) |  |  |
| **plan** | **kotlin.String** | Resolved plan id (free/starter/business/enterprise, or a custom override id). |  |
| **planName** | **kotlin.String** |  |  |
| **priceEur** | **kotlin.Double** | Monthly price in EUR; &#x60;-1.0&#x60; &#x3D; custom pricing (enterprise). |  |
| **usage** | [**UsageSnapshot**](UsageSnapshot.md) |  |  |
| **currentPeriodEnd** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |
| **manageUrl** | **kotlin.String** |  |  [optional] |
| **quantity** | **kotlin.Int** |  |  [optional] |
| **status** | **kotlin.String** |  |  [optional] |
| **subscriptionId** | **kotlin.String** |  |  [optional] |
| **trialEndsAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



