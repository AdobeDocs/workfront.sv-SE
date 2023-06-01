---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatera tal, valuta och procentvärden i textlägesrapporter
description: Numeriska värden, inklusive valutor, kan konfigureras för visning i olika format i rapporter och listor i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: e1411ce49d8668ba50bcb9b80d4a4b47d0dd00fc
workflow-type: tm+mt
source-wordcount: '154'
ht-degree: 5%

---

# Formatera tal, valuta och procentvärden i textlägesrapporter

Numeriska värden, inklusive valutor, kan konfigureras för visning i olika format i rapporter och listor i Adobe Workfront.

Om du vill ändra formatet för ett numeriskt värde måste du redigera **värdeformat** rad i kolumnen.

Om du till exempel vill visa kolumnen Budget som $1000 ser värdeformatraden ut så här:

```
valueformat=currencyStringCurrencyRounded
valuefield=budget
```

Mer information om hur du använder villkorsstyrd formatering i Workfront-rapporter och -listor i textläge finns i [Använda villkorsstyrd formatering i textläge](../../../reports-and-dashboards/reports/text-mode/use-conditional-formatting-text-mode.md).

Du kan formatera tal med följande värden för `valueformat` rad i kolumnen:

| Exempel | `valueformat=` |
|---|---|
| 1234 | <pre>doubleAsString</pre> <br>eller <br><pre>int</pre> |
| 1,234 | <pre>doubleAsInt</pre> |
| $1,234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234.56 | <pre>doubleAsDouble</pre> |
| $1,234.56 | <pre>currencyStringCurrency</pre> |
| 12% | <pre>doubleAsPercentRounded</pre> |
| 12.34% | <pre>doubleAsPercent</pre> |
| (1,234.56) | <pre>doubleAsFinancial</pre> |
| (1,234) | <pre>doubleAsFinancialRounded</pre> |

