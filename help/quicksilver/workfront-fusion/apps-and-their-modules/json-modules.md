---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: JSON-moduler
description: Adobe Workfront Fusion JSON-appen innehåller moduler som bearbetar data i JSON-format så att Adobe Workfront Fusion kan arbeta vidare med datainnehållet eller skapa nytt JSON-innehåll.
author: Becky
feature: Workfront Fusion
exl-id: 60540608-9d2e-4e10-9fb2-5388dda64784
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# [!UICONTROL JSON] moduler

The [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] appen innehåller moduler som bearbetar data i JSON-format så att [!DNL Adobe Workfront Fusion] kan arbeta vidare med datainnehållet eller skapa nytt JSON-innehåll.

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
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Tolka JSON

* [Datastruktur](#data-structure)
* [Samling kontra matris](#collection-vs-array)

### Datastruktur

Datastrukturen beskriver hur JSON-data ordnas och möjliggör mappning av enskilda JSON-objekt till andra moduler i ditt scenario. Om du inte anger datastrukturen kan du köra modulen manuellt och [!DNL Workfront Fusion] kommer att bygga upp strukturen från den tillhandahållna JSON-versionen:

1. Lägg till [!UICONTROL Parse JSON] modulen till ett scenario.
1. I **[!UICONTROL JSON String]** anger du den JSON som du vill bygga en datastruktur från.
1. Anslut inte andra moduler till [!UICONTROL Parse JSON] ännu. För [!DNL Workfront Fusion] känner ännu inte till JSON-datastrukturen, det är ännu inte möjligt att mappa data från [!UICONTROL Parse JSON] till andra moduler i ditt scenario.
1. Kör scenariot manuellt. Detta gör att [!UICONTROL Parse JSON] för att identifiera JSON-strukturen från den JSON du har angett.
1. Nu kan du ansluta följande moduler. Objekten från JSON-modulen Parse är nu tillgängliga för mappning.

Mer information finns i [Datastrukturer i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Samling kontra matris

Om JSON-strängfältet innehåller en samling `{ ... }`, är utdata ett enda paket som innehåller objekten i samlingen.

>[!INFO]
>
>**Exempel:**
>
>```
>{
>       "name" : "Peter",
>
>    
>   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Om JSON-strängfältet innehåller en array `[ ... ]`, är utdata en serie paket. varje paket innehåller ett element i arrayen.

>[!INFO]
>
>**Exempel:**
>
>```
>[
>   {
>       "name" : "Peter",
>       "ID" : 1
>   },
>
>  
> {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON] moduler och deras fält

När du konfigurerar [!DNL JSON] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Dessutom kan ytterligare JSON-fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Sammanställd till JSON](#aggregate-to-json)
* [Konvertera JSON till XML](#convert-json-to-xml)
* [Tolka JSON](#parse-json)
* [Skapa JSON](#create-json)
* [Omforma JSON](#transform-json)

### [!UICONTROL Aggregate to JSON]

Den här aggregeringsmodulen aggregerar utdata från en tidigare modul till JSON.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source module] </td> 
   <td> <p>Markera modulen som matar ut data som du vill aggregera till JSON.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Välj den datastruktur som du vill använda för att skapa JSON. Datastrukturen avgör vilka andra fält som är tillgängliga i den här modulen. Mer information finns i <a href="#data-structure" class="MCXref xref">Datastruktur</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Indentation]</td> 
   <td> <p> Ange om du vill dra in JSON med hjälp av tabbar, två blanksteg eller fyra blanksteg.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by]</td> 
   <td>Definiera ett uttryck som du vill gruppera aggregerade utdata med. Det här uttrycket kan innehålla ett eller flera mappade objekt. Sammanlagda data delas sedan upp i grupper med hjälp av det här uttryckets värde. Varje grupp skickar som ett separat paket med en nyckel (det utvärderade uttrycket) och ett värde (den sammanställda texten). Du kan använda nyckeln som ett filter i efterföljande moduler.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Aktivera det här alternativet om du vill stoppa scenariot när det inte finns några resultat.</td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Convert JSON to XML]

Den här åtgärdsmodulen konverterar en JSON-sträng till XML.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Ange eller mappa den JSON som du vill konvertera till XML.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Parse JSON]

Den här åtgärdsmodulen tolkar en JSON-sträng i en datastruktur, som gör att du kan komma åt data i JSON-strängen.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data structure]</td> 
   <td> <p>Välj den datastruktur som du vill använda för att skapa JSON. Mer information finns i <a href="#data-structure" class="MCXref xref">Datastruktur</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL JSON string] </td> 
   <td> <p>Ange eller mappa den JSON som du vill analysera.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Create JSON]

