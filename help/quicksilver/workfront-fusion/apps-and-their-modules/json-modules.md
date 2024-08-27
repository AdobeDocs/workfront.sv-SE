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
source-git-commit: 0290772c26ca82af31f14d101b4dde99377d6ce4
workflow-type: tm+mt
source-wordcount: '1084'
ht-degree: 0%

---

# [!UICONTROL JSON] moduler

Appen [!DNL Adobe Workfront Fusion] [!UICONTROL JSON] innehåller moduler som bearbetar data i JSON-format så att [!DNL Adobe Workfront Fusion] kan arbeta vidare med datainnehållet eller skapa nytt JSON-innehåll.

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
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

## Tolka JSON

* [Datastruktur](#data-structure)
* [Samling kontra matris](#collection-vs-array)

### Datastruktur

Datastrukturen beskriver hur JSON-data ordnas och möjliggör mappning av enskilda JSON-objekt till andra moduler i ditt scenario. Om du inte anger datastrukturen kan du köra modulen manuellt och [!DNL Workfront Fusion] skapar strukturen från den angivna JSON:

1. Lägg till modulen [!UICONTROL Parse JSON] i ett scenario.
1. I fältet **[!UICONTROL JSON String]** anger du den JSON som du vill bygga en datastruktur från.
1. Anslut inte andra moduler till modulen [!UICONTROL Parse JSON] än. Eftersom [!DNL Workfront Fusion] ännu inte känner till strukturen för JSON-data går det inte att mappa data från modulen [!UICONTROL Parse JSON] till andra moduler i ditt scenario.
1. Kör scenariot manuellt. Detta gör att modulen [!UICONTROL Parse JSON] kan identifiera JSON-strukturen från den JSON som du har angett.
1. Nu kan du ansluta följande moduler. Objekten från JSON-modulen Parse är nu tillgängliga för mappning.

Mer information finns i [Datastrukturer i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/data-structures.md).

### Samling kontra matris

Om JSON-strängfältet innehåller en samling `{ ... }` är utdata ett enda paket som innehåller objekten i samlingen.

>[!INFO]
>
>**Exempel:**
>
>```
>{
>       "name" : "Peter",
>
>    
   "ID" : 1
>}
>```
>
>![](assets/json-collection.png)

Om JSON-strängfältet innehåller arrayen `[ ... ]` är utdata en serie paket. varje paket innehåller ett element i arrayen.

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
 {
>       "name" : "Mike",
>       "ID" : 2
>   }
>]
>```
>
>![](assets/json-array.png)

## [!UICONTROL JSON]-moduler och deras fält

När du konfigurerar [!DNL JSON] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare JSON-fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

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
   <td>Definiera ett uttryck som du vill gruppera aggregerade utdata med. Det här uttrycket kan innehålla ett eller flera mappade objekt. De aggregerade data delas sedan upp i grupper med hjälp av det här uttryckets värde. Varje grupp skickar som ett separat paket med en nyckel (det utvärderade uttrycket) och ett värde (den sammanställda texten). Du kan använda nyckeln som ett filter i efterföljande moduler.</td> 
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
>1. Placera modulen [!DNL Google Sheets] > [!UICONTROL Select rows] i ditt scenario för att hämta data. Konfigurera modulen för att hämta rader från ditt [!DNL Google]-kalkylblad. Ställ in &#x200B;**[!UICONTROL Maximum number of returned rows]** på ett litet tal, men större än ett för testningsändamål (exempel, tre). Kör modulen [!DNL Google Sheets] genom att högerklicka på den och välja **[!UICONTROL Run this module only]**. Kontrollera modulens utdata.
>
1. Anslut modulen [!UICONTROL Array Aggregator] efter modulen [!DNL Google Sheets]. Välj modulen [!DNL Google Sheets] i fältet **[!UICONTROL Source node]** i modulens konfiguration. Låt de andra fälten vara som de är för tillfället.
>
1. Anslut [!UICONTROL JSON] > [!UICONTROL Create JSON] efter modulen [!UICONTROL Array Aggregator]. Modulens konfiguration kräver en datastruktur som beskriver JSON-formatet. Klicka på **[!UICONTROL Add]** för att öppna datastrukturinställningarna. Det enklaste sättet att skapa den här datastrukturen är att generera den automatiskt från ett JSON-exempel. Klicka på **[!UICONTROL Generator]** och klistra in JSON-exemplet i fältet **[!UICONTROL Sample data]**:
>
**Exempel:**
>
```
{

"books": [

{

"id": "ID",

"title": "Title",

"author": "Author"

}

]

}
```
>
1. Klicka på **[!UICONTROL Save]**. Fältet [!UICONTROL Specification] i datastrukturen innehåller nu den genererade strukturen.
1. Ändra namnet på datastrukturen till något mer specifikt och klicka på **[!UICONTROL Save]**. Ett fält som motsvarar rotarrayattributet visas som ett mappningsbart fält i JSON-modulens inställningar.
>
1. Klicka på knappen **[!UICONTROL Map]** bredvid fältet och mappa `Array[]`-objektet från Array-aggregatorns utdata till det.
>
1. Klicka på **[!UICONTROL OK]** för att stänga konfigurationen för modulen [!UICONTROL JSON].
>
1. Öppna konfigurationen för modulen [!UICONTROL Array Aggregator]. Ändra **[!UICONTROL Target structure]** från [!UICONTROL Custom] till fältet i modulen [!UICONTROL JSON] som motsvarar rotmatrisattributet. Mappa objekt från modulen [!DNL Google Sheets] till rätt fält.
>
1. Klicka på **[!UICONTROL OK]** för att stänga konfigurationen för modulen [!UICONTROL Array Aggregator].
>
1. Kör scenariot.
>
Modulen [!UICONTROL JSON] matar ut rätt JSON-format.
>
1. Öppna inställningarna för modulen [!DNL Google Sheets] och öka [!UICONTROL Maximum number of returned rows] så att det blir större än antalet rader i kalkylbladet för att bearbeta alla data.

## Felsökning

### Det går inte att mappa data från modulen [!UICONTROL Parse JSON]

Kontrollera att JSON-innehållet är korrekt mappat till modulen [!UICONTROL Parse JSON] och att datastrukturen är korrekt definierad. Mer information finns i [Omforma dataposter till JSON](#transforming-data-records-to-json) i den här artikeln.

### Modulen misslyckas när villkorssatser används i JSON

När du använder villkorssatser som `if` i JSON placerar du citattecknen utanför villkorssatsen.

>[!INFO]
>
**Exempel:**
>
![](assets/quotes-in-json-350x120.png)
