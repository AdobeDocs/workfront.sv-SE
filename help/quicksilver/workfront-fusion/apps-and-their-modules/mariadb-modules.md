---
title: MariaDB-moduler
description: I ett [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder  [!DNL MariaDB] samt ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: 45d4d7fe-a70c-4906-adb4-f913a870fe47
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '541'
ht-degree: 0%

---

# [!DNL MariaDB] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!DNL MariaDB] samt ansluta det till flera tredjepartsprogram och -tjänster.

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

Du måste ha ett [!DNL MariaDB]-konto för att kunna använda [!DNL MariaDB]-moduler.

## Anslut [!DNL MariaDB] till [!DNL Workfront Fusion]

Du kan skapa en anslutning till ditt [!DNL MariaDB]-konto direkt inifrån en [!DNL MariaDB]-modul.

1. Klicka på **[!UICONTROL Add]** bredvid fältet [!UICONTROL Connection] i någon [!DNL MariaDB]-modul.
1. Konfigurera följande fält:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Connection name]</p> </td> 
      <td> <p>Ange ett namn för den nya anslutningen.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Host]</td> 
      <td> <p>Ange IP-adressen eller värdnamnet för databasinstansen. Värden måste vara åtkomlig utanför nätverket.</p> <p>Exempel: <code>[!DNL mariadb.hwoh2j5h.us-east-1.rds.amazon.com]</code></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Port]</td> 
      <td>Standardporten är 3306. Om du använder en port som inte är standard anger du det här numret till din port. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Database Name]</td> 
      <td>Ange namnet på den databas som du vill interagera med.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Username]</td> 
      <td>Ange ditt användarnamn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Password]</td> 
      <td>Ange ditt lösenord.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL MariaDB] moduler och deras fält

När du konfigurerar [!DNL MariaDB] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL MariaDB] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

### Kör en fråga (avancerat)

Den här åtgärdsmodulen hämtar information från databasen baserat på en fråga som du anger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL MariaDB]-konto till [!DNL Workfront Fusion] finns i <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Ansluta [!DNL MariaDB] till [!DNL Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query]</td> 
   <td> <p>Ange den SQL-fråga som du vill att modulen ska använda för att hämta data.</p> <p>Viktigt: Variabler som används i frågan saneras inte. Se till att du sanerar variablerna på rätt sätt för att förhindra SQL-injektion.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Select rows from a table (advanced)]

Den här modulen läser post från din databas.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du ansluter ditt [!DNL MariaDB]-konto till [!DNL Workfront Fusion] finns i <a href="#connect-mariadb-to-workfront-fusion" class="MCXref xref">Ansluta [!DNL MariaDB] till [!DNL Workfront Fusion]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Table]</td> 
   <td> <p>Markera den tabell som innehåller de poster som du vill läsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td> <p>Ange med vilket filter du vill markera rader</p> 
    <ul> 
     <li> <p>Markera fältet som du vill söka efter</p> </li> 
     <li> <p>Välj den operator som du vill använda för sökningen</p> </li> 
     <li> <p>Ange eller mappa värdet som du vill söka efter.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort] </td> 
   <td> <p>För varje nivå som du vill att resultaten ska sorteras efter klickar du på <strong>[!UICONTROL Add item]</strong> och väljer sedan det fält som du vill sortera resultaten efter och om du vill sortera stigande eller fallande</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>
