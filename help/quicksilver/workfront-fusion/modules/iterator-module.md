---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: modules
title: Iterator-modulen i Adobe Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: d356276d-e5d9-496f-85cd-cb60a8f8f377
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---

# [!UICONTROL Iterator]-modulen i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Iteratormodul](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/modules/iterator-module.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

En [!UICONTROL Iterator]-modul är en särskild typ av modul som konverterar en array till en serie paket. Varje arrayobjekt genereras som ett separat paket.

Mer information finns i [Typer av moduler](../../workfront-fusion/modules/module-types.md) och [Mappa en array i Adobe Workfront Fusion](../../workfront-fusion/mapping/map-an-array.md).

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för Automatisering och integrering av arbetet] </p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både Adobe Workfront Fusion och Adobe Workfront för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Modulkonfiguration för [!UICONTROL Iterator]

Du konfigurerar en [!UICONTROL Iterator]-modul på samma sätt som du konfigurerar andra moduler. Fältet [!UICONTROL Array] innehåller arrayen som ska konverteras eller delas upp i separata paket.

![](assets/set-up-iterator-350x190.jpg)

Mer information finns i [Konfigurera en moduls inställningar i Adobe Workfront Fusion](../../workfront-fusion/modules/configure-a-modules-settings.md).

>[!INFO]
>
>**Exempel:**
>
>* I nedanstående scenario visas hur du hämtar e-postmeddelanden med bilagor och sparar de bifogade filerna som enskilda filer i en vald [!DNL Dropbox]-mapp.
>
>   E-postmeddelanden kan innehålla en array med bilagor. Modulen [!UICONTROL Iterator] som infogats efter den första modulen gör att du kan hantera varje bifogad fil separat. Modulen [!UICONTROL Iterator] delar upp arrayen med bilagor i enskilda paket. Varje paket, med en bifogad fil, sparas sedan en i taget i en markerad [!DNL Dropbox]-mapp. [!UICONTROL Iterator]-modulens konfiguration visas ovan: [!UICONTROL Array]-fältet ska innehålla `Attachments`-arrayen.
>
>   ![](assets/attachments-array-350x154.jpg)
>
>* För enkelhetens skull erbjuder många [!DNL Workfront Fusion]-appar specialiserade [!UICONTROL Iterator]-moduler med en förenklad konfiguration. Appen [!UICONTROL Email] innehåller till exempel den speciella [!UICONTROL Iterator] module [!UICONTROL Email] > [!UICONTROL Iterate attachments] som ger samma resultat som den allmänna [!UICONTROL Iterator]-modulen.
>
>   ![](assets/specialized-iterators-350x135.jpg)


## Felsökning: Mappningspanelen visar inte mappningsbara objekt i modulen [!UICONTROL Iterator]

När en [!UICONTROL Iterator]-modul inte har information om strukturen för arrayens objekt, visar mappningspanelen i modulerna efter [!UICONTROL Iterator]-modulen endast två objekt under [!UICONTROL Iterator]-modulen: `Total number of bundles` och `Bundle order position`:

![](assets/mapping-panel-doesnt-display-350x147.png)

Detta beror på att varje modul ansvarar för att tillhandahålla information om de objekt den matar ut, så att dessa objekt kan visas korrekt på mappningspanelen i efterföljande moduler. Det kan dock hända att flera moduler inte kan tillhandahålla den här informationen i vissa fall, till exempel [!UICONTROL JSON] > [!UICONTROL Parse JSON] eller [!UICONTROL Webhooks] > [!UICONTROL Custom Webhook] moduler som saknar datastruktur.

Lösningen är att manuellt köra scenariot för att få modulen att lära sig mer om de objekt den matar ut så att den kan ge information till följande moduler.

Om du till exempel har en [!UICONTROL JSON] > [!UICONTROL Parse JSON]-modul utan datastruktur enligt nedan:

![](assets/json-parse-json-350x285.png)

Om du ansluter en [!UICONTROL Iterator]-modul till den kan du inte mappa modulens utdata till fältet Array på inställningspanelen i modulen [!UICONTROL Iterator] :

![](assets/connect-iterator-module-350x146.png)

Du löser detta genom att starta scenariot manuellt i scenarioredigeraren. Du kan bryta länken mellan modulerna efter modulen [!UICONTROL JSON] > [!UICONTROL Parse JSON] för att förhindra att flödet fortsätter. Du kan också högerklicka på modulen [!UICONTROL JSON] > [!UICONTROL Parse JSON] och välja **[!UICONTROL Run this module only]** på snabbmenyn om du bara vill köra modulen [!UICONTROL JSON] > [!UICONTROL Parse JSON] .

När [!UICONTROL JSON] > [!UICONTROL Parse JSON] körs lär den sig om de objekt som den matar ut och skickar informationen till alla efterföljande moduler, inklusive Iterator-modulen. Mappningspanelen i Iteratorns inställningar visar sedan objekten:

![](assets/mapping-panel-displays-items-350x131.png)

Mappningspanelen i modulerna som är anslutna efter modulen [!UICONTROL Iterator] visar dessutom objekten som finns i arrayens objekt:

![](assets/items-contained-in-array-350x156.png)

Om du inte kan se vissa objekt på mappningspanelen i en modul kör du scenariot en gång så att alla moduler kan lära sig mer om de objekt de genererar och ge den här informationen till följande moduler.
