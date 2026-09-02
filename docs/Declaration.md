
# Declaration

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **declarationType** | [**DeclarationType**](DeclarationType.md) | Art der Erklärung: \&quot;dcgk\&quot; (Entsprechenserklärung § 161 AktG) oder \&quot;unternehmensfuehrung\&quot; (Erklärung zur Unternehmensführung § 289f HGB). |  [optional] |
| **isCurrent** | **kotlin.Boolean** | Kennzeichnet die aktuell gültige Fassung (max. eine je Mandant). |  [optional] |
| **text** | **kotlin.String** | Inhalt der Erklärung als Markdown. |  [optional] |
| **validFrom** | [**java.time.LocalDate**](java.time.LocalDate.md) | Datum, ab dem die Erklärung gilt. |  [optional] |
| **version** | **kotlin.String** | Versionsbezeichnung der Erklärung (z.B. \&quot;2025-01\&quot;). |  [optional] |



