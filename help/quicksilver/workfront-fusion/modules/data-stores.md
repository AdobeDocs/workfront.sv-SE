---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Datalager i [!DNL Adobe Workfront Fusion]
description: Ett datalager, som liknar en databas eller en enkel tabell, kan lagra data från scenarier, vilket gör det möjligt att överföra data mellan enskilda scenarier eller scenariokörningar. Du kan använda ett datalager för att lagra nya data från olika system under synkroniseringen.
author: Becky
feature: Workfront Fusion
exl-id: 2a665a71-b819-4861-b119-f5c28b87e9c5
source-git-commit: 00a969175626d27b70d516921097725fdf818799
workflow-type: tm+mt
source-wordcount: '1244'
ht-degree: 0%

---

# Datalager i [!DNL Adobe Workfront Fusion]

Ett datalager, som liknar en databas eller en enkel tabell, kan lagra data från scenarier, vilket gör det möjligt att överföra data mellan enskilda scenarier eller scenariokörningar. Du kan använda ett datalager för att lagra nya data från olika system under synkroniseringen.

Med datalagringsmodulerna kan du utföra följande åtgärder för poster i dina [!DNL Adobe Workfront Fusion] datalager:

* Lägg till
* Ersätt
* Uppdatera
* Hämta
* Ta bort
* Sök
* Antal

Mer information om hur du använder datalagermoduler finns i [[!UICONTROL Data store] moduler](../../workfront-fusion/apps-and-their-modules/data-store-modules.md).

En videointroduktion till datalager i Workfront Fusion finns på:

