---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: apps-and-their-modules
title: Arkivera moduler
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: e29b6d39-3666-4d6d-a178-1983ae9f3aa9
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '534'
ht-degree: 0%

---

# [!UICONTROL Archive] moduler

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Arkivera moduler](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/tools-and-transformers/archive-modules.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

I ett [!DNL Adobe Workfront Fusion]-scenario kan du använda ett arkiv, t.ex. en zippad fil, i ditt scenario, så att du kan använda det i dina automatiseringar eller integreringar.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md). Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

## [!UICONTROL Archive]-moduler och deras fält

När du konfigurerar [!UICONTROL Archive] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!UICONTROL Archive] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [[!UICONTROL Extract an archive]](#extract-an-archive)
* [[!UICONTROL Create an archive]](#create-an-archive)
* [[!UICONTROL Inflate]](#inflate)
* [[!UICONTROL Deflate]](#deflate)

## [!UICONTROL Extract an archive]

Denna åtgärdsmodul extraherar en fil som du identifierar från ett arkiv.

Modulen returnerar filens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p> Markera den fil som du vill extrahera. Den här filen kan mappas från en tidigare modul (till exempel modulen [!DNL Workfront] &gt;[!UICONTROL Download a document]).</p>  </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:** Hämta ZIP-filen från den definierade [!DNL Dropbox]-mappen (till exempel Arkiv), extrahera den med modulen [!UICONTROL Archive] och skicka extraherade filer till den önskade e-postadressen som bilagor med modulen [!UICONTROL Email] eller [!DNL Gmail].
>
>![](assets/example-dropbox-350x134.png)

## [!UICONTROL Create an archive]

Den här aggregeringsmodulen lägger till önskade filer i ett [!UICONTROL ZIP]- eller [!UICONTROL TAR]-arkiv.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Source module]</td> 
   <td> <p> Markera modulen som du vill hämta filerna från.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type] </td> 
   <td> <p>Välj om du vill lägga till filer i ett [!UICONTROL ZIP]-arkiv eller ett [!UICONTROL TAR]-arkiv.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Comment]</td> 
   <td>Skriv en kommentar som du vill lägga till i arkivet.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Group by]</td> 
   <td> <p>Definiera ett uttryck som du vill gruppera aggregerade utdata med. Det här uttrycket kan innehålla ett eller flera mappade objekt. De aggregerade data delas sedan upp i grupper med hjälp av det här uttryckets värde. Varje grupp skickar som ett separat paket med en nyckel (det utvärderade uttrycket) och ett värde (den sammanställda texten). Du kan använda nyckeln som ett filter i efterföljande moduler.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Stop processing after an empty aggregation]</td> 
   <td>Välj det här alternativet om du vill stoppa scenariot när det inte finns några resultat.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Archive name]</td> 
   <td> <p> Ange ett namn för det skapade arkivet. Lägg inte till ett tillägg.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Source file]</td> 
   <td> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </td> 
  </tr> 
 </tbody> 
</table>

>[!INFO]
>
>**Exempel:** Titta på inkommande e-post med modulen [!DNL Gmail] >[!UICONTROL Watch emails]. Om ett e-postmeddelande tas emot itereras dess bilagor in i enskilda paket, arkiveras sedan i filen [!DNL ZIP] och sparas i den angivna Dropbox-mappen.
>
>![](assets/example-gmail-350x102.png)

## [!UICONTROL Inflate]

Den här transformatormodulen dekomprimerar binära data med en inflationsalgoritm.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Ange eller mappa de data som du vill expandera med funktionen inflate.</p> </td> 
  </tr> 
 </tbody> 
</table>

## [!UICONTROL Deflate]

Den här transformatormodulen komprimerar binära data med en deflationsalgoritm.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Data] </td> 
   <td> <p>Ange eller mappa de data som du vill komprimera med hjälp av deflate-funktionen.</p> </td> 
  </tr> 
 </tbody> 
</table>
