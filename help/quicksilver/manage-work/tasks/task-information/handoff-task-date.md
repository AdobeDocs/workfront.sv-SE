---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över datum för aktivitetens leverans
description: Leveransdatumet är det datum då en uppgift blir tillgänglig för arbete. Det innebär vanligtvis att dess föregångare har löst sig och att den som tilldelats uppgiften kan börja arbeta med den.
author: Alina
feature: Work Management
exl-id: caf2dbba-5311-418d-8c82-ddcc256f9926
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '723'
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
>* Complete
>* Död
>

Workfront använder följande regler för att beräkna leveransdatum för en uppgift:

* **När aktiviteten har en ofullständig föregångare**: Ångra-datumet för aktiviteten är null.
* **När aktiviteten har en fullständig föregående**: Leveransdatumet är samma som det faktiska slutförandedatumet för föregående aktivitet. Om föregående aktivitet har en fördröjning beräknar Workfront leveransdatumet för efterföljande uppgift med följande formel:

  `Successor Handoff Date = Predecessor Actual Completion Date + Lag`

  Mer information om fördröjningstid finns i [Översikt över lagertyper](../use-prdcssrs/lag-types.md).

  Om den efterföljande aktiviteten har fler än en föregångare beräknas leveransdatumet utifrån det senaste faktiska slutförandedatumet för föregående aktiviteter. Om till exempel de två föregångarnas faktiska slutförandedatum är den 8 november 2022 och den 20 november 2022 är den efterträdande partens leveransdatum den 20 november 2022.

  >[!NOTE]
  >
  >   Beräkningen av leveransdatumet för en efterföljande aktivitet baserat på det faktiska slutförandedatumet eller en föregående aktivitet är densamma oavsett om föregående aktivitet används eller inte. Mer information om framtvingade föregångare finns i [Tvinga föregångare](../use-prdcssrs/enforced-predecessors.md).


* **När aktiviteten inte har någon föregångare och**:

   * **Det planerade startdatumet har redan infallit**: Leveransdatumet är samma som det planerade startdatumet för projektet om aktiviteten inte har någon obligatorisk begränsning. Om aktiviteter har tvingade begränsningar finns mer information i avsnittet &quot;När aktiviteten har en tvingad begränsning för planerade datum&quot; nedan.
   * **Det planerade startdatumet infaller i framtiden (vilket datum som helst efter det aktuella datumet)**: Leveransdatumet är samma som det planerade startdatumet för aktiviteten om aktiviteten inte har någon obligatorisk begränsning. Om aktiviteter har tvingade begränsningar finns mer information i avsnittet &quot;När aktiviteten har en tvingad begränsning för planerade datum&quot; nedan.

>[!NOTE]
>
>När aktiviteten har en föregångare mellan projekt beräknas överlämningsdatumet för efterföljande endast om något av följande inträffar:
>
>* Du beräknar manuellt om tidslinjen för den efterföljande partens projekt. Du måste ha behörigheten Hantera för projektet för att kunna beräkna om tidslinjen.
>* Tidslinjen för den efterträdande partens projekt beräknas automatiskt om på natten.
>
>Mer information om hur du beräknar om projektets tidslinje finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

* **När aktiviteten har en tvingad begränsning för planerade datum**: Leveransdatumet varierar beroende på begränsningstypen och om aktiviteten har ett faktiskt startdatum eller inte.\
  Följande är obligatoriska begränsningar för uppgifter:

   * Måste börja på
   * Måste avslutas
   * Starta tidigast
   * Starta senast
   * Fast den

  Följande scenarier finns:

   * **När aktiviteten har en begränsning på Måste starta den eller Start inte tidigare än**: Om aktivitetsbegränsningsdatumet redan har infallit och det inte finns något faktiskt startdatum för aktiviteten (aktiviteten har inte startats ännu) är leveransdatumet det närmaste möjliga datumet då aktiviteten kan startas. Om aktiviteten har startats är leveransdatumet lika med startdatumet för projektet.
   * **När aktiviteten har begränsningen Måste avslutas den eller starta inte senare än**: Om aktivitetsvillkorsdatumet är i framtiden och det inte finns något faktiskt startdatum för aktiviteten (aktiviteten har inte startats ännu) är leveransdatumet aktivitetens planerade startdatum. Om det finns som faktiskt startdatum för aktiviteten är datumet för leverans projektets startdatum.
   * **När aktiviteten har en begränsning för fasta datum**: Leveransdatumet är det planerade startdatumet för aktiviteten, oavsett om den har en föregångare eller inte och oavsett om den har slutförts eller inte.

<!--these are old descriptions, edited by Anna As. on August 25, 2023 in this issue - https://experience.adobe.com/#/@adobeinternalworkfront/so:hub-Hub/workfront/issue/64c0032500018fabd4fc484167eb10dc/updates
   * When the task has a constraint of Must Start On or Start No Earlier Than, the Handoff Date is the Constraint date, unless there is an Actual Start Date on the task. If there is an Actual Start Date on the task, the Handoff Date is the Actual Completion Date of the predecessor.
   * When the task has a constraint of Must Finish On or Start No Later Than, the Handoff Date is always the Actual Completion Date of the predecessor, regardless of whether there is an Actual Start Date on the task or not. 
   * When the task has a constraint of Fixed Dates, the Handoff Date is the Planned Start Date of the task, regardless of whether it has a predecessor or not and regardless of whether the predecessor is completed or not.

-->

## Hitta leveransdatumet

Du kan visa datum för leverans för en uppgift i en uppgiftsrapport eller i vyn för en uppgiftslista.\
Mer information om hur du skapar en rapport finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).
