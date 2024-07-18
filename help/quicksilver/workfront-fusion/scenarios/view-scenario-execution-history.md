---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Visa ett scenarios körningshistorik i Adobe Workfront Fusion
description: Du kan visa information om alla körningar för ett scenario eller söka efter specifika data i alla körningar i scenariot.
author: Becky
feature: Workfront Fusion
exl-id: cc2c3f87-34dc-4a06-9f5f-1a7fb10a3b82
source-git-commit: ae57c38149bf6db3bbbb471fad8f3567b7d712a7
workflow-type: tm+mt
source-wordcount: '881'
ht-degree: 0%

---

# Visa ett scenarios körningshistorik i [!DNL Adobe Workfront Fusion]

Du kan visa information om alla körningar för ett scenario eller söka efter specifika data i alla körningar i scenariot.

Ett scenario körningshistorik visar alla körningar i ett scenario under de senaste 30 dagarna.

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
  <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visa alla körningar av ett scenario

### Visa historik för scenariokörning på sidan [!UICONTROL Scenario Detail]

1. Klicka på fliken **[!UICONTROL Scenario]** i den vänstra panelen och klicka sedan på scenariot.

   eller

   Om du arbetar med scenariot i scenarioredigeraren klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) i fönstrets övre vänstra hörn.

1. Visa informationen i listan till höger.

   ![](assets/open-history-tab-350x202.png)

   Du kan också klicka för att se en helsidesvy av den här informationen. I helsidesvyn kan du filtrera historiken för att visa specifika körningar.

   Följande information visas för varje körning av scenariot:

   * Datum när körningen var **[!UICONTROL Started]**
   * **[!UICONTROL Status]** (lyckades eller misslyckades)
   * Kör **[!UICONTROL Duration]**
   * Antal **[!UICONTROL Operations]**
   * Storlek på **[!UICONTROL Data Transfer]**
   * Länka till **[!UICONTROL Details]**

>[!NOTE]
>
>Scenhistoriken visar ett **Bearbetningsemblem** bredvid scenarier som nyligen har körts, medan körningsinformationen skrivs till lagringen. Bearbetningen sker omedelbart efter att scenariot har körts. och bör inte vara längre än några minuter. Detaljer om scenariokörningen kanske inte visas när körningen bearbetas.

### Visa historik för scenariokörning på fliken [!UICONTROL History]

Fliken [!UICONTROL History] visar fler detaljer än vad som är tillgängligt på sidan [!UICONTROL Scenario detail]. Du kan även filtrera och sortera körningarna på fliken [!UICONTROL History].

1. Klicka på fliken **[!UICONTROL Scenario]** i den vänstra panelen och klicka sedan på scenariot.

   eller

   Om du arbetar med scenariot i scenarioredigeraren klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) i fönstrets övre vänstra hörn.

1. Klicka på fliken **[!UICONTROL History]** i sidans övre vänstra hörn
1. (Valfritt) Klicka på länken **[!UICONTROL Details]** om du vill ha detaljerad information om en vald scenariokörning, inklusive vilka paket som har bearbetats.

   Mer information om att bearbeta paket finns i [Körningsflöde för scenarier i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* Länken [!UICONTROL details] är bara synlig om körningen har tillgängliga detaljer.
   >
   >* Scenhistoriken visar ett **Bearbetningshistorik** bredvid scenarier som nyligen har körts, medan körningsinformationen skrivs till lagringen. Bearbetningen sker omedelbart efter att scenariot har körts. och bör inte vara längre än några minuter. Detaljer om scenariokörningen kanske inte visas när körningen bearbetas.

## Filtrera historiken för scenariokörning

Du kan filtrera körningshistoriken så att endast körningar med angivna värden visas.

1. Öppna helsideshistoriken för ett scenario enligt beskrivningen i [Visa historik för scenariokörning på fliken [!UICONTROL History] ](#view-scenario-execution-history-on-the-history-tab) i den här artikeln.
1. Klicka på ikonen [!UICONTROL filter] ![](assets/fusion-scenario-filter-icon.png) i kolumnrubriken som du vill filtrera efter.
1. Ange de värden som du vill filtrera efter i dialogrutan [!UICONTROL filter].
1. Klicka på **[!UICONTROL Save]**.

Filterikonen är orange i kolumner med ett aktivt filter.

## Sortera körningshistoriken för scenarier

Du kan sortera körningshistoriken för scenarier.

1. Öppna helsideshistoriken för ett scenario enligt beskrivningen i [Visa historik för scenariokörning på fliken [!UICONTROL History] ](#view-scenario-execution-history-on-the-history-tab) i den här artikeln.
1. Klicka på ikonen [!UICONTROL Sort] i kolumnrubriken som du vill filtrera efter.
1. Valfritt: Om du vill ändra sorteringsordningen klickar du på ikonen [!UICONTROL Sort] igen.

## Sök i alla körningar av ett scenario

1. Klicka på ikonen **[!UICONTROL Scenario]** ![](assets/scenarios-icon.png) i den vänstra panelen och klicka sedan på scenariot.

   eller

   Om du arbetar med scenariot i scenarioredigeraren klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) i fönstrets övre vänstra hörn.

1. Klicka på fliken **[!UICONTROL History]** i skärmens övre vänstra hörn.
1. Klicka på **[!UICONTROL Fulltext search]** högst upp i listan över körningar.

   eller

   Skriv **Ctrl+Skift+F** (Windows) eller **Cmd+Skift+F** (Mac)
Fönstret [!UICONTROL Search in history] öppnas.

1. (Valfritt) Om du vill söka efter körningar som innehåller specifik text anger du texten i sökfältet i fönstret **[!UICONTROL Search in history]**.

   Om du vill söka efter exakt text omger du texten med citattecken (&quot;exempel&quot;).

   >[!INFO]
   >
   >**Exempel:** Om du vill hitta den körning som skapade ett visst projekt anger du projekt-ID:t i fältet [!UICONTROL Fulltext search].
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Valfritt) Om du vill begränsa sökningen efter datumintervall markerar du start- och slutdatum för den önskade sökningen i området [!UICONTROL By date range].

   >[!NOTE]
   >
   >* Körningar är bara tillgängliga under de senaste 30 dagarna.
   >
   >* [!DNL Workfront Fusion] lagrar webkrocknyttolaster i 30 dagar. Om du får åtkomst till en webkrok-nyttolast mer än 30 dagar efter att den skapades uppstår felet [!UICONTROL Failed to read file from storage.]


1. (Valfritt) Om du vill begränsa sökningen efter status väljer du önskad status i listrutan **[!UICONTROL By status]**.


   Tillgängliga statusvärden är:

   * [!UICONTROL All]

   * [!UICONTROL Error]

   * [!UICONTROL Warning]

   * [!UICONTROL Success]

1. (Valfritt) Ändra den ordning som resultatet visas i listrutan **[!UICONTROL Sort by dates]**.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Copy execution ID]** om du vill kopiera ett scenario-körnings-ID <img src="assets/copy-fusion-execution-id-icon.png"> i raden för önskad körning

1. (Valfritt) Klicka på resultatet av [!UICONTROL Fulltext search] för att undersöka scenariomodulens utdatapaket som innehåller informationen.
