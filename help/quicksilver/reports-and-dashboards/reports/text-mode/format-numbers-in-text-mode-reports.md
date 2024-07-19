---
product-area: reporting
navigation-topic: text-mode-reporting
title: Formatera tal, valuta och procentvärden i textlägesrapporter
description: Numeriska värden, inklusive valutor, kan konfigureras för visning i olika format i rapporter och listor i Adobe Workfront.
author: Nolan
feature: Reports and Dashboards
exl-id: 965f5dcd-4844-4792-9fd0-a47814a325a4
source-git-commit: 8de9c79f6c62b74a652482ec10bf38fada8c5fc8
workflow-type: tm+mt
source-wordcount: '155'
ht-degree: 1%

---

# Formatera tal, valuta och procentvärden i textlägesrapporter

<!-- Audited: 2/2024 -->

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
| 1234 | <pre>doubleAsString</pre> <br>eller <br><pre>int</pre> |
| 1 234 | <pre>doubleAsInt</pre> |
| $1 234 | <pre>currencyStringCurrencyRounded</pre> |
| 1234,56 | <pre>doubleAsDouble</pre> |
| 1 234,56 USD | <pre>currencyStringCurrency</pre> |
| 12 % | <pre>doubleAsPercentRounded</pre> |
| 12,34 % | <pre>doubleAsPercent</pre> |
| (1 234,56) | <pre>doubleAsFinancial</pre> |
| (1 234) | <pre>doubleAsFinancialRounded</pre> |