Den här åtgärdsmodulen skapar JSON från en datastruktur.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">Datastruktur</td> 
   <td> <p>Välj den datastruktur som du vill använda för att skapa JSON. Mer information finns i <a href="#data-structure" class="MCXref xref">Datastruktur</a> i den här artikeln.</p> </td> 
  </tr> 
 </tbody> 
</table>

### [!UICONTROL Transform JSON]

Den här åtgärdsmodulen omvandlar ett objekt till en json-sträng.

<table style="table-layout:auto"> 
 <col data-mc-conditions=""> 
 <col data-mc-conditions=""> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object]</td> 
   <td> <p>Ange eller mappa objektet som du vill omforma till JSON.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Omvandla dataposter till JSON

>[!INFO]
>
>**Exempel:** I följande exempel visas hur du omformar dataposter från [!DNL Google Sheets] till JSON-format:
>
>1. Placera [!DNL Google Sheets] > [!UICONTROL Select rows] i ditt scenario för att hämta data. Konfigurera modulen för att hämta rader från din [!DNL Google] kalkylblad. Ange &#x200B;**[!UICONTROL Maximum number of returned rows]** till ett litet tal, men större än ett för testningsändamål (exempel, tre). Kör [!DNL Google Sheets] genom att högerklicka och välja &quot;**[!UICONTROL Run this module only]**.&quot; Kontrollera modulens utdata.
>
1. Anslut [!UICONTROL Array Aggregator] modulen efter [!DNL Google Sheets] -modul. Välj [!DNL Google Sheets] i **[!UICONTROL Source node]** fält. Låt de andra fälten vara som de är för tillfället.
>
1. Anslut [!UICONTROL JSON] > [!UICONTROL Create JSON] modulen efter [!UICONTROL Array Aggregator] -modul. Modulens konfiguration kräver en datastruktur som beskriver JSON-formatet. Klicka **[!UICONTROL Add]** för att öppna datastrukturinställningarna. Det enklaste sättet att skapa den här datastrukturen är att generera den automatiskt från ett JSON-exempel. Klicka **[!UICONTROL Generator]** och klistra in JSON-exemplet i **[!UICONTROL Sample data]** fält:
>
**Exempel:**
>   
>```
>{
>
>"books": [
>
>{
>
>"id": "ID",
>
>"title": "Title",
>
>"author": "Author"
>
>}
>
>]
>
>}
>```
>
1. Klicka på **[!UICONTROL Save]**. The [!UICONTROL Specification] -fältet i datastrukturen innehåller nu den genererade strukturen.
1. Ändra namnet på datastrukturen till något mer specifikt och klicka på **[!UICONTROL Save]**. Ett fält som motsvarar rotarrayattributet visas som ett mappningsbart fält i JSON-modulens inställningar.
>
1. Klicka på **[!UICONTROL Map]** intill fältet och mappa `Array[]` objekt från Array-aggregatorns utdata till det.
>
1. Klicka **[!UICONTROL OK]** för att stänga [!UICONTROL JSON] modulens inställningar.
>
1. Öppna inställningarna för [!UICONTROL Array Aggregator] -modul. Ändra **[!UICONTROL Target structure]** från [!UICONTROL Custom] till [!UICONTROL JSON] modulens fält som motsvarar rotmatrisattributet. Mappa objekt från [!DNL Google Sheets] till lämpliga fält.
>
1. Klicka **[!UICONTROL OK]** för att stänga [!UICONTROL Array Aggregator] modulens inställningar.
>
1. Kör scenariot.
>
The [!UICONTROL JSON] returnerar rätt JSON-format.
>
1. Öppna inställningarna för [!DNL Google Sheets] och öka [!UICONTROL Maximum number of returned rows] talet vara större än antalet rader i kalkylbladet för att bearbeta alla data.

## Felsökning

### Det går inte att mappa data från [!UICONTROL Parse JSON] modul

Kontrollera att JSON-innehållet är korrekt mappat till [!UICONTROL Parse JSON] och att datastrukturen är korrekt definierad. Mer information finns i [Omvandla dataposter till JSON](#transforming-data-records-to-json) i den här artikeln.

### Modulen misslyckas när villkorssatser används i JSON

När du använder villkorssatser som `if` i JSON placerar citattecknen utanför villkorssatsen.

>[!INFO]
>
**Exempel:**
>
![](assets/quotes-in-json-350x120.png)
