---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över datum för aktivitetsleverans
description: Leveransdatumet är det datum då en uppgift blir tillgänglig för arbete. Det innebär vanligtvis att dess föregångare har löst sig och att den som tilldelats uppgiften kan börja arbeta med den.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 39efbf1d678cf85e9b6b61744fb046664992370c
workflow-type: tm+mt
source-wordcount: '476'
ht-degree: 0%

---

# Översikt över datum för aktivitetsleverans

Leveransdatumet är det datum då en uppgift blir tillgänglig för arbete. Det innebär vanligtvis att dess föregångare har löst sig och att den som tilldelats uppgiften kan börja arbeta med den.

>[!TIP]
>
>Leveransdatum finns inte för utgåvor och projekt.

## Hur Adobe Workfront beräknar leveransdatumet

>[!NOTE]
>
>Leveransdatumet beräknas bara om projektstatusen är lika med följande statusvärden:
>
>* Parkerad
>* Aktuell
>* Slutförd
>* Död
>


Workfront använder följande regler för att beräkna leveransdatum för en uppgift:

* **När aktiviteten har en ofullständig föregångare**: Leveransdatumet för aktiviteten är null.
* **När aktiviteten har en fullständig föregångare**: Leveransdatumet är samma som det faktiska slutförandedatumet för föregående aktivitet. Om föregående aktivitet har en fördröjning beräknar Workfront leveransdatumet för efterföljande uppgift med följande formel:

   `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

   Mer information om fördröjningstid finns i [Översikt över lagertyper](../use-prdcssrs/lag-types.md).

   Om den efterföljande aktiviteten har fler än en föregångare beräknas leveransdatumet utifrån det senaste faktiska slutförandedatumet för föregående aktiviteter. Om till exempel de två föregångarnas faktiska slutförandedatum är den 8 november 2022 och den 20 november 2022 är den efterträdande partens leveransdatum den 20 november 2022.

   >[!NOTE]
   >
   >   Beräkningen av leveransdatumet för en efterföljande aktivitet baserat på det faktiska slutförandedatumet eller en föregående aktivitet är densamma oavsett om föregående aktivitet används eller inte. Mer information om framtvingade föregångare finns i [Tvinga föregående](../use-prdcssrs/enforced-predecessors.md).


* **När aktiviteten inte har någon föregångare och**:

   * **Det planerade startdatumet har redan infallit**: Leveransdatumet är samma som projektets planerade startdatum.
   * **Det planerade startdatumet infaller i framtiden (vilket datum som helst efter det aktuella datumet)**: Leveransdatumet är samma som projektets planerade startdatum.

>[!NOTE]
>
>När aktiviteten har en föregångare mellan projekt beräknas överlämningsdatumet för efterföljande endast om något av följande inträffar:
>
>* Du beräknar manuellt om tidslinjen för den efterföljande partens projekt. Du måste ha behörigheten Hantera för projektet för att kunna beräkna om tidslinjen.
>* Tidslinjen för den efterträdande partens projekt beräknas automatiskt om på natten.
>
>Mer information om hur du beräknar om projektets tidslinje finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **När aktiviteten har en tvingad begränsning för planerade datum**: Leveransdatumet är alltid detsamma som datumet som anges av villkoret, oavsett andra villkor.\
   Följande är obligatoriska begränsningar för uppgifter:

   * Måste börja på
   * Måste avslutas
   * Starta tidigast
   * Starta inte senare än
   * Fast den

## Hitta leveransdatumet

Du kan visa datum för leverans för en uppgift i en uppgiftsrapport eller i vyn för en uppgiftslista.\
Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
