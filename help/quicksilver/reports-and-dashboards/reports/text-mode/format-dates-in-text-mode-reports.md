---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatera datum i textlägesrapporter
description: Datum kan konfigureras för visning i en mängd olika format i rapporter och listor i Adobe Workfront. Om du vill skapa ett datumformat måste du ändra värdeformatraden för textlägeskoden i kolumnen.
author: Nolan
feature: Reports and Dashboards
exl-id: ff0686aa-b306-4954-8f9b-3e98bf8cff22
source-git-commit: 54f4c136cfaaaaaa90a4fc64d3ffd06816cff9cb
workflow-type: tm+mt
source-wordcount: '190'
ht-degree: 1%

---

# Formatera datum i textlägesrapporter

Datum kan konfigureras för visning i en mängd olika format i rapporter och listor i Adobe Workfront. Om du vill skapa ett datumformat måste du ändra `valueformat` raden i textlägeskoden i kolumnen.

`valueformat= [new date format]` Om du t.ex. vill att det beräknade slutförandedatumet ska visas som MM/DD/ÅÅ ser koden ut så här:

```
valueformat=atDate
valuefield=projectedCompletionDate
```

Om du vill visa det planerade slutförandedatumet som *Mth, DD, Year* skulle koden se ut så här:

```
valueformat=mediumAtdate
valuefield=plannedCompletionDate
```

Mer information om hur du använder villkorsstyrd formatering i Workfront-rapporter och -listor i textläge finns i [Använda villkorsstyrd formatering i textläge](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Du kan formatera datum med följande

```
valueformat
```

 värden för textläge:

| **Format** | Exempel  | ***valueFormat=*** |
|---|---|---|
| MM/DD/YY | 10/11/18 | `atDate` |
| MM/DD/YY-tid | 10/11/18 12:00 pm | `longAtDate` |
| MM/DD/YY | 10/11/18 | `shortAtDate` |
| Mth, DD, YR | 11 okt 2018 | `mediumAtDate` |
| DW, Mth, Day, YR | Mån, 11 oktober 2018 | `partialAtDate` |
| DW, Mth, Day, YR Time | Mån, 11 oktober 2018 12:00 | `fullAtDate` |
