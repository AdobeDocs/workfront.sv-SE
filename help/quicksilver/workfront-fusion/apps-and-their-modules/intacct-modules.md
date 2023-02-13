---
title: Intacctmoduler
description: Intacctmoduler
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: fa1aa943-fbda-4eb4-bfa1-ab94a56785a7
source-git-commit: 9a4a847b542783845a3f896ec4e35d5efc7c122b
workflow-type: tm+mt
source-wordcount: '543'
ht-degree: 0%

---

# Intacctmoduler

I en [!DNL Adobe Workfront Fusion] kan du automatisera arbetsflöden som använder Intacct och ansluta det till flera tredjepartsprogram och -tjänster.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Om du vill använda Intacct-moduler måste du ha ett Intacct-konto.

## Anslut till Workfront Fusion via Internet

### Auktoriserar [!DNL Workfront Fusion] för att göra ändringar i Int.

Före [!DNL Workfront Fusion] kan ansluta till [!DNL Intacct]måste du godkänna det.

Gå till **[!UICONTROL Company]** -fliken.

1. Klicka **Företagsinformation**.
1. Navigera till **Säkerhet** -fliken.
1. Klicka [!UICONTROL Edit] i det övre högra hörnet
1. Välj Webbtjänstauktoriseringar.
1. Klicka på plusikonen
1. Ange AzuquaMPP som sender_id.
1. (Valfritt) Ange en beskrivning för anslutningen

### Konfigurera en anslutning i [!DNL Workfront Fusion] {#set-up-a-connection-in-workfront-fusion}

Du kan skapa en anslutning till [!DNL Intacct] direkt inifrån ett [!DNL Intacct] -modul.

1. Klicka i någon av Int-modulerna på **[!UICONTROL Add]** bredvid fältet Connection.
1. Ange dina Intaccent-inloggningsuppgifter

   * Företags-ID
   * Användar-ID
   * Lösenord

1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## Intacctmoduler och deras fält

När du konfigurerar [!DNL Intacct] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Dessutom kan ytterligare Intacct-fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Search records]](#search-records)

### [!UICONTROL Make a custom API call] {#make-a-custom-api-call}

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Intacct] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Intacct] moduler.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Anslutning</p> </td> 
   <td> <p>Instruktioner om hur du ansluter Intacct-kontot till [!DNL Workfront Fusion] 2.0, se <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Konfigurera en anslutning i Workfront Fusion</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Brödtext-XML</td> 
   <td> <p>Inkludera endast XML-innehållet i brödtexten. Begäran innehåller automatiskt autentiseringshuvuden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search records]

Den här sökmodulen hämtar en lista med poster som matchar specifika sökvillkor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p>Anslutning</p> </td> 
   <td> <p>Instruktioner om hur du ansluter Intacct-kontot till [!DNL Workfront Fusion] 2.0, se <a href="#set-up-a-connection-in-workfront-fusion" class="MCXref xref">Konfigurera en anslutning i Workfront Fusion</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj den typ av post som du vill söka efter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Sökvillkor</p> </td> 
   <td> 
    <ul> 
     <li> <p>Markera fältet som du vill söka efter</p> </li> 
     <li> <p>Välj den operator som du vill använda för sökningen</p> </li> 
     <li> <p>Ange värdet som du vill söka efter</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resultatuppsättning</td> 
   <td>Välj om du vill returnera alla matchande poster eller bara den första matchande posten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Gräns</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Sortera efter</td> 
   <td>Markera det fält som du vill sortera resultaten efter. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Order</td> 
   <td>Välj om du vill sortera stigande eller fallande.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Utdata</td> 
   <td> <p>Välj den information som du vill inkludera i utdatapaketet för den här modulen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Skiftlägeskänslighet</td> 
   <td>Aktivera det här alternativet om du vill att frågan ska vara skiftlägeskänslig.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Fråga om privata enheter</td> 
   <td>Aktivera det här alternativet om du vill tillåta modulen att söka efter privata enheter.</td> 
  </tr> 
 </tbody> 
</table>
