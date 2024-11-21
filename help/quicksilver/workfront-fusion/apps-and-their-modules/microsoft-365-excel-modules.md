---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
keywords: koppling
navigation-topic: apps-and-their-modules
title: Microsoft Office 365 Excel-moduler
description: I ett [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder Microsoft 365 Excel samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 9aa3739d-6800-4eb1-a17f-32fdfd8ed0f2
source-git-commit: 55485da1ea650121b5537a3f19d8102623ed4f43
workflow-type: tm+mt
source-wordcount: '2374'
ht-degree: 0%

---

# [!DNL Microsoft Office 365 Excel] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!DNL Microsoft 365 Excel] samt ansluta det till flera tredjepartsprogram och -tjänster.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
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

## Förutsättningar

Du måste ha ett Microsoft-konto för att kunna använda [!DNL Microsoft office 365 Excel].

## API-information för Microsoft Office 365 Excel

Microsoft Office 365 Excel-anslutningen använder följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bas-URL</td> 
   <td> https://graph.microsoft.com/v1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-version</td> 
   <td> v1.0 </td> 
  </tr> 
  <tr> 
   <td role="rowheader">API-tagg</td> 
   <td>v2.0.16</td> 
  </tr>
 </tbody> 
 </table>



## Ansluter tjänsten [!DNL Office 365 Excel] till [!DNL Workfront Fusion]

Instruktioner om hur du ansluter ditt [!DNL Office 365 Excel]-konto till [!UICONTROL Workfront Fusion] finns i [Skapa en anslutning till [!UICONTROL Adobe Workfront Fusion] - grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

>[!NOTE]
>
>Vissa Microsoft-program använder samma anslutning, som är kopplad till individuella användarbehörigheter. När du skapar en anslutning visas därför alla behörigheter som tidigare har beviljats användarens anslutning, förutom de nya behörigheter som krävs för det aktuella programmet.
>
>Om en användare till exempel har behörighet att läsa tabell som beviljats via Excel-anslutningen och sedan skapar en anslutning i Outlook-anslutningen för att läsa e-post, visar tillståndsskärmen både den behörighet som redan har beviljats för att läsa tabell och den behörighet som nyligen har krävts för att skriva e-post.

## [!DNL Microsoft Office 365 Excel]-moduler och deras fält

När du konfigurerar [!DNL Microsoft 365 Excel] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL Microsoft 365 Excel] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Arbetsbok](#workbook)
* [Kalkylblad](#worksheet)
* [Tabell](#table)
* [Övriga](#other)

### Arbetsbok

* [Se arbetsböcker](#watch-workbooks)
* [Sök i arbetsböcker](#search-workbooks)
* [Hämta en arbetsbok](#download-a-workbook)

#### [!UICONTROL Watch Workbooks]

Den här utlösarmodulen startar ett scenario när en arbetsbok skapas.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Välj den mapp som du vill bevaka för nya arbetsböcker.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Du kan ställa in ett filter så att det bara bevakar arbetsböcker som uppfyller de villkor du väljer.</p> <p>För varje filter anger du fältet som du vill att filtret ska utvärderas, operatorn och värdet som du vill att filtret ska tillåta. Du kan använda mer än ett filter genom att lägga till OCH- eller OR-regler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet arbetsböcker som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search Workbooks]

Denna åtgärdsmodul söker efter [!DNL Excel] arbetsböcker.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Folder]</td> 
   <td> <p>Välj den mapp som du vill söka efter arbetsböcker i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Du kan ställa in ett filter så att du bara söker efter arbetsböcker som uppfyller de villkor du väljer.</p> <p>För varje filter anger du fältet som du vill att filtret ska utvärderas, operatorn och värdet som du vill att filtret ska tillåta. Du kan använda mer än ett filter genom att lägga till OCH- eller OR-regler.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal kalkylblad som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download a Workbook]

Den här åtgärdsmodulen hämtar innehållet i den angivna Excel-arbetsboken.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Download a workbook]</td> 
   <td> <p>Välj hur du vill identifiera arbetsboken för modulen som ska hämtas.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL By entering an ID manually]</strong> </p> <p>I fältet [!UICONTROL Workbook ID] anger eller mappar du ID:t för den specifika arbetsbok som du vill att modulen ska hämta.</p> </li> 
     <li> <p><strong>[!UICONTROL By selecting from the path]</strong> </p> <p>I fältet [!UICONTROL Workbook] väljer du arbetsboken som du vill att modulen ska hämta.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Kalkylblad

* [[!UICONTROL Watch Worksheet Rows]](#watch-worksheet-rows)
* [[!UICONTROL List Worksheets]](#list-worksheets)
* [[!UICONTROL List Worksheet Rows]](#list-worksheet-rows)
* [[!UICONTROL Add a Worksheet]](#add-a-worksheet)
* [[!UICONTROL Add a Worksheet Row]](#add-a-worksheet-row)
* [[!UICONTROL Update a Worksheet Row]](#update-a-worksheet-row)
* [[!UICONTROL Delete a Worksheet Row]](#delete-a-worksheet-row)

#### [!UICONTROL Watch Worksheet Rows]

Denna utlösarmodul startar ett scenario när en ny rad läggs till i bladet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller det kalkylblad som du vill bevaka för nya rader.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera det Excel-blad som du vill bevaka för nya rader.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ange eller mappa det maximala antalet kalkylbladsrader som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Worksheets]

Den här åtgärdsmodulen hämtar en lista med kalkylblad i den angivna arbetsboken.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller de kalkylblad som du vill att modulen ska visa.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ange eller mappa det maximala antal kalkylblad som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Worksheet Rows]

Den här åtgärdsmodulen hämtar en lista med rader i det angivna kalkylbladet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller kalkylbladet som innehåller de rader som du vill visa.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera kalkylbladet som innehåller raderna som du vill visa.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ange eller mappa det maximala antalet kalkylbladsrader som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a Worksheet]

Den här åtgärdsmodulen skapar ett nytt kalkylblad i den valda arbetsboken.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken där du vill lägga till ett kalkylblad.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Name] </td>
   <td> <p>Ange eller mappa ett namn för det nya kalkylbladet.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a Worksheet Row]

Den här åtgärdsmodulen lägger till en ny rad i det markerade kalkylbladet.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller kalkylbladet där du vill lägga till en rad.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera det kalkylblad där du vill lägga till en rad.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>Välj vilken typ av värde som ska anges i kalkylbladet. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel försöker utvärdera det angivna uttrycket. Namnen på funktionerna i en formel är på engelska. Exempel: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel försöker utvärdera det angivna uttrycket. Funktionsnamnen är på samma språk som i Excel-programmet. Exempel: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel utvärderar inte värdet. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>För varje kolumn anger du det värde som du vill att kolumnen ska ha i den nya raden.</td>
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a Worksheet Row]

Den här åtgärdsmodulen uppdaterar en befintlig kalkylbladsrad.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller kalkylbladet som innehåller raden som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera kalkylbladet som innehåller raden som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Type of values being entered]</p> </td> 
   <td> <p>Välj vilken typ av värde som ska anges i kalkylbladet. </p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Formulas]</strong> </p> <p> Excel försöker utvärdera det angivna uttrycket. Namnen på funktionerna i en formel är på engelska. Exempel: <code>[!DNL =SUM(A1:A10)]</code></p> </li> 
     <li> <p><strong>[!UICONTROL Formulas local]</strong> </p> <p>Excel försöker utvärdera det angivna uttrycket. Funktionsnamnen är på samma språk som i Excel-programmet. Exempel: <code>=SUM(A1, 1.5)</code> vs <code>=SUMME(A1; 1,5)</code></p> </li> 
     <li> <p><strong>[!UICONTROL Value]</strong> </p> <p>Excel utvärderar inte värdet. </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Row ID]</td> 
   <td>Markera numret på den rad som ska uppdateras.</td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>För varje kolumn anger du det värde som du vill att kolumnen ska ha i den nya raden.</td>
   —&gt; 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a Worksheet Row]

