---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Välja var en utlösarmodul ska börja i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Välj var en utlösarmodul ska börja i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Välj var en utlösarmodul ska starta](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/choose-where-trigger-module-starts.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Vissa utlösarmoduler låter dig välja det första paket från vilket du vill att hämtningen av paket ska starta.

Du kan också ange om du vill hämta alla paket eller bara paketen från efter ett visst datum.

Mer information om utlösarmoduler finns i avsnittet [Utlösarmoduler](../../workfront-fusion/modules/module-types.md#triggers) i artikeln [Typer av moduler](../../workfront-fusion/modules/module-types.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

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

+++

## Välj var en utlösarmodul ska starta

1. Spara en utlösarmodul.

   eller

   Ändra inställningarna för utlösarmodulen enligt beskrivningen i [Konfigurera inställningarna för en modul i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   eller

   Högerklicka på ikonen för utlösarmodulen i [!UICONTROL Scenario editor], enligt beskrivningen i [Skapa ett scenario i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Välj ett alternativ i rutan **[!UICONTROL Choose where to start]** som visas.

   ![](assets/choose-where-to-start-350x346.jpg)

   Vilka alternativ som visas beror på möjligheterna med en viss tjänst. De kan omfatta följande:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL From now on] (standard)</td>
            <td>Hämtar alla paket som lagts till eller uppdaterats (beroende på inställningar) från och med nu</td>
        </tr>
        <tr>
            <td>[!UICONTROL From after a specific date]</td>
            <td>Hämtar alla paket som lagts till eller uppdaterats (beroende på inställningar) efter ett angivet datum/tid</td>
        </tr>
        <tr>
            <td>[!UICONTROL With ID greater than or equal to a specific value]</td>
            <td>Hämtar alla paket med ett ID som är större än eller lika med ett angivet ID</td> 
        </tr>
        <tr>
            <td>[!UICONTROL All bundles]</td>
            <td>Hämtar alla tillgängliga paket</td>
        </tr>
        <tr>
            <td>[!UICONTROL Select the first bundle]</td>
            <td>Gör att du kan välja det första paket från vilket hämtningen av paket ska börja</td>
        </tr>
   </table>
