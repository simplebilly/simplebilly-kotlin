
# ShippingRuleCreate

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **name** | **kotlin.String** | Delivery-method label, e.g. \&quot;Standardversand\&quot;. |  |
| **price** | **kotlin.String** | Shipping cost in the shop&#39;s currency. |  |
| **carrier** | **kotlin.String** | Provider that auto-filled this rule (e.g. \&quot;ups\&quot;), if any. |  [optional] |
| **country** | [**CountryCode**](CountryCode.md) | None &#x3D; applies to all countries. |  [optional] |
| **deliveryTime** | **kotlin.String** | Delivery time text, e.g. \&quot;1-3\&quot;. |  [optional] |
| **isActive** | **kotlin.Boolean** |  |  [optional] |
| **maxWeightKg** | **kotlin.Double** |  |  [optional] |
| **minWeightKg** | **kotlin.Double** |  |  [optional] |
| **notes** | **kotlin.String** |  |  [optional] |
| **priority** | **kotlin.Int** | Lower wins when multiple rules match. |  [optional] |



