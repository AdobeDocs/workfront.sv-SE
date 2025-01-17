---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: scenarios
title: Lägg till ett filter i ett scenario i  [!DNL Adobe] Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 114ab37f-71e0-494e-9f3d-93ff5a9d13ba
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '585'
ht-degree: 0%

---

# Lägg till ett filter i ett scenario i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Lägg till ett filter i ett scenario](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/add-modules/add-a-filter-to-a-scenario.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

I vissa scenarier behöver du bara arbeta med paket som uppfyller specifika kriterier. Med filter kan du välja dessa paket.

<!--

For example, you could create a scenario with the [!UICONTROL Watch records] trigger for [!DNL Salesforce] to capture only records containing a specific word written by a specific author.

-->

Du kan lägga till ett filter mellan två moduler och kontrollera om paket som tagits emot från de föregående modulerna uppfyller specifika filtervillkor:

* Om de gör det skickas paketen vidare till nästa modul i scenariot.
* Om de inte gör det avslutas behandlingen för paketen.

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

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Förutsättningar

Du måste lägga till båda modulerna i ett scenario innan du kan lägga till ett filter mellan dem.

## Lägg till ett filter mellan två moduler:

1. Klicka på **[!UICONTROL Scenarios]** ![](assets/scenarios-icon.png) i den vänstra panelen och välj sedan scenariot för att öppna det.
1. Klicka på **[!UICONTROL Edit]** i fönstrets övre högra hörn.
1. Klicka på kopplingslinjen mellan modulerna.
1. Skriv **[!UICONTROL Label]** som filter i rutan som visas.
1. Definiera ett filter **[!UICONTROL Condition]**.

   Du kan ange en eller två operander i de två rutorna. Om du anger operander i båda rutorna kan du välja en operator i listrutan mellan dem för att ange relationen mellan dem.

   >[!TIP]
   >
   >I operandfälten kan du ange värden på samma sätt som du skulle mappa dem, vilket beskrivs i [Mappa information från en modul till en annan i  [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

   Om du till exempel vill att filtret ska hitta filer i [!DNL Adobe Workfront] som slutar med XML och skicka dem vidare till [!DNL Dropbox] anger du **[!UICONTROL File name]** i den första rutan och .**[!UICONTROL xml]** i den andra rutan. I listrutan mellan dem väljer du **[!UICONTROL Ends with (case insensitive)]**. Det här filtret gäller inkommande paket från den första modulen (Workfront). Endast paket som innehåller XML-filer överförs till nästa modul ([!DNL Dropbox]).

   ![](assets/set-up-filter-box-350x368.jpg)

1. Klicka på **[!DNL OK]**.

## Kopiera ett filter

Scenarioredigeraren innehåller för närvarande ingen funktion för att kopiera ett filter.

>[!NOTE]
>
>Om du kopierar modulerna på någon sida av filtret kopieras även filtret.
>
>Mer information om att kopiera moduler finns i [Kopiera moduler eller scenarier i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/copy-modules-or-scenarios.md)

Om du vill kopiera ett filter utan att kopiera moduler kan du använda [!DNL Google] Chrome för följande tillfällig lösning:

1. Installera tillägget [!UICONTROL [!DNL Adobe Workfront Fusion] DevTool Chrome].
1. Öppna scenariot i [!DNL Workfront Fusion].
1. Klicka på Chrome trepunktsmeny och klicka sedan på **[!UICONTROL More tools*]* > **[!UICONTROL Developer tools]**.

1. Klicka på fliken [!UICONTROL Workfront Fusion] på menyraden längst upp på panelen [!UICONTROL Developer tools] som visas.

   ![](assets/copy-a-filter-350x174.png)

1. Klicka på ikonen **[!UICONTROL Tools]** ![](assets/devtools-tools-icon.png) i det vänstra fältet.

1. Klicka på **[!UICONTROL Copy Filter]** och konfigurera sedan verktyget **[!UICONTROL Copy Filter]** på den högra panelen:

   1. Ange **[!UICONTROL Source Module]** som modul direkt efter det filter du vill kopiera.
   1. Ange **[!UICONTROL Target Module]** som modul precis före det filter du vill kopiera.

1. Klicka på **[!UICONTROL Run]**.
