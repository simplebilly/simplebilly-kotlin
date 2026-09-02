
# ApiResponseGdprExportData

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **activityLog** | [**kotlin.collections.List&lt;GdprActivity&gt;**](GdprActivity.md) |  |  |
| **apiKeys** | [**kotlin.collections.List&lt;GdprApiKey&gt;**](GdprApiKey.md) | Key identifiers and names only — never a usable credential. |  |
| **billing** | [**kotlin.collections.List&lt;GdprBillingInfo&gt;**](GdprBillingInfo.md) |  |  |
| **exportedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  |
| **generatedByAi** | **kotlin.Boolean** | Honesty field: this document is a plain data dump, never AI-generated. |  |
| **notifications** | [**kotlin.collections.List&lt;GdprNotification&gt;**](GdprNotification.md) |  |  |
| **refreshTokens** | [**kotlin.collections.List&lt;GdprRefreshToken&gt;**](GdprRefreshToken.md) | Session records: metadata only, never the token hash. |  |
| **tenants** | [**kotlin.collections.List&lt;GdprTenant&gt;**](GdprTenant.md) |  |  |
| **usageEvents** | [**kotlin.collections.List&lt;GdprUsageEvent&gt;**](GdprUsageEvent.md) |  |  |
| **user** | [**GdprUser**](GdprUser.md) |  |  |



