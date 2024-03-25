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

# Visa ett scenario körningshistorik i [!DNL Adobe Workfront Fusion]

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
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>  
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Visa alla körningar av ett scenario

### Visa historik för scenariekörning på [!UICONTROL Scenario Detail] page

1. Klicka på **[!UICONTROL Scenario]** i den vänstra panelen och klicka sedan på scenariot.

   eller

   Om du arbetar med scenariot i scenarioredigeraren klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) nära fönstrets övre vänstra hörn.

1. Visa informationen i listan till höger.

   ![](assets/open-history-tab-350x202.png)

   Du kan också klicka för att se en helsidesvy av den här informationen. I helsidesvyn kan du filtrera historiken för att visa specifika körningar.

   Följande information visas för varje körning av scenariot:

   * Datum när körningen utfördes **[!UICONTROL Started]**
   * **[!UICONTROL Status]** (lyckades eller misslyckades)
   * Kör **[!UICONTROL Duration]**
   * Antal **[!UICONTROL Operations]**
   * Storlek på **[!UICONTROL Data Transfer]**
   * Länka till **[!UICONTROL Details]**

>[!NOTE]
>
>Scenariohistoriken visar en **Bearbetar** emblem bredvid scenarier som nyligen har körts, medan körningsinformationen skrivs till lagringen. Bearbetningen sker omedelbart efter att scenariot har körts. och bör inte vara längre än några minuter. Detaljer om scenariokörningen kanske inte visas när körningen bearbetas.

### Visa historik för scenariekörning på [!UICONTROL History] tab

The [!UICONTROL History] på fliken visas mer information än vad som är tillgängligt på [!UICONTROL Scenario detail] sida. Du kan även filtrera och sortera körningarna på [!UICONTROL History] -fliken.

1. Klicka på **[!UICONTROL Scenario]** i den vänstra panelen och klicka sedan på scenariot.

   eller

   Om du arbetar med scenariot i scenarioredigeraren klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) nära fönstrets övre vänstra hörn.

1. Klicka på **[!UICONTROL History]** -fliken i det övre vänstra hörnet av sidan
1. (Valfritt) Klicka på knappen **[!UICONTROL Details]** länk.

   Mer information om att bearbeta paket finns i [Scenariokörningsflöde i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/scenario-execution-flow.md).

   >[!NOTE]
   >
   >* The [!UICONTROL details] -länken visas bara om körningen har information tillgänglig.
   >
   >* Scenariohistoriken visar en **Bearbetar historik** emblem bredvid scenarier som nyligen har körts, medan körningsinformationen skrivs till lagringen. Bearbetningen sker omedelbart efter att scenariot har körts. och bör inte vara längre än några minuter. Detaljer om scenariokörningen kanske inte visas när körningen bearbetas.

## Filtrera historiken för scenariokörning

Du kan filtrera körningshistoriken så att endast körningar med angivna värden visas.

1. Öppna helsideshistoriken för ett scenario enligt beskrivningen i [Visa historik för scenariekörning på [!UICONTROL History] tab](#view-scenario-execution-history-on-the-history-tab) i den här artikeln.
1. Klicka på [!UICONTROL filter] icon ![](assets/fusion-scenario-filter-icon.png) i kolumnrubriken som du vill filtrera efter.
1. I [!UICONTROL filter] anger du de värden som du vill filtrera efter.
1. Klicka på **[!UICONTROL Save]**.

Filterikonen är orange i kolumner med ett aktivt filter.

## Sortera körningshistoriken för scenarier

Du kan sortera körningshistoriken för scenarier.

1. Öppna helsideshistoriken för ett scenario enligt beskrivningen i [Visa historik för scenariekörning på [!UICONTROL History] tab](#view-scenario-execution-history-on-the-history-tab) i den här artikeln.
1. Klicka på [!UICONTROL Sort] i kolumnrubriken som du vill filtrera efter.
1. Valfritt: Om du vill ändra sorteringsordningen klickar du på [!UICONTROL Sort] ikonen igen.

## Sök i alla körningar av ett scenario

1. Klicka på **[!UICONTROL Scenario]** icon ![](assets/scenarios-icon.png) i den vänstra panelen klickar du på scenariot.

   eller

   Om du arbetar med scenariot i scenarioredigeraren klickar du på vänsterpilen ![](assets/exit-editing-arrow.png) nära fönstrets övre vänstra hörn.

1. Klicka på **[!UICONTROL History]** i skärmens övre vänstra hörn.
1. Klicka **[!UICONTROL Fulltext search]** högst upp i listan över exekveringar.

   eller

   Typ **Ctrl+Skift+F** (Windows) eller **Cmd+Skift+F** (Mac) [!UICONTROL Search in history] öppnas.

1. (Valfritt) Om du vill söka efter körningar som innehåller viss text anger du texten i sökfältet i **[!UICONTROL Search in history]** -fönstret.

   Om du vill söka efter exakt text omger du texten med citattecken (&quot;exempel&quot;).

   >[!INFO]
   >
   >**Exempel:** Om du vill hitta den körning som skapade ett specifikt projekt anger du projekt-ID:t i [!UICONTROL Fulltext search] bar.
   >
   >&quot;625ef2ef0006036bd1794b6e52d737c5&quot;

1. (Valfritt) Om du vill begränsa sökningen efter datumintervall väljer du start- och slutdatum för den önskade sökningen i dialogrutan [!UICONTROL By date range] område.

   >[!NOTE]
   >
   >* Körningar är bara tillgängliga under de senaste 30 dagarna.
   >
   >* [!DNL Workfront Fusion] lagrar webkrocknyttolaster i 30 dagar. Om du får åtkomst till en webkrok-nyttolast mer än 30 dagar efter att den skapades uppstår felet &quot;[!UICONTROL Failed to read file from storage.]&quot;


1. (Valfritt) Om du vill begränsa sökningen efter status väljer du önskad status i dialogrutan **[!UICONTROL By status]** nedrullningsbar meny.


   Tillgängliga statusvärden är:

   * [!UICONTROL All]

   * [!UICONTROL Error]

   * [!UICONTROL Warning]

   * [!UICONTROL Success]

1. (Valfritt) Ändra den ordning som resultatet visas i **[!UICONTROL Sort by dates]** nedrullningsbar meny.

1. (Valfritt) Om du vill kopiera ett scenario-körnings-ID klickar du på **[!UICONTROL Copy execution ID]** icon <img src="assets/copy-fusion-execution-id-icon.png"> i raden för önskad körning

1. (Valfritt) Klicka på ett resultat av [!UICONTROL Fulltext search] för att undersöka scenariomodulens utdatapaket som innehåller informationen.
