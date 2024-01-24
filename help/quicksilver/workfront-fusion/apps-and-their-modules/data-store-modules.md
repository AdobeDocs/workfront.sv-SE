---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Datalagermoduler
description: An [!DNL Adobe Workfront Fusion] datalager, som liknar en databas eller en enkel tabell, kan lagra data från scenarier, vilket gör det möjligt att överföra data mellan enskilda scenarier eller scenariokörningar. Du kan använda ett datalager för att lagra nya data från olika system under synkroniseringen.
author: Becky
feature: Workfront Fusion
exl-id: 1dc9cb88-d1b9-4a67-91fb-be980cc1ccd1
source-git-commit: c51169c18bef8ac8126a04c08deb88d830517b0b
workflow-type: tm+mt
source-wordcount: '1038'
ht-degree: 0%

---

# [!UICONTROL Data store] moduler

An [!DNL Adobe Workfront Fusion] datalager, som liknar en databas eller en enkel tabell, kan lagra data från scenarier, vilket gör det möjligt att överföra data mellan enskilda scenarier eller scenariokörningar. Du kan använda ett datalager för att lagra nya data från olika system under synkroniseringen.

Med datalagermodulerna kan du lägga till, ersätta, uppdatera, hämta, ta bort, söka efter eller räkna poster i [!DNL Adobe Workfront Fusion] datalager.

Mer information om hur du skapar, redigerar och felsöker datalager finns i [Datalager i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

En videointroduktion till datalager i Workfront Fusion finns på:

* [Datalager](https://video.tv.adobe.com/v/3427029/){target=_blank}

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

## Förutsättningar

Används [!UICONTROL Data Store] måste du först skapa ett datalager.

Mer information om hur du skapar datalager finns i [Datalager i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-stores.md)

## [!UICONTROL Data Store] moduler och deras fält

När du konfigurerar datalagermoduler [!DNL Workfront Fusion] visar fälten som listas nedan. Dessutom kan ytterligare datalagerfält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

Alla [!UICONTROL Data Store] moduler är åtgärdstypmoduler.

* [Lägg till/ersätta en post](#addreplace-a-record)
* [Uppdatera en post](#update-a-record)
* [Hämta en post](#get-a-record)
* [Kontrollera förekomsten av en post](#check-the-existence-of-a-record)
* [Ta bort en post](#delete-a-record)
* [Ta bort alla poster](#delete-all-records)
* [Sök i poster](#search-records)
* [Antal poster](#count-records)

### [!UICONTROL Add/Replace a Record]

Den här åtgärdsmodulen lägger till eller ersätter en post.

Du anger datalagret och postens nyckel.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

>[!NOTE]
>
>Modulen genererar ett fel när du försöker lägga till den post som redan finns i datalagret under samma namn och [!UICONTROL Overwrite an existing record] alternativet är inaktiverat.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Välj eller lägg till datalagret där du vill skapa en post. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Ange den unika nyckeln för den post som du vill att modulen ska lägga till eller ersätta. Nyckeln kan användas senare för att hämta posten. Om du lämnar det här fältet tomt genereras en nyckel automatiskt.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Overwrite an existing record] </td> 
   <td> <p>Aktivera det här alternativet om du vill skriva över posten. Den post som du vill skriva över måste anges i fältet Nyckel ovan.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record] </td> 
   <td> <p>Ange önskade värden för postens fält.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Update a Record]

Den här åtgärdsmodulen uppdaterar en post.

Du anger datalagret och postens nyckel.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Välj eller lägg till datalagret där du vill skapa en post. </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Ange den unika nyckeln för den post som du vill att modulen ska uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Insert missing record] </td> 
   <td> <p>Aktivera det här alternativet om du vill skapa en ny post om posten med den angivna nyckeln inte redan finns.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Record]</td> 
   <td> <p> Ange önskade värden i postens fält som du vill uppdatera.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Get a Record]

Denna åtgärdsmodul hämtar en post.

Du anger datalagret och postens nyckel.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Välj det datalager som du vill hämta en post från</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Ange den unika nyckeln för den post som du vill hämta modulen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Check the Existence of a Record]

Den här åtgärdsmodulen anger om en viss post finns.

Du anger datalagret och postens nyckel.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Välj det datalager som du vill kontrollera om posten finns.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Ange den unika nyckeln för den post som du vill att modulen ska kontrollera om den finns.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete a Record]

Den här åtgärdsmodulen tar bort en post.

Du anger datalagret och postens nyckel.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Välj det datalager som du vill kontrollera om posten finns.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Key] </td> 
   <td> <p>Ange den unika nyckeln för den post som du vill ta bort modulen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Delete All Records]

Den här åtgärdsmodulen tar bort alla poster från ett visst datalager.

Du anger datalagret.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Markera det datalager som du vill ta bort alla poster från.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Search Records]

Den här sökmodulen söker efter poster i ett objekt i datalagret som matchar den sökfråga du anger.

Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store]</td> 
   <td> <p> Markera det datalager som du vill söka i.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Filter]</p> </td> 
   <td> <p>Ange filtret för sökningen.</p> </td> 
  </tr> 
  <tr> 
   <td> <p>[!UICONTROL Sort]</p> </td> 
   <td> <p style="font-weight: normal;">För varje fält som du vill sortera efter fyller du i följande fält:</p> <p style="font-weight: bold;">[!UICONTROL Key]</p> <p>Markera kolumnnamnet som du vill sortera resultaten efter.</p> <p style="font-weight: bold;">[!UICONTROL Order]</p> <p>Välj om du vill sortera resultaten i stigande eller fallande ordning.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Limit]</td> 
   <td> <p> Ange maximalt antal sökresultat [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Continue the execution of the route even if the module returns no results]</td> 
   <td> <p> Om det här alternativet är aktiverat fortsätter den väg som den här modulen är en del av bearbetningen, även om den här modulen inte returnerar några resultat.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Count Records]

Den här åtgärdsmodulen numrerar posterna i ett datalager.

Du anger datalagret.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data store] </td> 
   <td> <p>Markera det datalager som innehåller de poster som du vill räkna.</p> </td> 
  </tr> 
 </tbody> 
</table>
