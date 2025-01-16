---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatera tal, valuta och procentvärden i textlägesrapporter
description: Numeriska värden, inklusive valutor, kan konfigureras för visning i olika format i rapporter och listor i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 9caac488522d2a12d3bdf4bf23ba7e44c6dbf7d2
workflow-type: tm+mt
source-wordcount: '145'
ht-degree: 2%

---

# Formatera tal, valuta och procentvärden i textlägesrapporter

<!-- Audited: 1/2025 -->

Numeriska värden, inklusive valutor, kan konfigureras för visning i olika format i rapporter och listor i Adobe Workfront.

Om du vill ändra formatet för ett numeriskt värde måste du redigera raden **värdeformat** i kolumnen.

Om du till exempel vill visa kolumnen Budget som $1000 ser värdeformatraden ut så här:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Mer information om hur du använder villkorsstyrd formatering i Workfront-rapporter och -listor i textläge finns i [Använda villkorsstyrd formatering i textläge](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Du kan formatera tal med följande värden för raden `valueformat` i kolumnen:

| Exempel | `valueformat=` |
|---|---|
| 1234 | `doubleAsString`<br>eller<br>`int` |
| 1 234 | `doubleAsInt` |
| $1 234 | `currencyStringCurrencyRounded` |
| 1234,56 | `doubleAsDouble` |
| 1 234,56 USD | `currencyStringCurrency` |
| 12 % | `doubleAsPercentRounded` |
| 12,34 % | `doubleAsPercent` |
| (1 234,56) | `doubleAsFinancial` |
| (1 234) | `doubleAsFinancialRounded` |

