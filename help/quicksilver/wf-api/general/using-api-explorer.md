---
content-type: api
navigation-topic: general-api
title: Använda API Explorer
description: Använda API Explorer
author: Becky
feature: Workfront API
role: Developer
exl-id: dcb7dadb-4dd8-48da-a559-cbe8ad99ff9e
source-git-commit: 494c7bf8aaf3570d4a01b5e88b85410ee3f52f18
workflow-type: tm+mt
source-wordcount: '362'
ht-degree: 0%

---


# Använda API Explorer

När du använder API:t Adobe Workfront Core är API Explorer ett äldre referensverktyg som katalogiserar relationerna mellan resurser, parametrar och variabler som stöds.

## Öppna API Explorer:

1. Använd en webbläsare för att navigera till [API-utforskaren](https://developer.adobe.com/workfront/api-explorer/)\
   ![Navigera till API-utforskaren](assets/mceclip1-350x149.png)

1. I det övre högra hörnet av API-utforskaren väljer du önskad **API-version** för Workfront. Som standard markeras den senaste versionen automatiskt
1. Fältet **Filter** kan användas för att filtrera objekten listade efter namn och kommer att trunkera listan med objekt som visas i enlighet med detta:

   ![API Explorer-fält](assets/mceclip2-350x147.png)

   * **Fält**: Tillgängliga fält i det angivna objektet.
   * **Referenser**: Tillgängliga referensvariabler för det angivna objektet. En referens är ett alias för en variabel. När en referens har initierats kan den användas omväxlande med variabelnamnet. En referens använder initierat minne.
   * **Samlingar**: Tillgängliga samlingar för objektet. Samlingar är variabler som representerar en 1:N-relation mellan objektet och resursen.
   * **Sök**: Tillgängliga sökresurser för objektet. Resultatet av en sökning baseras på de frågeparametrar som anges av sökresursen i API-begäran.
   * **Åtgärder**: Funktioner som stöds för objektet. Åtgärder kan vara enkla eller komplexa procedurer som körs mot en resurs eller uppsättning resurser. En viss åtgärd kan också påverka relaterade resurser.

1. Öppna en flik och klicka sedan på objekt-ID:t för att visa tillämpliga variabler.\
   ![Visa variabler](assets/approval-350x89.png)\
   Beroende på vilket objekt som valts kan följande variabler användas:

   | Variabel | Definition |
   |---|---|
   | Fältnamn | Namnet på ett fält som används i en åtgärd i Workfront API. |
   | Fälttyp | Den typ av värden som kan anges i ett specifikt fält i en datatabell. Möjliga fälttypsvärden är string, double, int, dateTime. |
   | Uppräknad typ | Den typ av värden som kan användas för att identifiera en datatyp. |
   | Möjliga värden | Godtagbara värden för objektet. |
   | Attributtyp ObjCode | Attribut som kan användas för att ändra objektklassen. |
   | URL | Den startsökväg som gör att din app kan kommunicera med Workfront API. |
   | Argument | Objektets variabler som kan skickas mellan programmet och Workfront. |
   | Resultattyp | Tillåtna datatyper som kan returneras från en metod. |
