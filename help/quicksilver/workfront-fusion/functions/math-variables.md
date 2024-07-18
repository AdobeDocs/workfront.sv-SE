---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: functions
title: Matematiska variabler i  [!DNL Adobe Workfront Fusion]
description: Följande matematiska variabler är tillgängliga på  [!DNL Adobe Workfront Fusion mapping] panelen.
author: Becky
feature: Workfront Fusion
exl-id: 2fb561d2-0780-4fd6-87b3-5360a02df177
source-git-commit: c325e16ba0cde4cd48fc3e40358a9ea9ed310659
workflow-type: tm+mt
source-wordcount: '120'
ht-degree: 0%

---

# Matematiska variabler i [!DNL Adobe Workfront Fusion]

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

## pi

Representerar den matematiska symbolen $\pi$.

## [!UICONTROL random]

Returnerar ett pseudoslumpmässigt flyttal i intervallet [`0`,`1`] (inklusive `0`, men inte `1`).

Använd följande formel för att generera ett pseudoslumpmässigt heltal i intervallet [`min`,`max`] (inklusive både `min` och `max`):

![](assets/math-variable-random-350x61.png)

```
floor(random * (1.max - 1.min + 1)) + 1.min
```
