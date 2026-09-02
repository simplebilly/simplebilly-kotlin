
# AttachmentVersion

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **attachmentId** | [**java.util.UUID**](java.util.UUID.md) | Parent attachment whose history this row records. |  |
| **fileName** | **kotlin.String** | Storage key of this version&#39;s bytes. |  |
| **versionNumber** | **kotlin.Int** | 1-based; ascending per attachment in upload order. |  |
| **fileSize** | **kotlin.Long** |  |  [optional] |
| **mimeType** | **kotlin.String** |  |  [optional] |
| **originalName** | **kotlin.String** |  |  [optional] |
| **sha256Hash** | **kotlin.String** |  |  [optional] |
| **uploadedBy** | [**java.util.UUID**](java.util.UUID.md) |  |  [optional] |



