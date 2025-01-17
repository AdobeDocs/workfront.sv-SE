---
product-previous: workfront-fusion
product-area: workfront-integrations
navigation-topic: mapping
title: Mappa en array i [!DNL Adobe] Workfront Fusion
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion
exl-id: 725e0c24-cb4b-46c4-9c00-4f9cc334fbc7
source-git-commit: 2d6af8b4988bd9aab7381daa79dec79e41408c45
workflow-type: tm+mt
source-wordcount: '907'
ht-degree: 0%

---

# Mappa en matris i [!DNL Adobe Workfront Fusion]

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Mappa en array eller ett arrayelement](https://experienceleague.adobe.com/docs/workfront-fusion/using/create-scenarios/map-data/map-an-array.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

En array är en speciell typ av objekt som kan innehålla följande:

* Ett eller flera textvärden (enkel array)
* En eller flera samlingar av samma typ (komplex array)

>[!INFO]
>
>**Exempel:** Modulen [!UICONTROL Watch emails] returnerar en array med bilagor för varje e-postmeddelande. Alla bilagor representerar en samling som kan innehålla namn, innehåll, storlek och så vidare.

Mer information finns i [Objektdatatyper i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/item-data-types.md).

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
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

Mer information om [!DNL Adobe Workfront Fusion] licenser finns i [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).



## Mappa en hel array

1. I modulerna som du mappar arrayen till klickar du på fältet där du vill mappa arrayen. Det här är fältet som arrayen mappas till.

1. Mappa objektet i rutan som visas.

   På panelen kan du mappa fält på samma sätt som andra typer av objekt. Om du inte vill fylla i varje objekt separat, men vill mappa en annan array till målfältet, använder du knappen [!UICONTROL Map]. I det här fallet måste du se till att båda arrayerna (källarrayen och målarrayen) har samma struktur.

   Du kan lägga till valfritt antal objekt i en array.

Du kan dela upp en array i enskilda paket med hjälp av en iterator. Mer information finns i modulen [[!UICONTROL Iterator] i  [!DNL Adobe Workfront Fusion]](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

## Mappa objekt till en ny array

I vissa fält i Workfront Fusion kan du mappa element till en array. Du kan t.ex. skapa en array med checklisteobjekt i modulen Workfront Boards > Lägg till checklisteobjekt. När modulen körs läggs alla objekt i checklistan till på kortet.

Alla modulfält som visar&quot;Lägg till objekt&quot; skapar en array.

![Lägg till objekt](assets/add-item.png)

Så här lägger du till element i arrayen:

1. Klicka på **Lägg till objekt**
1. Ange information om objektet på panelen som öppnas.
1. Klicka på **Lägg till**.
1. (Valfritt) Upprepa steg 1-3 för varje element som du vill lägga till i -arrayen.

## Mappa arrayelement


### Mappa arrayelement efter nummer

Arrayelement visas som ett tal inom hakparenteser efter arraynamnet. Du kan mappa ett enskilt element i en array till ett fält genom att använda detta indexnummer.

![](assets/map-array-1st-element.png)

>[!NOTE]
>
>Matrisindexeringen i Workfront Fusion börjar från 1.

Så här mappar du ett arrayelement:

1. Klicka i det fält där du vill mappa elementet.

   Mappningspanelen öppnas.

1. Leta reda på arrayen som innehåller elementet som du vill mappa.
1. Klicka på pilen bredvid arrayen.
1. Klicka på elementet som du vill mappa.

   Elementet mappas med indexvärdet 1. Detta mappar det första elementet i arrayen.

1. Om du vill mappa ett annat element i arrayen klickar du på [1] och anger indexnumret för det arrayelement som du vill mappa.

   ![](assets/access-another-element.png)

### Mappa ett arrayelement med en given nyckel

Vissa arrayer innehåller samlingar med nyckelvärdesobjekt som metadata, attribut och så vidare. Om du vill använda något av dessa värden kan du slå upp ett element med dess angivna nyckelvärde och hämta motsvarande värde från värdeobjektet. Vi rekommenderar att du använder en formel som innehåller en kombination av funktionerna `map()` och `get()`.



>[!BEGINSHADEBOX]

I följande exempel visas utdata för appen [!DNL Jira].

![](assets/output-of-jira-app-350x100.png)

I det här exemplet hämtas ett filnamn från en array med bilagor, för den specifika bilagan med ID 10108.

I det här exemplet genereras följande utdata:

![](assets/output-from-jira-350x261.png)

Formeln kan förklaras på följande sätt:

* `map`

   1. Den första parametern i funktionen `map()` är hela arrayobjektet.
   1. Den andra parametern är värdobjektets raw-namn. Håll markören över objektet på panelen [!UICONTROL mapping] om du vill få Raw-namnet:

      ![](assets/obtain-raw-name-350x124.png)

      >[!NOTE]
      >
      >Alla parametrar är versalkänsliga. Även om objektets etikett i det här exemplet skiljer sig från dess Raw-namn endast med versaler, måste du använda raw-namnet.

   1. Den tredje parametern är nyckelobjektets raw-namn:

      ![](assets/3rd-parameter-350x166.png)

   1. Den fjärde parametern är det angivna nyckelvärdet.

  Eftersom funktionen `map()` returnerar en array (eftersom det kan finnas fler element med det angivna nyckelvärdet), måste du använda funktionen `get()` för att få det första elementet:

* `get`

   1. Den första parametern i funktionen `get()` är resultatet av funktionen `map()`.

   1. Den andra parametern är elementets index. I det här exemplet är indexvärdet `1`.

I det här exemplet genereras följande utdata:

![](assets/output-from-jira-350x261.png)

>[!ENDSHADEBOX]

Mer information om funktionen `map()` finns i [Array-funktioner](/help/quicksilver/workfront-fusion/functions/array-functions.md).

Mer information om funktionen `get()` finns i [Allmänna funktioner](/help/quicksilver/workfront-fusion/functions/general-functions.md).

## Konvertera arrayelement till en serie paket

Matriser kan konverteras till en serie paket med modulen [!UICONTROL Iterator]. Mer information finns i [[!UICONTROL Iterator] modul](/help/quicksilver/workfront-fusion/modules/iterator-module.md).

![](assets/series-of-bundles.png)