* [Datalager](https://video.tv.adobe.com/v/3427029/){target=_blank}

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
   <p>Aktuell: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Äldre: Alla </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Nytt:</p> <ul><li>[!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Workfront] Plan: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</li><li>[!UICONTROL Ultimate] [!DNL Workfront] Plan: [!DNL Workfront Fusion] ingår.</li></ul>
   <p>eller</p>
   <p>Aktuell: Din organisation måste köpa [!DNL Adobe Workfront Fusion].</p>
   </td> 
  </tr>
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Tillgängligt datautrymme

<!--If your organization is on the new Workfront plan model (Select, Prime, and Ultimate packages), your total data store size is:-->

Om din organisation använder den nya Workfront-planmodellen (Select-, Prime- och Ultimate-paket) påverkar din organisations plan storleken och antalet datalager som är tillgängliga i Fusion-instansen.

### Ultimat plan

Fusion-instanser i Ultimate-paketet tar emot:

* 100 MB ledigt utrymme
* 50 datalager

### Select- och Prime-planer

Fusion-instanser på Select- eller Prime-paketen tar emot:—>

* 100 MB för de första 500 kB-åtgärderna.

* 10 MB för varje ytterligare 100 K-åtgärd.

  En organisation med 600 kB-åtgärder får till exempel 110 MB.

Din organisation kan ha upp till 50 datalager. Den kombinerade storleken på dessa datalager får inte överskrida organisationens totala datalagringsstorlek.

## Skapa ett datalager i [!DNL Workfront Fusion]

* [Konfigurera datalagret](#set-up-the-data-store)
* [Ställ in datastrukturen](#set-up-the-data-structure)

### Konfigurera datalagret

Innan du kan använda ett datalager i en modul måste du skapa datalagret i [!DNL Workfront Fusion].

>[!NOTE]
>
>Din organisation har ett begränsat antal tillgängliga datalager. Om du försöker skapa fler datalager än vad du har tillgängligt [!DNL Workfront] returnerar [!UICONTROL Maximum stores reached] fel.
>
>Mer information finns i [Högsta antal arkiv har nåtts](#maximum-stores-reached-error) i den här artikeln.

1. Logga in på [!DNL Workfront Fusion] konto.
1. Klicka **[!UICONTROL Data stores]** i den vänstra navigeringspanelen.
1. Klicka **[!UICONTROL Add data store]** i skärmens övre högra hörn.
1. Ange inställningar för det nya datalagret.

   En fetstilt titel på ett fält i en [!DNL Workfront Fusion] -modulen anger en obligatorisk inställning.

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data store name] </td> 
      <td> <p>Ange ett namn för datalagret. </p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data Structure]</p> </td> 
      <td> <p>En datastruktur är en lista med kolumner för en tabell. Den här listan anger kolumnnamnet och datatypen.</p> <p>Gör något av följande:</p> 
       <ul> 
        <li style="font-weight: bold;">Välj en datastruktur som redan har skapats</li> 
        <li> <p style="font-weight: bold;">Lägg till en ny datastruktur</p> <p>Klicka <strong>[!UICONTROL Add]</strong> för att skapa en ny datastruktur.</p> <p>Mer information finns i <a href="#set-up-the-data-structure" class="MCXref xref">Ställ in datastrukturen</a> i den här artikeln.</p> </li> 
        <li style="font-weight: bold;"> <p>Lämna fältet tomt</p> <p style="font-weight: normal;">Om du inte markerar eller lägger till en datastruktur kommer databasen endast att innehålla primärnyckeln. En sådan databastyp är användbar om du bara vill spara nycklar och bara vill veta om det finns en viss nyckel i databasen eller inte.</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Data storage size in MB]</p> </td> 
      <td> <p>Allokera storleken på datalagret från din totala interna datalagring.</p> <p> Standardvärdet är 10 MB. Om du har mindre än 10 MB oallokerat datalagringsutrymme från din tilldelning på 95 MB är standardstorleken mängden oallokerat lagringsutrymme.  <p>Obs! Det reserverade beloppet kan ändras när som helst.</p>  </td> 
     </tr> 
    </tbody> 
   </table>

### Ställ in datastrukturen

1. När du skapar eller redigerar ett datalager klickar du **[!UICONTROL Add]**.
1. I **[!UICONTROL Add data structure]** konfigurera följande fält som visas:

   <table style="table-layout:auto">
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Data structure name]</td> 
      <td> <p> Ange ett namn för den nya datastrukturen.</p> </td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Specification]</p> </td> 
      <td> <p>Gör något av följande för att konfigurera kolumnerna i datalagret.</p> 
       <ul> 
        <li> <p>Klicka <strong>[!UICONTROL Add item]</strong> om du vill ange egenskaperna för en kolumn manuellt.</p> <p>Ange <strong>[!UICONTROL Name]</strong> och <strong>[!UICONTROL Type]</strong> för datalagrets kolumn och definiera motsvarande egenskaper.</p> </li> 
        <li> <p>Klicka <strong>[!UICONTROL Generator]</strong> för att fastställa kolumnerna från de exempeldata som du anger.</p> 
         <div class="example" data-mc-autonum="<b>Example: </b>">
          <span class="autonumber"><span><b>Exempel: </b></span></span> 
          <p>I följande JSON-exempeldata skapas tre kolumner: namn, ålder och telefonnummer. Telefonnummer är en samling mobiltelefonnummer och telefonnummer.</p> 
          <p><code>&lbrace;</code> </p> 
          <p><code>"name":"John",</code> </p> 
          <p><code>"age":30,</code> </p> 
          <p><code>"phone number": &lbrace;</code> </p> 
          <p><code>"mobile":"987654321",</code> </p> 
          <p><code>"landline":"123456789"</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p><code>&rbrace;</code> </p> 
          <p>De tomma kolumnerna i datalagervyn:</p> 
          <p> <img src="assets/empty-columns-350x132.png" style="width: 350;height: 132;"> </p> 
          <p>Du kan sedan lägga till värden i datalagret manuellt eller med [!DNL Workfront Fusion] datalagermoduler.</p> 
         </div> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Strict] </td> 
      <td> <p>Aktivera det här alternativet för att säkerställa att nyttolasten matchar datastrukturerna. Nyttolaster som innehåller extra artiklar som inte har angetts i datastrukturen nekas.</p> </td> 
     </tr> 
    </tbody> 
   </table>

## Redigera ett befintligt datalager

Du kan redigera egenskaperna och innehållet i ett befintligt datalager i dialogrutan [!UICONTROL Data Store] område på [!DNL Workfront Fusion].

