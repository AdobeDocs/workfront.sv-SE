---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Om att mappa filer i  [!DNL Adobe Workfront Fusion]
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '472'
ht-degree: 0%

---

# Om att mappa filer i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Mappa en fil mellan moduler](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-files.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Vissa moduler kan bearbeta filer. Dessa moduler kan antingen returnera en utdatafil som ska skickas för vidare bearbetning eller kräva att en fil skickas till dem för bearbetning. Innan dessa moduler kan användas tillsammans för att bearbeta filer måste de mappas till varandra.

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
   <td>
   <p>Aktuellt produktkrav: Om du har planen [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] måste din organisation köpa både [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i planen [!UICONTROL Ultimate] [!DNL Workfront].</p>
   <p>eller</p>
   <p>Äldre produktkrav: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] för att kunna använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr>  </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mappningsfiler

Moduler som kan arbeta med filer kräver två informationsdelar:

* Filnamn
* Filinnehåll (data)

När du mappar en fil väljer du de moduler i ditt scenario från vilka du vill hämta data. Filnamnet och filinnehållet mappas sedan automatiskt som de är.

>[!NOTE]
>
>Om du behöver bearbeta en fil från en URL rekommenderar vi att du använder modulen `HTTP > Get a File` för att hämta filen från URL:en och sedan mappar filen från modulen `HTTP > Get a File` till fältet för den önskade modulen i ditt scenario.

>[!INFO]
>
>**Exempel:** I det här exemplet visas hur du hämtar dokument från [!DNL Adobe Workfront] till [!DNL Google Drive]. [!DNL Workfront]-utlösaren [!UICONTROL Watch Record] returnerar detaljerad information om varje dokument, inklusive dess namn och ID.
>
>Nästa modul, [!UICONTROL Download Document], hämtar faktiska data så att de kan överföras till Google Drive.
>
>Om du vill mappa den här informationen till [!DNL Google Drive] så att den kan överföras måste du ange källfilen som informationen ska mappas från. Om du väljer alternativet [!DNL Workfront] > [!UICONTROL Download Document] under källfilen mappar [!DNL Workfront Fusion] filnamnet och filinnehållet så att dokumentet från [!DNL Workfront] överförs till den angivna Google-mappen.
>
>![](assets/wf-download-document-350x605.png)
>
>Om du vill byta namn på filen, men behålla data som de är, kan du använda alternativet [!UICONTROL Map] för att mappa filnamnet och filinnehållet separat. Du anger det fullständiga filnamnet, inklusive tillägget. Textformat och binära format som foton, videoklipp och PDF stöds.
>
>![](assets/use-the-map-option-350x358.png)
