
# PriceTier

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **productId** | [**java.util.UUID**](java.util.UUID.md) | References the product entity. |  |
| **unitPrice** | **kotlin.String** | Net unit price once &#x60;min_quantity&#x60; is reached. |  |
| **customerGroupId** | **kotlin.String** | None &#x3D; tier applies to all customers; otherwise a customer group id. |  [optional] |
| **minQuantity** | **kotlin.Long** | Quantity from which this tier applies (inclusive). |  [optional] |



