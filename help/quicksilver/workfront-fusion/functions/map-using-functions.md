---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mappa objekt med funktioner i  [!DNL Adobe Workfront Fusion]
description: När du mappar objekt kan du använda funktioner för att skapa enkla eller komplexa formler.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: d175a3d43f13338661d8b7e1cb79038a36522ff9
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Mappa objekt med funktioner i [!DNL Adobe Workfront Fusion]

När du mappar objekt kan du använda funktioner för att skapa enkla eller komplexa formler. De funktioner som är tillgängliga i [!DNL Adobe Workfront Fusion] liknar funktioner i Excel och i vissa programmeringsspråk:

* De utvärderar allmän logik, matematik, text, datum och arrayer.
* Med dem kan du utföra villkorsstyrd logik och omformningar av objektvärden, som att konvertera text till versaler, trimma text, konvertera ett datum till ett annat format och mycket mer.

Mer information finns i [Mappa information från en modul till en annan i Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).


## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">

<col>  
 <col>  
 <tbody>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>  
   <td> <p>Alla</p> </td>  
  </tr>  
  <tr data-mc-conditions="">  
   <td role="rowheader">[!DNL Adobe Workfront] licens</td>  
   <td> <p>Nytt: [!UICONTROL Standard]</p><p>eller</p><p>Aktuell: [!UICONTROL Work] eller högre</p> </td>  
  </tr>  
  <tr>  
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td>  
   <td> 
   <p>Aktuell: Inga [!DNL Workfront Fusion]-licenskrav.</p> 
   <p>eller</p> 
   <p>Äldre: Alla </p> 
   </td>  
  </tr>  
  <tr>  
   <td role="rowheader">Produkt</td>  
   <td> 
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Planen [!DNL Workfront Fusion] ingår.</li></ul> 
   <p>eller</p> 
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p> 
   </td>  
  </tr> 
 </tbody>  
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).


## Översikt över mappningsfliken

Så här öppnar du panelen [!UICONTROL mapping] för ett fält:

1. Klicka på **Scenarier** i den vänstra panelen.
1. Välj ett scenario.

![](assets/open-functions-bar.png)


### Flikar på mappningspanelen

Följande är flikar på mappningspanelen:

* **Allmänna funktioner** ![](assets/toolbar-icon-general-function.png) - Mer information finns i [Allmänna funktioner i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md).

* **Matematiska funktioner** ![](assets/toolbar-icon-math-functions.png) - Mer information finns i [Matematiska funktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md).

* **Text och binära funktioner** ![](assets/toolbar-icon-text&binary-functions.png) - Mer information finns i [Strängfunktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md).

* **Datum och tid** ![](assets/toolbar-icon-date&time-functions.png) - Se [Datum- och tidsfunktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) och artiklarna nedan för mer information:

   * [Tokens för datum- och tidsformatering i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Tokens för datum- och tidsanalys i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktioner för att arbeta med arrayer** ![](assets/toolbar-icon-functions-for-arrays.png) - Mer information finns i [Arrayfunktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md).

* **Mappa andra funktioner** ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) visar objekt som du kan mappa från andra moduler. Den här fliken är inte alltid tillgänglig.

![](assets/functions-toolbar-350x189.png)

## Infoga funktioner i fält

Så här infogar du en funktion i ett fält:

1. Klicka på funktionsnamnet.

   eller

   Dra funktionen till fältet.


>[!BEGINSHADEBOX]

**Exempel:** En del datatyper hindrar användare från att ange fler än ett visst antal tecken. Du kan använda delsträngsfunktionen för att begränsa ett värde till ett visst antal tecken.

I det här exemplet begränsar delsträngsfunktionen projektnamnet till 50 tecken.

![](assets/example-meet-length-restriction-350x184.png)

>[!ENDSHADEBOX]

## Kapslingsfunktioner

Du kan kapsla in funktioner i varandra.

## Använd [!DNL Google Sheets]-funktioner

Om [!DNL Workfront Fusion] inte innehåller någon funktion som du vill använda, men den finns i [!DNL Google Sheets], kan du använda den genom att följa de här stegen:

1. Skapa ett nytt tomt kalkylblad i [!DNL Google Sheets].
1. Öppna ditt scenario i [!DNL Workfront Fusion].
1. Lägg till modulen **[!DNL Google Sheets]** >**[!UICONTROL Update a cell]** i scenariot.

   Instruktioner om hur du lägger till en modul finns i [Lägga till en modul i ett scenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) i artikeln [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Konfigurera modulen:

   1. Välj det nya kalkylbladet i fältet **[!UICONTROL Spreadsheet]**.
   1. Infoga formeln som innehåller [!DNL Google Sheets] funktioner i fältet **[!UICONTROL Value]**.

      Du kan använda utdata från föregående moduler som vanligt.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Infoga modulen **[!UICONTROL Google Sheets]>[!UICONTROL Get a cell]** för att få fram det beräknade resultatet.
1. Konfigurera modulen med samma cell-ID som du använde i steg 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
