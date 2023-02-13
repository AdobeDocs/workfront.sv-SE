---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Arrayfunktioner i Adobe Workfront Fusion
description: Följande arrayfunktioner är tillgängliga i panelen för mappning av Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: bf065d00-5d84-47e1-8169-bf9e01e2429d
source-git-commit: c57a796ccbfb36bce58d49345e7515dd524604c5
workflow-type: tm+mt
source-wordcount: '538'
ht-degree: 0%

---

# Arrayfunktioner i Adobe Workfront Fusion

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

## [!UICONTROL add (array; value1; value2; ...)]

Lägger till värden som anges i parametrar till en array och returnerar den arrayen.

## [!UICONTROL contains (array; value)]

Verifierar om en array innehåller värdet.

## [!UICONTROL distinct (array; [key])]

Tar bort dubbletter inuti en array. Använd &quot;[!UICONTROL key]-argument för att komma åt egenskaper inuti komplexa objekt. Använd punktnotation om du vill komma åt kapslade egenskaper. Det första objektet i en array är index 1.

>[!INFO]
>
>**Exempel:** `distinct(Contacts[];name)`
>
>Tar bort dubbletter i en array med kontakter genom att jämföra egenskapen name

## [!UICONTROL flatten (array)]

Skapar en ny array med alla underarrayelement sammanfogade rekursivt, upp till det angivna djupet.


## [!UICONTROL join (array; separator)]

Sammanfogar alla objekt i en array till en sträng med den angivna avgränsaren mellan varje objekt.

## [!UICONTROL keys (object)]

Returnerar en array med egenskaperna för ett givet objekt eller en angiven array.

## [!UICONTROL length (array)]

Returnerar antalet objekt i en array.

## [!UICONTROL map (complex array; key;[key for filtering];[possible values for filtering])]

Returnerar en primitiv array som innehåller värden för en komplex array. Den här funktionen tillåter filtrering av värden. Använd råa variabelnamn för nycklar.

>[!INFO]
>
>**Exempel:**
>
>* `map(Emails[];email)`
  >
>  Returnerar en primitiv array med e-post
>
>* `map(Emails[];email;label;work;home)`
  >
>  Returnerar en primitiv array med e-postmeddelanden som har en etikett som är lika med arbetet eller hemmet

Mer information finns i [Mappa information från en modul till en annan i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md)


## [!UICONTROL merge (array1; array2; ...)]

Sammanfogar en eller flera arrayer till en array.

## [!UICONTROL remove (array; value1; value2; ...)]

Tar bort värden som anges i parametrarna för en array. Den här funktionen gäller bara för primitiva arrayer med text eller siffror.

## [!UICONTROL reverse (array)]

Det första elementet i arrayen blir det sista elementet, det andra blir det näst sista och så vidare.

## [!UICONTROL slice (array; start; [end])]

Returnerar en ny array som endast innehåller markerade objekt.

## [!UICONTROL sort (array; [order]; [key])]

Sorterar värden i en array. Giltiga värden för `order` parametern är:

* `asc`

   (standard) - stigande ordning: 1, 2, 3, ... för typen Number. A, B, C, a, b, c, ... för text

* `desc`

   fallande ordning: ..., 3, 2, 1 för typen Number. ..., c, b, a, C, B, A för typen Text.

* `asc ci`

   skiftlägesokänslig stigande ordning: A, a, B, b, C, c, ... för text.

* `desc ci`

   skiftlägesokänslig fallordning: ..., C, c, B, b, A, a för typen Text.

Använd `key` -parameter för att komma åt egenskaper inuti komplexa objekt.

Använd råa variabelnamn för nycklar.

Använd punktnotation om du vill komma åt kapslade egenskaper.

Det första objektet i en array är index 1.

>[!INFO]
>
>**Exempel:**
>
>* `sort(Contacts[];name)`
   >
   >    Sorterar en array med kontakter efter egenskapen &quot;name&quot; i standardstigande ordning
>
>* `sort(Contacts[];desc;name)`
   >
   >   Sorterar en array med kontakter efter egenskapen &quot;name&quot; i fallande ordning
>
>* `sort(Contacts[];asc ci;name)`
   >
   >    Sorterar en array med kontakter efter egenskapen &quot;name&quot; i fallokänslig stigande ordning
>
>* `sort(Emails[];sender.name)`
   >
   >    Sorterar en matris med e-postmeddelanden efter egenskapen &quot;sender.name&quot;


## [!UICONTROL arrayDifference [array1, array2, mode]]

Returnerar skillnaden mellan två arrayer.

Ange ett av följande värden för `mode` parameter.

* `classic`: Returnerar en ny array som innehåller alla element i `array1` som inte finns i `array2`.

* `symmetric`: Returnerar en array med element som inte är gemensamma för båda arrayerna.

   Funktionen returnerar med andra ord en array som innehåller alla element i `array1` som inte finns i `array2`och alla element i `array2` som inte finns i `array1`.

   >[!INFO]
   >
   >**Exempel:**
   >
   >Följande arrayer:
   >
   >
   ```
   >myArray = [1,2,3,4,5]
   >```
   >
   >
   ```
   >yourArray = [3,4,5,6,7]
   >```
   >
   >* `arrayDifference [myArray, yourArray, classic]`
      >
      >    Returnerar `[1,2]`
   >
   >* `arrayDifference [yourArray, myArray, classic]`
      >
      >    Returnerar `[6,7]`
   >
   >* `arrayDifference [myArray, yourArray, symmetric]`
      >
      >    Returnerar `[1,2,6,7]`

