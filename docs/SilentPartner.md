
# SilentPartner

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **instrumentType** | [**InstrumentType**](InstrumentType.md) | Instrument: \&quot;typisch\&quot; | \&quot;atypisch\&quot; | \&quot;partiarisches_darlehen\&quot; | \&quot;genussrecht\&quot;. |  |
| **contractDate** | [**java.time.LocalDate**](java.time.LocalDate.md) | Datum des Vertragsabschlusses. |  [optional] |
| **einlage** | **kotlin.String** | Einlage (§ 230 HGB). |  [optional] |
| **gewinnquotePct** | **kotlin.String** | Gewinnbeteiligungsquote in Prozent (§ 231 HGB). |  [optional] |
| **gewinnvortrag** | **kotlin.String** | Nicht erhobene Gewinne (§ 232 Abs. 3 HGB). |  [optional] |
| **kestPflichtig** | **kotlin.Boolean** | 25 % Kapitalertragsteuer einbehalten (§ 43 Abs. 1 Nr. 3 EStG; typisch + partiarisches Darlehen). |  [optional] |
| **name** | **kotlin.String** | Name des stillen Gesellschafters. |  [optional] |
| **notes** | **kotlin.String** | Freitext-Notizen. |  [optional] |
| **verlustVerrechnungskonto** | **kotlin.String** | Kumulierte Verluste gegen die Einlage (§ 232 Abs. 2 HGB, ≤ Einlage). |  [optional] |
| **verlustbeteiligung** | **kotlin.Boolean** | Verlustbeteiligung (§ 231 Abs. 2 HGB; kann ausgeschlossen werden). |  [optional] |



