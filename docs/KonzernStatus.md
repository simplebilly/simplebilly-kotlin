
# KonzernStatus

## Properties
| Name | Type | Description | Notes |
| ------------ | ------------- | ------------- | ------------- |
| **groessenbefreit** | **kotlin.Boolean** |  |  |
| **kapitalmarktorientiert** | **kotlin.Boolean** |  |  |
| **konzernabschlusspflicht** | **kotlin.Boolean** |  |  |
| **missingGroupFigures** | **kotlin.Boolean** | Keine group_figures-Zeile für das Jahr vorhanden → keine Größenbefreiung. |  |
| **mutterunternehmen** | **kotlin.Boolean** | Mutterunternehmen: mindestens eine beherrschte Beteiligung (§ 290 Abs. 1 HGB). |  |
| **participations** | [**kotlin.collections.List&lt;KonzernBeteiligung&gt;**](KonzernBeteiligung.md) |  |  |
| **thresholds** | [**KonzernThresholds**](KonzernThresholds.md) |  |  |
| **year** | **kotlin.Int** |  |  |
| **zwischenholdingBefreit** | **kotlin.Boolean** |  |  |
| **parentName** | **kotlin.String** | Mutterunternehmen für die Zwischenholding-Befreiung (§ 291 HGB). |  [optional] |
| **parentSitus** | **kotlin.String** |  |  [optional] |
| **zwischenholdingHinweis** | **kotlin.String** | Hinweis zu den § 291-Voraussetzungen (EU/EWR-Sitz, geprüfter Konzernabschluss). |  [optional] |



