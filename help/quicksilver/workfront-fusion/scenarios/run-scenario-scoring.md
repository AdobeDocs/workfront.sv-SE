---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Kör Scenario Scoring Expert i Adobe Workfront Fusion
description: Scenariobedömningsexperten kan hjälpa dig att se till att ditt scenario är konfigurerat på ett sätt som följer bästa praxis. Den kontrollerar ditt scenario och ger rekommendationer om dess struktur och organisation.
author: Becky
feature: Workfront Fusion
exl-id: 144c8dbd-a3e9-4267-b3db-0768dac8f384
source-git-commit: 2b455fb2d3892c6bb796aa7ea57a60c861c3d599
workflow-type: tm+mt
source-wordcount: '314'
ht-degree: 0%

---

# Kör Scenario Scoring Expert i Adobe Workfront Fusion

Scenariobedömningsexperten kan hjälpa dig att se till att ditt scenario är konfigurerat på ett sätt som följer bästa praxis. Den kontrollerar ditt scenario och ger rekommendationer om dess struktur och organisation.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">  
 <col> 
 <col> 
 <tbody> 
  <tr> 
    <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>[!DNL Pro] eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Adobe Workfront Fusion] licens**</td> 
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

Kör scenariobedömningsexperten

1. Klicka på fliken **[!UICONTROL Scenario]** i den vänstra panelen.
1. Välj det scenario där du vill köra scenariobedömningsexperten.
1. Klicka någonstans i scenariot för att öppna Scenarioredigeraren.
1. Klicka på ikonen Scenario Scoring Expert ![Expert för bedömning av scenario](assets/scoring-expert-icon.png) längst ned på skärmen.

   Panelen Scenariobedömningsexpert öppnas.
1. Klicka på **Utvärdera**.

Scenario Scoring Expert returnerar poängen från 10 och visar vilka kontroller som har passerat eller misslyckats. Om en kontroll har misslyckats ger scenariobedömningsexperten rekommendationer för hur man ska se till att scenariot uppfyller dessa kontroller.

![Scenariopoäng](assets/scenario-score.png)

## Bedömningskontroller av scenarier

Scenariobedömningsexperten använder följande kontroller:

* Scenariot måste namnges.
* Alla moduler måste ha en etikett.
* Scenariot måste köras enligt ett angivet schema.

  Instruktioner finns i [Schemalägg ett scenario](/help/quicksilver/workfront-fusion/scenarios/schedule-a-scenario.md).
* Scenens storlek för utkast måste vara mindre än 5 MB.

  Mer information finns i [Förberedelser för Fusion-prestanda](/help/quicksilver/workfront-fusion/get-started/fusion-performance-guardrails.md#scenarios).
* Om en Workfront direktutlösarmodul används måste den filtreras.

  Instruktioner finns i [Händelseprenumerationsfilter i  [!DNL Workfront] > [!UICONTROL Watch Events]-modulen](/help/quicksilver/workfront-fusion/apps-and-their-modules/workfront-modules.md#event-subscription-filters-in-the-workfront--watch-events-module).

