
# EmissionEntry

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **activityValue** | **kotlin.String** | Activity amount in &#x60;unit&#x60; (kWh, l, km, t, tkm, EUR). |  |
| **categoryId** | **kotlin.String** | GHG-Protocol category key, e.g. \&quot;purchased_goods\&quot;, \&quot;business_travel\&quot;. |  |
| **description** | **kotlin.String** |  |  |
| **efSource** | **kotlin.String** | Emission-factor source, e.g. \&quot;UBA-2024\&quot;, \&quot;DEFRA-2024\&quot;. |  |
| **efVersion** | **kotlin.String** |  |  |
| **method** | [**EmissionMethod**](EmissionMethod.md) | \&quot;activity\&quot; | \&quot;spend\&quot; | \&quot;supplier\&quot;. |  |
| **scope** | [**GhgScope**](GhgScope.md) | GHG scope: \&quot;1\&quot; | \&quot;2\&quot; | \&quot;3\&quot;. |  |
| **tco2e** | **kotlin.String** | Computed server-side: activity * factor / 1000, rounded to 4 dp. |  |
| **unit** | **kotlin.String** | Unit of the activity value. |  |
| **year** | **kotlin.Int** | Reporting year. |  |
| **updatedAt** | [**java.time.OffsetDateTime**](java.time.OffsetDateTime.md) |  |  [optional] |