* [Redigera egenskaperna för ett datalager](#edit-the-properties-of-a-data-store)
* [Redigera innehållet i ett datalager](#edit-the-contents-of-a-data-store)

### Redigera egenskaperna för ett datalager

Egenskaperna för ett datalager omfattar datastrukturen som används i datalagret samt storleken på datalagret.

1. Klicka **[!UICONTROL Data Store]** ![](assets/data-store-icon.png) i den vänstra navigeringspanelen för att öppna [!UICONTROL Data Store] område.
1. Klicka **[!UICONTROL Edit]** ![](assets/data-store-edit.png) bredvid det datalager som du vill redigera.
1. (Valfritt) Om du vill ändra den datastruktur som används av det här datalagret till en annan befintlig datastruktur väljer du den i **[!UICONTROL Data structure]** nedrullningsbar meny.

   eller

   (Valfritt) Om du vill ändra den datastruktur som används av det här datalagret till en helt ny datastruktur, se [Ställ in datastrukturen](#set-up-the-data-structure) i den här artikeln.

1. (Valfritt) Ändra storleken på datalagret genom att ange den nya storleken i **[!UICONTROL Data storage size in MB]** fält.
1. Klicka på **[!UICONTROL Save]**.

### Redigera innehållet i ett datalager

1. Klicka på **[!UICONTROL Data Store]** icon ![](assets/data-store-icon.png) i den vänstra navigeringspanelen för att öppna [!UICONTROL Data Store] område.
1. Klicka **[!UICONTROL Browse]**  bredvid det datalager som du vill redigera.
1. (Valfritt) Ändra ordning på kolumner genom att dra dem till önskad plats.
1. (Valfritt) [!UICONTROL Edit] en enda cell genom att klicka på **[!UICONTROL Edit]** i cellen och sedan ange önskat värde.
1. (Valfritt) Lägg till ett nytt objekt i datalagret genom att klicka på **[!UICONTROL Add]** och anger sedan informationen för det nya objektet.
1. Klicka på **[!UICONTROL Save]**.

## Felsökning

* [Återställa förlorade data från ett datalager](#restoring-lost-data-from-a-data-store)
* [Slut på utrymme-fel](#out-of-space-error)
* [Högsta antal arkiv har nåtts](#maximum-stores-reached-error)

### Återställa förlorade data från ett datalager

Det finns för närvarande inget verktyg som kan automatisera återställning av förlorade data.

#### Tillfällig lösning

1. Granska alla körningsloggar för scenarier där objekt infogades i datalagret.

   Mer information om hur du undersöker körningsloggar finns i [Visa ett scenario körningshistorik i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/view-scenario-execution-history.md).

1. Kopiera data.
1. Infoga data i datalagret igen.

   Mer information om hur du infogar data i ett datalager finns i [Redigera innehållet i ett datalager](#edit-the-contents-of-a-data-store) i den här artikeln.

### [!UICONTROL Out of space] fel

An [!UICONTROL Out of Space] ett fel inträffar eftersom dina tidigare skapade datalager redan har tilldelats ditt allokerade datalager.

#### Tillfällig lösning

1. Redigera alla befintliga datalager för att utnyttja mindre utrymme. Detta frigör utrymme för ditt nya datalager.

   Mer information finns i [Redigera egenskaperna för ett datalager](#edit-the-properties-of-a-data-store) i den här artikeln.

>[!NOTE]
>
>Vi rekommenderar att du inte tilldelar allt utrymme till ett enda datalager om du inte är säker på att du inte behöver fler datalager.

### [!UICONTROL Maximum stores reached] fel

A [!UICONTROL Maximum stores reached] felet inträffar eftersom din organisation har använt alla tillgängliga datalager. En organisation har ett antal tillgängliga datalager som är dubbelt så många som antalet tillgängliga scenarier. Det totala antalet tillgängliga datalager beror därför på den plan du har köpt.

Om din organisation till exempel har köpt en plan med 15 scenarier kan organisationen ha upp till 30 datalager.

#### Tillfällig lösning

Om du vill minska antalet befintliga datalager kan du göra något av följande:

* Kombinera befintliga datalager
* Ta bort oanvända datalager
