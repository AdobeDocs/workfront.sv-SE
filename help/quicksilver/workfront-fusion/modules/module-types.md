---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Typer av moduler
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 58b4aa76-6c4c-47fc-a42c-c5286da5633a
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '976'
ht-degree: 0%

---

# Typer av moduler

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Modulöversikt](https://experienceleague.adobe.com/docs/workfront-fusion/using/get-started-with-fusion/understand-workfront-fusion/module-overview.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

A[!UICONTROL dobe Workfront Fusion] skiljer ut fem typer av moduler: åtgärdsmoduler, sökmoduler, utlösarmoduler, aggregatorer och iteratorer. Aggregatorer och iteratorer är för avancerade scenarier.

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både Adobe Workfront Fusion och Adobe Workfront för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Åtgärdsmoduler

Åtgärdsmoduler är den vanligaste typen av modul. En vanlig åtgärdsmodul returnerar ett enskilt paket som sedan skickas vidare till nästa modul för bearbetning.

Till skillnad från utlösarmoduler kan åtgärdsmoduler placeras i början, mitten eller slutet av ett scenario. Scenarier kan innehålla ett obegränsat antal åtgärdsmoduler.

>[!INFO]
>
>**Exempel:**
>
>* **[!DNL Workfront]>[!UICONTROL Upload a file]** skickar en fil till [!DNL Workfront] och returnerar dess identifierare.
>* **[!UICONTROL Image]>[!UICONTROL Resize]** tar emot en bild, ändrar storlek på den till angivna mått och överför den storleksändrade bilden till nästa åtgärd.

Åtgärdstypen har fyra undertyper: Skapa, Läs, Uppdatera och Ta bort. Undertypen Uppdatera gör att du kan utföra följande tre åtgärder:

* **Radera innehållet i ett fält**. Den här åtgärden utförs när innehållet i fältet utvärderas för att radera nyckelord (ska inte blandas ihop med *empty*).

  ![](assets/erase-content-of-field.png)

* **Ändra inte innehållet i ett fält**. Den här åtgärden utförs när fältet lämnas tomt eller innehållet i fältet utvärderas till tomt (representeras med null i JSON).

  ![](assets/leave-content-field-unchanged-350x231.png)

* **Ersätt innehållet i ett fält**. Denna operation äger rum i alla andra fall än de som beskrivs ovan.

>[!NOTE]
>
>* Om du inte ser nyckelordet `erase` på mappningspanelen är modulen inte en uppdateringsmodul eller så har den inte uppdaterats till de senaste specifikationerna för appen.
>* [!UICONTROL Empty] ändrar inte fältinnehållet. Om du behöver radera fältet kan du använda följande formel:
>
>![](assets/formula-ifempty-name-erase.png)
>
>Det går för närvarande inte att lämna ett fält oförändrat när dess innehåll utvärderas som tomt.

## Sökmoduler

En vanlig sökning returnerar noll, ett eller flera paket, som sedan skickas vidare till nästa modul för bearbetning.

Du kan placera sökningar i början, mitten eller slutet av ett scenario.

Scenarier kan innehålla ett obegränsat antal sökningar.

>[!INFO]
>
>**Exempel:**
>
>**[!DNL Workfront]>[!UICONTROL Read Related Records]** läser poster som matchar den sökfråga du anger, i ett visst överordnat objekt

## Utlösarmoduler

Utlösare genererar paket när en viss tjänst har ändrats. Ändringen kan vara att skapa nya poster, ta bort poster, uppdatera poster och så vidare.

Varje utlösare kan returnera noll, ett eller flera paket som sedan skickas vidare till nästa modul för bearbetning.

Utlösare kan bara placeras i början av ett scenario.

Varje scenario kan bara innehålla en utlösare.

[!DNL Workfront Fusion] skiljer mellan två typer av utlösare: avsökningsutlösare och direktutlösare.

### Avsökningsutlösare

Avsökningsutlösare avsöker regelbundet en viss tjänst även om det inte har skett någon förändring sedan den föregående körningen. Vi rekommenderar att du schemalägger ett scenario som innehåller en avsökningsutlösare som körs med regelbundna intervall. Om det finns en *ändring* returnerar utlösaren paket som innehåller information om ändringen. Om det inte finns någon *change* returnerar utlösaren inga paket. Instruktioner om hur du schemalägger ett scenario finns i [Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/schedule-a-scenario.md).

Med avsökningsutlösare kan du välja det första paket som de ska skicka via epokpanelen. Panelen visas automatiskt när du har sparat en utlösare eller ändrat utlösarinställningarna. Mer information finns i [Välja var en utlösarmodul ska börja i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/choose-where-trigger-module-starts.md).

>[!NOTE]
>
>Inställningarna som görs på epokpanelen påverkar bara den första körningen av modulen. När modulen har körts kommer den ihåg det senaste utdatapaketet och annullerar inställningarna som gjorts via epokpanelen.

>[!INFO]
>
>**Exempel:**
>
>* **[!DNL Workfront]>[!UICONTROL Watch records]** returnerar filer som nyligen har lagts till sedan scenariot kördes senast
>
>* **[!DNL Google Sheets]>[!UICONTROL Watch Rows]** returnerar nya rader som har lagts till av användaren sedan scenariot kördes senast

### Direktutlösare

Direktutlösare gör att tjänsten omedelbart kan meddela [!DNL Workfront Fusion] om en *ändring*. Vi rekommenderar att du schemalägger ett scenario som innehåller en direktutlösare som körs omedelbart. Instruktioner finns i [Schemalägg ett scenario i Adobe Workfront Fusion](../../workfront-fusion/scenarios/schedule-a-scenario.md). Se även [Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/webhooks/instant-triggers-webhooks.md) för mer information om hur inkommande data hanteras.

>[!INFO]
>
>**Exempel:**
>
>* **[!DNL Workfront]>[!UICONTROL Watch Events]** returnerar information när en viss typ av händelse inträffar i Workfront, till exempel när en uppgift skapas.
>* **[!DNL Google Sheets]>[!UICONTROL Watch Changes]** returnerar information när en cell uppdateras.

## Aggregatorer

En aggregator är en typ av modul som samlar flera paket i ett enda paket.

Varje aggregator returnerar bara ett paket som sedan skickas vidare till nästa modul för vidare bearbetning.

Du kan bara placera aggregerare mitt i ett scenario.

Scenarier kan innehålla ett obegränsat antal aggregerare.

>[!INFO]
>
>**Exempel:**
>
>* **[!UICONTROL Archive]>[!UICONTROL Create an archive]** komprimerar mottagna filer till ett zip-arkiv
>* **[!UICONTROL CSV]>[!UICONTROL Aggregate to CSV]** sammanfogar flera strängar från en CSV-fil till en enda rad
>* **[!UICONTROL Tools]>[!UICONTROL Text aggregator]** kombinerar flera strängar till en enda sträng

Mer information finns i [Aggregatormodulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

## Iteratorer

En iterator är en typ av modul som delar upp arrayer i flera separata paket.

Varje iterator returnerar ett eller flera paket som sedan skickas till nästa modul för bearbetning.

Du kan bara placera iteratorer mitt i ett scenario.

Scenarier kan innehålla ett obegränsat antal iteratorer.

>[!INFO]
>
>**Exempel:**
>
>**[!UICONTROL Email]>[!UICONTROL Retrieve attachments]** bryter en array med bilagor i separata paket

Mer information finns i [Interpolatormodulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/iterator-module.md) och [Mappa en array i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-an-array.md).