Den här åtgärdsmodulen tar bort en rad från ett kalkylblad.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller kalkylbladet som innehåller raden som du vill ta bort.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet]</td>
   <td> <p> Markera kalkylbladet som innehåller raden som du vill ta bort.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Row ID]</td>
   <td>Ange eller mappa ID:t för raden som du vill ta bort.</td> 
  </tr> 
 </tbody> 
</table>

### Tabell

* [[!UICONTROL Watch table rows]](#watch-table-rows)
* [[!UICONTROL List tables]](#list-tables)
* [[!UICONTROL List table rows]](#list-table-rows)
* [[!UICONTROL Get a Table]](#get-a-table)
* [[!UICONTROL Add a table]](#add-a-table)
* [[!UICONTROL Add a table row]](#add-a-table-row)
* [[!UICONTROL Update a table]](#update-a-table)
* [[!UICONTROL Delete a table]](#delete-a-table)

#### [!UICONTROL Watch table rows]

Detta startar ett scenario när en ny rad läggs till i en tabell.

>[!NOTE]
>
>Tabellen här refererar till det inbäddade tabellelementet i arbetsboken. Inte hela tabellen (arbetsbok/ark).

![](assets/embedded-table-350x420.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Workbook]</p> </td> 
   <td> <p>Markera arbetsboken som innehåller tabellen som du vill bevaka.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p> Markera det kalkylblad som innehåller tabellen som du vill titta på.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Table]</p> </td> 
   <td> <p>Markera tabellen som du vill bevaka.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ange eller mappa det maximala antal rader som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List tables]

Den här sökmodulen hämtar en lista med alla tabellobjekt.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller de tabeller som du vill visa.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera kalkylbladet som innehåller de tabeller som du vill visa</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ange eller mappa det maximala antalet tabeller som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List table rows]

Den här sökmodulen hämtar en lista med alla tabellrader i en arbetsbok.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller tabellen som innehåller raderna som du vill visa.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera kalkylbladet som innehåller tabellen som innehåller raderna som du vill visa</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table] </td>
   <td> <p>Markera tabellen som innehåller raderna som du vill visa.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Limit]</td>
   <td> <p>Ange eller mappa det maximala antalet tabellrader som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get a Table]

Den här åtgärdsmodulen hämtar metadata för den angivna tabellen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> 
     <p >[!UICONTROL Connection]</p>
   </td> 
   <td> 
     <p>Instruktioner om hur du ansluter Office 365-kontot till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p>
    —&gt; </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>Välj hur du vill identifiera tabellen som du vill hämta.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa ID:t för arbetsboken som innehåller tabellen som du vill hämta i fältet [!UICONTROL Workbook ID].</p> <p>I fältet [!UICONTROL Table Name] anger eller mappar du namnet på tabellen som du vill hämta.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Markera arbetsboken och kalkylbladet som innehåller tabellen som du vill hämta och markera sedan tabellen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a table]

Den här åtgärdsmodulen skapar ett tabellelement i Excel-kalkylbladet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>Markera arbetsboken som innehåller kalkylbladet där du vill lägga till en tabell.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Markera det kalkylblad där du vill lägga till en tabell.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Has headers]</td> 
   <td> <p>Aktivera det här alternativet om du vill definiera den första raden som tabellrubriker.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Address]</p> </td> 
   <td> <p>Ange tabellens storlek genom att ange cellerna längst upp till vänster och längst ned till höger. Exempel: <code>A1:C10</code> skapar en tabell med 3 kolumner och 10 rader.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add a table row]

