---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Hantera låsta scenarier i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 5fccf336-d904-43fe-ad4a-c3ce76dbcad0
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '395'
ht-degree: 0%

---

# Hantera låsta scenarier i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Hantera låsta scenarier](https://experienceleague.adobe.com/docs/workfront-fusion/using/manage-scenarios/view-manage-locked-scenario.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

I vissa fall kan ett scenario vara tillfälligt låst i [!DNL Workfront Fusion]. Låsta körningar låses upp automatiskt inom 2-4 timmar. Du kan även låsa upp scenarier manuellt.

>[!IMPORTANT]
>
>Om du låser upp ett scenario manuellt kan det orsaka fel i körningarna av ett scenario.

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
  <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p><p>[!UICONTROL [!DNL Workfront Fusion] for Work Automation] </p>  </td>    </tr> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Låsta scenarier

Scenarier kan vara låsta av flera anledningar.

Workfront Fusion stöder inte parallell bearbetning av schemalagda scenarier. Dessa scenarier är låsta i början av scenariot och olåsta när det är klart. Om körningen avbryts kanske scenariot inte låses upp. Detta kan inträffa när en användare manuellt framtvingar ett stopp av scenariot eller när det uppstår ett systemproblem.

Dessutom kan Workfront Fusion Engineering Team låsa ett scenario eftersom det orsakar prestandaproblem eller andra problem.

Oavsett orsaken till ett låst scenario låses scenariot upp automatiskt 2-4 timmar efter att det är låst.

## Lås upp ett låst scenario

Låsta scenarier låser upp 2-4 timmar från den tidpunkt de låstes. Du kan låsa upp ett scenario manuellt innan det är schemalagt att låsas upp automatiskt.

Om du låser upp ett scenario manuellt kan det orsaka fel i körningarna av ett scenario. Vi rekommenderar att du endast låser upp scenarier manuellt när ett scenario är låst på grund av att körningar körs och stoppas som en del av utformningen av scenariot. I andra fall rekommenderar vi att du väntar på att scenariot ska låsas upp automatiskt.

>[!IMPORTANT]
>
>Om du låser upp ett scenario manuellt kan det orsaka fel i körningarna av ett scenario.

1. Gå till sidan Scenarioinformation i det låsta scenariot.
1. Klicka på **[!UICONTROL Options]** i skärmens övre högra hörn.
1. Välj **[!UICONTROL Unlock execution]**.
1. Klicka på **[!UICONTROL Unlock]**.
