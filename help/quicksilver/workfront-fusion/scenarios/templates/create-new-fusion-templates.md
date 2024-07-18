---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Skapa nya mallar i  [!DNL Adobe Workfront Fusion]
description: Du kan skapa nya scenariomallar i  [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: f3f34e807228b299c0570e63bdf329f4e20e0340
workflow-type: tm+mt
source-wordcount: '729'
ht-degree: 0%

---

# Skapa nya mallar i [!DNL Adobe Workfront Fusion]

Du kan skapa nya scenariomallar i [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Innan du skapar en ny mall kan du kontrollera fliken [!UICONTROL Public templates] för att se till att mallen som du vill skapa inte redan är tillgänglig.

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
  <td>
   <p>Aktuellt licenskrav: Inget [!DNL Workfront Fusion]-licenskrav.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet], [!UICONTROL [!DNL Workfront Fusion] för Automatisering av arbete]</p>
   </td>    </tr> 
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

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Skapa en ny mall

Du kan skapa en mall på ungefär samma sätt som när du skapar ett scenario. Fusion-administratörer kan också skapa mallar från befintliga scenarier.

* [Skapa en mall](#build-a-template)
* [Skapa en mall från ett scenario](#create-a-template-from-a-scenario)

### Skapa en mall

1. Klicka på **[!UICONTROL Templates]** ![](assets/fusion-template-icon.png) i den vänstra navigeringspanelen.
1. Klicka på **[!UICONTROL Create a new template]** i det övre högra hörnet.
1. (Valfritt) Byt namn på mallen genom att ersätta standardvärdet **[!UICONTROL New template name]** i det övre vänstra hörnet.
1. (Valfritt) Om du vill ändra språk för mallen klickar du på **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) och väljer språk i listrutan Språk.

   >[!IMPORTANT]
   >
   >Valet Språk motsvarar de tillgängliga språken i systeminställningarna och gäller endast namnet på den offentliga mallen och dess beskrivning. Du kan inte ändra ett mallspråk när mallen har sparats.

1. (Valfritt) Om du vill ange en beskrivning av mallen klickar du på **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) och anger beskrivningen.
1. Lägg till program, moduler och verktyg på samma sätt som när du skapar ett standardscenario.

   Mer information om hur du lägger till sammanhangsbaserad hjälp till modulerna finns i [Konfigurera [!UICONTROL Wizard]-funktioner](#set-up-wizard-functionality) i den här artikeln.

   Mer information om hur du skapar ett scenario finns i [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Om mallen innehåller moduler som kräver att anslutningen, inloggningsuppgifterna eller annan sekretesskänslig information läggs till, delas informationen inte med mallanvändarna.

1. (Valfritt) Klicka på **[!UICONTROL Run once]** om du vill testa mallen.
1. Klicka på ikonen **[!UICONTROL Save]** ![](assets/save-icon.png).

>[!NOTE]
>
>Genom att spara mallen kan du göra den synlig för alla dina teammedlemmar. Om du vill att mallen ska vara tillgänglig utanför ditt team måste du skicka in en begäran om att den ska godkännas och publiceras. Begäran kommer till Adobe Workfront för godkännande och när den har godkänts är mallen tillgänglig för andra utanför teamet.
>
>Mer information om publiceringsmallar finns i [Publish och dela [!DNL Adobe Workfront Fusion] mallar](/help/quicksilver/workfront-fusion/scenarios/templates/publish-and-share-fusion-templates.md).

### Skapa en mall från ett scenario

>[!NOTE]
>
>Du måste vara en Fusion-administratör för att kunna skapa en mall från ett scenario.

1. Öppna sidan med scenarioinformation för det scenario som du vill skapa ett scenario från.
1. Klicka på listrutan **Admin** uppe till höger på sidan.
1. Välj **Klona som mall**.

   Scenariot kopieras till en ny mallsida.
1. (Valfritt) Byt namn på mallen genom att ersätta standardvärdet **[!UICONTROL New template name]** i det övre vänstra hörnet.
1. (Valfritt) Om du vill ändra språk för mallen klickar du på **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) och väljer språk i listrutan Språk.

   >[!IMPORTANT]
   >
   >Valet Språk motsvarar de tillgängliga språken i systeminställningarna och gäller endast namnet på den offentliga mallen och dess beskrivning. Du kan inte ändra ett mallspråk när mallen har sparats.

1. (Valfritt) Om du vill ange en beskrivning av mallen klickar du på **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) och anger beskrivningen.
1. Redigera program, moduler och verktyg på samma sätt som när du redigerar ett standardscenario.

   Mer information om hur du lägger till sammanhangsbaserad hjälp till modulerna finns i [Konfigurera [!UICONTROL Wizard]-funktioner](#set-up-wizard-functionality) i den här artikeln.

   >[!NOTE]
   >
   >Om mallen innehåller moduler som kräver att anslutningen, inloggningsuppgifterna eller annan sekretesskänslig information läggs till, delas informationen inte med mallanvändarna.

1. (Valfritt) Klicka på **[!UICONTROL Run once]** om du vill testa mallen.
1. Klicka på ikonen **[!UICONTROL Save]** ![](assets/save-icon.png).

## Konfigurera [!UICONTROL Wizard]-funktioner {#set-up-wizard-functionality}

Med [!DNL Workfront Fusion template] [!UICONTROL Wizard] kan du ge framtida användare av mallen instruktioner eller information om de specifika fält som används i moduler.

1. Klicka på modulen som lagts till i mallen för att visa modulens fält.
1. Leta reda på fältet där du vill lägga till [!UICONTROL Wizard]-information och aktivera **[!UICONTROL Use in Wizard]** för det fältet.
1. Ange den information som du vill göra synlig för användare i fältet [!UICONTROL Help].
1. (Valfritt) Aktivera **[!UICONTROL Use as default value]** om du vill tillåta användare att se den här texten när de använder mallen.
1. Upprepa steg 2-4 för varje fält som du vill ange information för.
1. Klicka på **[!UICONTROL OK]** om du vill spara ändringarna och stänga modulen.
