---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Välja var en utlösarmodul ska börja i Adobe Workfront Fusion
description: Vissa utlösarmoduler låter dig välja det första paket från vilket du vill att hämtningen av paket ska starta.
author: Becky
feature: Workfront Fusion
exl-id: 5ab7cac4-8d50-4be0-b26b-b832544f18f7
source-git-commit: e58ff769015b8c4e34b34eea653f55a296eea371
workflow-type: tm+mt
source-wordcount: '280'
ht-degree: 0%

---

# Välj var en utlösarmodul ska börja i [!DNL Adobe Workfront Fusion]

Vissa utlösarmoduler låter dig välja det första paket från vilket du vill att hämtningen av paket ska starta.

Du kan också ange om du vill hämta alla paket eller bara paketen från efter ett visst datum.

Mer information om utlösarmoduler finns i avsnittet [Utlösarmoduler](../../workfront-fusion/modules/module-types.md#triggers) i artikeln [Typer av moduler](../../workfront-fusion/modules/module-types.md).

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Välj var en utlösarmodul ska starta

1. Spara en utlösarmodul.

   eller

   Ändra inställningarna för utlösarmodulen enligt beskrivningen i [Konfigurera en moduls inställningar i [!UICONTROL Adobe Workfront Fusion]](../../workfront-fusion/modules/configure-a-modules-settings.md).

   eller

   Högerklicka på ikonen för utlösarmodulen i dialogrutan [!UICONTROL Scenario editor], enligt beskrivningen i [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

1. Välj ett alternativ i dialogrutan **[!UICONTROL Choose where to start]** som visas.

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
