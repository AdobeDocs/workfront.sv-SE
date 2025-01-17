---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: connections-annd-webhooks
title: Anslut [!DNL Adobe Workfront Fusion] till valfri webbtjänst
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 8b2a7d85-e20e-4836-8418-3463d284194e
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '259'
ht-degree: 0%

---

# Anslut [!DNL Adobe Workfront Fusion] till valfri webbtjänst

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artiklarna:
>
>* [Anslut Adobe Workfront Fusion till en webbtjänst som använder API-tokenauktorisering](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/connect-to-applications/connect-wf-web-service-uses-api-token-auth.html)
>* [Konfigurera en webkrok för en webbtjänst utan anslutning](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/receive-a-webhook-from-a-web-service.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

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

Om [!DNL Adobe Workfront Fusion] inte erbjuder någon app för webbtjänsten som du vill använda i ditt scenario kan du ansluta till webbtjänsten med hjälp av [!DNL Workfront Fusion] HTTP- och Webhooks-moduler, vilket förklaras i följande artiklar:

* [Anslut [!DNL Adobe Workfront Fusion] till en webbtjänst som använder API-tokenauktorisering](../../workfront-fusion/connections/connect-wf-web-service-uses-api-token-auth.md)
* [Ta emot en webkrok från en webbtjänst](../../workfront-fusion/connections/receive-a-webhook-from-a-web-service.md)
