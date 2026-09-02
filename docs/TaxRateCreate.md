
# TaxRateCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **countryCode** | **kotlin.String** | ISO 3166-1 alpha-2 country code. |  |
| **isDefault** | **kotlin.Boolean** | Default rate for the country (one per country); fallback for lookups when no dated rate applies. |  |
| **name** | **kotlin.String** | Human name, e.g. \&quot;VAT\&quot;. |  |
| **ratePercent** | **kotlin.Long** | Rate in hundredths of a percent: 1900 &#x3D; 19.00%. |  |
| **effectiveFrom** | [**java.time.LocalDate**](java.time.LocalDate.md) | Date this rate took effect; &#x60;None&#x60; &#x3D; not date-bound. |  [optional] |



