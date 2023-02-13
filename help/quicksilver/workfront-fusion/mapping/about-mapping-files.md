---
content-type: overview
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Om att mappa filer i [!DNL Adobe Workfront Fusion]
description: Vissa moduler kan bearbeta filer. Dessa moduler kan antingen returnera en utdatafil som ska skickas för vidare bearbetning eller kräva att en fil skickas till dem för bearbetning. Innan dessa moduler kan användas tillsammans för att bearbeta filer måste de mappas till varandra.
author: Becky
feature: Workfront Fusion
exl-id: 9ed5f176-86d8-4139-b582-c2f58aaed8d4
source-git-commit: 97f91d663df86341a079894cff04d07c18b7bf08
workflow-type: tm+mt
source-wordcount: '404'
ht-degree: 0%

---

# Om att mappa filer i [!DNL Adobe Workfront Fusion]

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr>  </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Mappningsfiler

Moduler som kan arbeta med filer kräver två informationsdelar:

* Filnamn
* Filinnehåll (data)

När du mappar en fil väljer du de moduler i ditt scenario från vilka du vill hämta data. Filnamnet och filinnehållet mappas sedan automatiskt som de är.

>[!NOTE]
>
>Om du behöver bearbeta en fil från en URL rekommenderar vi att du använder `HTTP > Get a File` för att hämta filen från URL:en och sedan mappa filen från `HTTP > Get a File` till den önskade modulens fält i ditt scenario.

>[!INFO]
>
>**Exempel:** I det här exemplet visas hur du hämtar dokument från [!DNL Adobe Workfront] till [!DNL Google Drive]. The [!DNL Workfront] trigger [!UICONTROL Watch Record] returnerar detaljerad information om varje dokument, inklusive namn och ID.
>
>Nästa modul, [!UICONTROL Download Document]hämtar , faktiska data så att de kan överföras till Google Drive.
>
>Mappa informationen till [!DNL Google Drive] så att den kan överföras måste du ange från vilken källfil informationen ska mappas. Om du väljer [!DNL Workfront] > [!UICONTROL Download Document] alternativ under källfilen, [!DNL Workfront Fusion] mappar filnamnet och filinnehållet så att dokumentet från [!DNL Workfront] överförs till den angivna Google-mappen.
>
>![](assets/wf-download-document-350x605.png)
>
>Men om du vill byta namn på filen, men behålla data som de är, kan du använda [!UICONTROL Map] om du vill mappa filnamnet och filinnehållet separat. Du anger det fullständiga filnamnet, inklusive tillägget. Textformat och binära format som foton, videoklipp och PDF stöds.
>
>![](assets/use-the-map-option-350x358.png)
