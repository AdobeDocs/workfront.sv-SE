---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Schemalägg ett scenario i Adobe Workfront Fusion
description: Som standard körs ett scenario var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta ett aktiverat scenario körs.
author: Becky
feature: Workfront Fusion
exl-id: bce89abe-ec37-4705-a88f-de62c8b27f49
source-git-commit: f5549be5951a2648d6a77d25bebbd4141f18d36c
workflow-type: tm+mt
source-wordcount: '523'
ht-degree: 0%

---

# Schemalägg ett scenario i [!DNL Adobe Workfront Fusion]

Som standard körs ett scenario var 15:e minut. Du kan ändra detta genom att definiera när och hur ofta ett aktiverat scenario körs. Fusionsscenarier kan schemaläggas så att de körs så ofta som var femte minut.

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
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td>    </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Schemalägg ett scenario

1. Klicka på i det övre högra hörnet på sidan Scenariodetaljer **[!UICONTROL Options]** > **[!UICONTROL Scheduling]**

   eller

   Klicka på **[!UICONTROL Scheduling]** -ikon (klocka) i scenariots utlösarmodul.

1. Ange information i följande fält:

   <table style="table-layout:auto">   
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Run scenario]</td> 
      <td> <p>Välj med vilken frekvens du vill köra scenariot och välj sedan intervallet.</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL At regular intervals]</strong> </p> <p>Ange antalet minuter mellan körningar. Standardvärdet är 15 minuter.</p> </li> 
        <li> <p><strong>[!UICONTROL Once]</strong> </p> <p>Ange det datum och den tidpunkt då du vill att scenariot ska köras. Använd formatet <code>MM/DD/YYYY h:mm A</code>. Exempel: <code>06/25/2019 11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Every day]</strong> </p> <p>Ange den tidpunkt då du vill att scenariot ska köras. Använd formatet <code>h:mm A</code>. Exempel: <code>11:00 PM</code>.</p> </li> 
        <li> <p><strong>[!UICONTROL Days of the week]</strong> </p> <p>Dagar: Välj de veckodagar som du vill att scenariot ska köras. Du kan välja en eller flera dagar.</p> <p>Tid: Ange den tidpunkt då du vill att scenariot ska köras på de valda dagarna. Använd formatet <code>h:mm A</code>. Exempel: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Days of the month]</strong> </p> <p>Dagar: Välj de dagar i månaden som du vill att scenariot ska köras. Du kan välja en eller flera dagar.</p> <p>Tid: Ange den tidpunkt då du vill att scenariot ska köras på de valda dagarna. Använd formatet <code>h:mm A</code>. Exempel: <code>11:00 PM</code></p> </li> 
        <li> <p><strong>[!UICONTROL Specified dates]</strong> </p> <p>Månader: Välj de månader som du vill köra scenariot. Du kan välja en eller flera månader.</p> <p>Dagar: Välj de dagar i månaden som du vill att scenariot ska köras. Du kan välja en eller flera dagar.</p> <p>Tid: Ange den tidpunkt då du vill att scenariot ska köras på de valda dagarna. Använd formatet <code>h:mm A</code>. Exempel: <code>11:00 PM</code></p> </li> 
       </ul> <p>Obs! Det måste finnas ett datum för att ett scenario ska kunna köras på det datumet. Ett scenario som till exempel bara är schemalagt för den 31:e månaden kommer inte att köras i februari, april, juni, september eller november eftersom dessa månader inte har en 31:a dag.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Advanced scheduling]</td> 
      <td>Du kan definiera tidsintervall under vilka ditt scenario ska köras. Du kan ange tidsintervall, veckodagar eller månader. För varje intervall klickar du <strong>[!UICONTROL Add]</strong> och fylla i fälten enligt beskrivningen i [!UICONTROL Run scenario] fält.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start]</td> 
      <td>Ange det datum och den tidpunkt efter vilken du vill att scenariot ska köras. Använd formatet <code>MM/DD/YYYY h:mm A</code>. Exempel: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL End]</td> 
      <td>Ange det datum och den tidpunkt då du vill att scenariot ska köras. Använd formatet <code>MM/DD/YYYY h:mm A</code>. Exempel: <code>06/25/2019 11:00 PM</code>.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **[!UICONTROL OK]** för att spara schemainställningarna och återgå till scenariot.