Den här åtgärdsmodulen ändrar en befintlig tabell.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Workbook] </td>
   <td> <p>Markera arbetsboken som innehåller tabellen där du vill lägga till en rad.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Worksheet] </td>
   <td> <p>Markera det kalkylblad som innehåller tabellen där du vill lägga till en rad.</p> </td> 
  </tr> 
  <tr> 
    <td role="rowheader" >[!UICONTROL Table]</td>
   <td>Markera den tabell där du vill lägga till en rad.</td> 
  </tr> 
  <tr>
    <td role="rowheader" >[!UICONTROL Row]</td>
    <td>För varje kolumn anger du det värde som du vill att kolumnen ska ha i den nya raden.</td>
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Row ID]</p> </td> 
   <td> <p>Om du vill lägga till en rad på en viss plats i tabellen anger eller mappar du ett radnummer. Modulen infogar den nya raden efter den här raden.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a table]

Den här åtgärdsmodulen uppdaterar en befintlig tabell.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update a table]</td> 
   <td> <p>Välj hur du vill identifiera tabellen som du vill uppdatera.</p> 
    <ul> 
     <li> <p><strong>Ange manuellt</strong> </p> <p>Ange eller mappa ID:t för arbetsboken som innehåller tabellen som du vill uppdatera i fältet [!UICONTROL Workbook ID].</p> <p>I fältet [!UICONTROL Table Name] anger eller mappar du namnet på tabellen som du vill uppdatera.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Markera arbetsboken och kalkylbladet som innehåller tabellen som du vill uppdatera och markera sedan tabellen.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table] </td> 
   <td> <p>Markera tabellen som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name]</td> 
   <td> <p>Om du vill byta namn på tabellen anger eller mappar du ett nytt namn för tabellen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show Headers]</td> 
   <td> <p>Aktivera det här alternativet om du vill visa rubrikerna i den uppdaterade tabellen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Show totals]</td> 
   <td>Aktivera det här alternativet om du vill visa tabellens totala värden.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Style]</td> 
   <td>Välj ett format för den nya tabellen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete a table]

