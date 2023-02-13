---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Mappa objekt med funktioner i [!DNL Adobe Workfront Fusion]
description: När du mappar objekt kan du använda funktioner för att skapa enkla eller komplexa formler.
author: Becky
feature: Workfront Fusion
exl-id: e64d9b1e-8576-43db-ac29-0d386a482fbc
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '467'
ht-degree: 0%

---

# Mappa objekt med funktioner i [!DNL Adobe Workfront Fusion]

När du mappar objekt kan du använda funktioner för att skapa enkla eller komplexa formler.

Tillgängliga funktioner i [!DNL Adobe Workfront Fusion] liknar funktioner i Excel och i vissa programmeringsspråk. De utvärderar allmän logik, matematik, text, datum och arrayer. Med dem kan du utföra villkorsstyrd logik och omformningar av objektvärden, som att konvertera text till versaler, trimma text, konvertera ett datum till ett annat format och mycket mer. Mer information finns i [Mappa information från en modul till en annan i Adobe Workfront Fusion](../../workfront-fusion/mapping/map-information-between-modules.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Infoga funktioner i fält

Om du klickar på ett fält visas [!UICONTROL mapping] visas. Mappningspanelen innehåller flera flikar:

![](assets/functions-toolbar-350x189.png)

Den första fliken ![](assets/toolbar-icon-functions-you-map-from-other-modules.png) (visas när panelen öppnas) visar objekt som du kan mappa från andra moduler.

De andra flikarna innehåller följande typer av funktioner:

* **Allmänna funktioner** ![](assets/toolbar-icon-general-function.png) - Se [Allmänna funktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/general-functions.md) för mer information.

* **Matematiska funktioner** ![](assets/toolbar-icon-math-functions.png) - Se [Matematiska funktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/math-functions.md) för mer information.

* **Text- och binärfunktioner** ![](assets/toolbar-icon-text&binary-functions.png) - Se [Strängfunktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/string-functions.md) för mer information.

* **Datum och tid** ![](assets/toolbar-icon-date&time-functions.png) - Se [Datum- och tidsfunktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/date-and-time-functions.md) och artiklarna nedan för mer information.

   * [Token för datum- och tidsformatering i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-formatting.md)
   * [Token för datum- och tidsanalys i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/tokens-for-date-and-time-parsing.md)

* **Funktioner för att arbeta med arrayer** ![](assets/toolbar-icon-functions-for-arrays.png) - Se [Array-funktioner i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/functions/array-functions.md) för mer information.

Så här infogar du en funktion i ett fält:

1. Klicka på funktionsnamnet.

   eller

   Dra funktionen till fältet.

>[!INFO]
>
>**Exempel:** Vissa datatyper förhindrar att användare skriver fler än ett visst antal tecken. Du kan använda delsträngsfunktionen för att begränsa ett värde till ett visst antal tecken.
>
>I det här exemplet begränsar delsträngsfunktionen projektnamnet till 50 tecken.
>
>![](assets/example-meet-length-restriction-350x184.png)

## Kapslingsfunktioner

Du kan kapsla in funktioner i varandra.

## Använd [!DNL Google Sheets] funktioner

If [!DNL Workfront Fusion] har ingen funktion som du vill använda, men den finns i [!DNL Google Sheets]gör du så här:

1. I [!DNL Google Sheets]skapar du ett nytt tomt kalkylblad.
1. I [!DNL Workfront Fusion]öppnar du ditt scenario.
1. Lägg till **[!DNL Google Sheets]** >**[!UICONTROL Update a cell]** till scenariot.

   Instruktioner om hur du lägger till en modul finns i [Lägga till en modul i ett scenario](../../workfront-fusion/scenarios/create-a-scenario.md#add) i artikeln [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Konfigurera modulen:

   1. Välj det nya kalkylbladet i dialogrutan **[!UICONTROL Spreadsheet]** fält.
   1. Infoga formeln som innehåller [!DNL Google Sheets] till **[!UICONTROL Value]** fält.

      Du kan använda utdata från föregående moduler som vanligt.

      ![](assets/exploit-google-sheet-functions-350x218.png)

1. Infoga **[!UICONTROL Google Sheets]>[!UICONTROL Get a cell]** för att få fram det beräknade resultatet.
1. Konfigurera modulen med samma cell-ID som du använde i steg 4.

   ![](assets/exploit-google-sheet-functions-2-350x187.png)
