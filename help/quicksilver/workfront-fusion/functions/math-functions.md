---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Matematiska funktioner i Adobe Workfront Fusion
description: Följande matematiska funktioner är tillgängliga i panelen för mappning av Adobe Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: 8a3c7a89-62b5-45e9-b857-8beedd0e5af4
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '253'
ht-degree: 0%

---

# Matematiska funktioner i [!DNL Adobe Workfront Fusion]

<!--Audited: 4/2024-->

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

## [!UICONTROL average ([array of values]) average(value1; [value2], ...)]

Returnerar det genomsnittliga värdet för de numeriska värdena i en viss array, eller det genomsnittliga värdet för numeriska värden som anges individuellt.

## [!UICONTROL ceil (number)]

Returnerar det minsta heltalet som är större än eller lika med ett angivet tal.

>[!INFO]
>
>**Exempel:**
>
>* `ceil(` `1.2` `)`
>
>   Returnerar 2
>
>* `ceil(` `4` `)`
>
>   Returnerar 4

## [!UICONTROL floor (number)]

Returnerar det största heltalet mindre än eller lika med ett angivet tal.

>[!INFO]
>
>**Exempel:**
>
>* `floor(` `1.2` `)`
>
>   Returnerar 1
>
>* `floor(` `1.9` `)`
>
>   Returnerar 1
>
>* `floor(` `4` `)`
>
>   Returnerar 4

## [!UICONTROL max ([array of values]), max(value1;value2; ...)]

Returnerar det största talet i en angiven array eller det största talet bland tal som anges individuellt.

## [!UICONTROL min ([array of values]), min(value1; value2; ...)]

Returnerar det minsta talet i en angiven array eller det minsta talet bland tal som anges individuellt.

## [!UICONTROL round (number)]

Avrundar ett numeriskt värde till närmaste heltal.

>[!INFO]
>
>**Exempel:**
>
>* `round(` `1.2` `)`
>
>   Returnerar 1
>
>* `round(` `1.5` `)`
>
>   Returnerar 2
>
>* `round(` `1.7` `)`
>
>   Returnerar 2
> 
>* `round(` `2` `)`
>
>   Returnerar 2

## [!UICONTROL sum ([array of values]), sum(value1; value2; ...)]

Returnerar summan av värdena i en angiven array eller summan av talen som anges individuellt.

## [!UICONTROL parseNumber (number; decimal separator)]

Tolkar en sträng med ett tal och returnerar talet. parseNumber(1 756,456;,)

## [!UICONTROL formatNumber (number; decimalPOINTS; [decimalSeparator]; [thousandsSeparator])]

Returnerar ett tal i begärt format. Som standard är decimalkommat ett komma (,) och tusentalsavgränsaren är en punkt (.).

>[!INFO]
>
>**Exempel:**
>
>`formatNumber( 123456789 ; 3 ; , ; . )`
>
>Returnerar 123,456,789,000