Den här åtgärdsmodulen tar bort den angivna tabellen från ett [!DNL Excel]-kalkylblad.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Get a table]</td> 
   <td> <p>Välj hur du vill identifiera tabellen som du vill ta bort.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa ID:t för arbetsboken som innehåller tabellen som du vill ta bort i fältet [!UICONTROL Workbook ID].</p> <p>I fältet [!UICONTROL Table Name] anger eller mappar du namnet på tabellen som du vill ta bort.</p> </li> 
     <li> <p><strong>[!UICONTROL Select from the list]</strong> </p> <p>Markera arbetsboken och kalkylbladet som innehåller tabellen som du vill ta bort och markera sedan tabellen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

### Övriga

* [[!UICONTROL Retrieve data]](#retrieve-data)
* [[!UICONTROL Make an API Call]](#make-an-api-call)

#### [!UICONTROL Retrieve data]

Den här åtgärden hämtar data från det definierade kalkylbladsområdet och returnerar ett paket för varje rad.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workbook] </td> 
   <td> <p>Markera arbetsboken som innehåller de data som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Worksheet] </td> 
   <td> <p>Markera det kalkylblad som innehåller de data som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Range] </td> 
   <td> <p>Ange det område i bladet som du vill hämta data från genom att ange cellerna längst upp till vänster och längst ned till höger. Exempel: <code>A1:D10</code></p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make an API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat API-anrop.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Connection]</p> </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!DNL Office 365]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/scenarios/create-a-scenario.md#connect" class="MCXref xref">Ansluta modulens app- eller webbtjänst till [!DNL Workfront Fusion]</a> i artikeln <a href="../../workfront-fusion/scenarios/create-a-scenario.md" class="MCXref xref">Skapa ett scenario i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ange en relativ sökväg till <code>https://graph.microsoft.com</code>. Exempel:<code> /v1.0/me/drive/root/children</code></td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   td&gt; <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metoder för HTTP-begäran i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!   <p>När du använder villkorssatser som <code>if</code> i JSON placerar du citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>
