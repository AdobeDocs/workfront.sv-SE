---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Skapa nya mallar i [!DNL Adobe Workfront Fusion]
description: Du kan skapa nya scenariomallar i [!DNL Adobe] Workfront Fusion.
author: Becky
feature: Workfront Fusion
exl-id: fdfa509c-30c6-431e-89f3-a4bf50261e8a
source-git-commit: fcaa2136310cad8ef478020a9bae34bbe5520c6d
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Skapa nya mallar i [!DNL Adobe Workfront Fusion]

Du kan skapa nya scenariomallar i [!DNL Adobe] Workfront Fusion.

>[!TIP]
>
>Innan du skapar en ny mall kan du kontrollera [!UICONTROL Public templates] för att säkerställa att mallen som du vill skapa inte redan är tillgänglig.

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
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Skapa en ny mall

1. Klicka **[!UICONTROL Templates]** ![](assets/fusion-template-icon.png) i den vänstra navigeringspanelen.
1. Klicka **[!UICONTROL Create a new template]** i det övre högra hörnet.
1. (Valfritt) Byt namn på mallen genom att ersätta standardmallen **[!UICONTROL New template name]** i det övre vänstra hörnet.
1. (Valfritt) Om du vill ändra mallens språk klickar du på **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) och välj språk i listrutan Språk.

   >[!IMPORTANT]
   >
   >Valet Språk motsvarar de tillgängliga språken i systeminställningarna och gäller endast namnet på den offentliga mallen och dess beskrivning. Du kan inte ändra ett mallspråk när mallen har sparats.

1. (Valfritt) Om du vill ange en beskrivning av mallen klickar du på **[!UICONTROL Set up a template]** ![](assets/fusion-scenario-settings-icon.png) och ange beskrivningen.
1. Lägg till program, moduler och verktyg på samma sätt som när du skapar ett standardscenario.

   Information om hur du lägger till sammanhangsberoende hjälp till modulerna finns i [Konfigurera [!UICONTROL Wizard] funktionalitet](#set-up-wizard-functionality) i den här artikeln.

   Mer information om hur du skapar ett scenario finns i [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../../workfront-fusion/scenarios/create-a-scenario.md).

   >[!NOTE]
   >
   >Om mallen innehåller moduler som kräver att anslutningen, inloggningsuppgifterna eller annan sekretesskänslig information läggs till, delas informationen inte med mallanvändarna.

1. (Valfritt) Klicka på **[!UICONTROL Run once]** för att testa mallen.
1. Klicka på **[!UICONTROL Save]** icon ![](assets/save-icon.png).

>[!NOTE]
>
>Genom att spara mallen kan du göra den synlig för alla dina teammedlemmar. Om du vill att mallen ska vara tillgänglig utanför ditt team måste du publicera den och sedan använda en delad länk, eller be administratören att godkänna och publicera mallen.

## Konfigurera [!UICONTROL Wizard] funktionalitet {#set-up-wizard-functionality}

The [!DNL Workfront Fusion template] [!UICONTROL Wizard] gör att du kan ge framtida användare av mallen instruktioner eller information om de specifika fält som används i moduler.

1. Klicka på modulen som lagts till i mallen för att visa modulens fält.
1. Leta reda på fältet där du vill lägga till [!UICONTROL Wizard] information och aktivera **[!UICONTROL Use in Wizard]** för det fältet.
1. Ange den information som du vill göra synlig för användarna i [!UICONTROL Help] fält.
1. (Valfritt) Aktivera om du vill tillåta användare att se den här texten när de använder mallen **[!UICONTROL Use as default value]**.
1. Upprepa steg 2-4 för varje fält som du vill ange information för.
1. Klicka **[!UICONTROL OK]** om du vill spara ändringarna och stänga modulen.
