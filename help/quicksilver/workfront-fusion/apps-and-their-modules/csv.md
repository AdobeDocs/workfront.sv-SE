---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations;documents
navigation-topic: apps-and-their-modules
title: CSV
description: Med Adobe Workfront Fusion CSV-modulerna kan du skapa CSV-filer och tolka CSV-text från ett mottaget textvärde eller en fil.
author: Becky
feature: Workfront Fusion
exl-id: 4e37482a-e84e-4ab2-a48f-7e7bfbecee56
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '865'
ht-degree: 0%

---

# CSV

The [!DNL Adobe Workfront Fusion] [!UICONTROL CSV] Med -moduler kan du skapa CSV-filer och tolka CSV-text från ett mottaget textvärde eller en fil.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td>
  <td> <p>[!UICONTROL Pro] eller högre</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td>
   <td> <p>[!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens**</td> 
   <td>
   <p>Aktuellt licenskrav: Nej [!DNL Workfront Fusion] krav på licens.</p>
   <p>eller</p>
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] for Work Automation and Integration],  [!UICONTROL [!DNL Workfront Fusion] for Work Automation]</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>
   <p>Aktuellt produktbehov: Om du har [!UICONTROL Select] eller [!UICONTROL Prime] [!DNL Adobe Workfront] Planera, din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln. [!DNL Workfront Fusion] ingår i [!UICONTROL Ultimate] [!DNL Workfront] plan.</p>
   <p>eller</p>
   <p>Krav för äldre produkt: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## [!UICONTROL Create CSV]

The [!UICONTROL Create CSV] Med Aggregator kan du skapa en csv-text från mottagna textvärden.

Mer information om aggregerare finns i [Aggregator-modulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
    <tr>
        <td>[!UICONTROL Source Module]</td>
        <td>Markera modulen som du använder för att sammanställa de fält du behöver.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Aggregated Fields]</td>
        <td>Markera de fält som du vill samla i listan med tillgängliga fält.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Include headers in the first row]</td>
        <td>Välj det här alternativet om du vill ta med rubrikerna i resultatet.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Group by]</td>
        <td>Ange filtret för att gruppera resultaten. Ange till exempel ett datum.</td>
    </tr>
    <tr>
        <td>[!UICONTROL Stop processing after an empty aggregation]</td>
        <td>Välj det här alternativet om du vill stoppa scenariot när det inte finns några resultat.</td>
    </tr>
</table>

## [!UICONTROL Create CSV (advanced)]

The [!UICONTROL Create CSV (advanced)] Med Aggregator kan du skapa en CSV-text från mottagna textvärden. Den använder en datastruktur som definierar CSV-kolumnerna i den resulterande CSV-filen. När kolumnerna har definierats visas de som fält i CSV-modulen och kan mappas till en senare modul i scenariot.

Mer information om aggregerare finns i [Aggregator-modulen i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/aggregator-module.md).

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source Module]</td> 
   <td>Välj den programmodul som du använder för att samla in de fält som du behöver.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Data Structure]</td> 
   <td> <p>Välj datastrukturen för att samla fälten på det sätt du vill. När du har definierat datastrukturen kan du mappa objekten till motsvarande fält.</p> <p>Mer information finns i <a href="../../workfront-fusion/modules/data-structures.md" class="MCXref xref">Datastrukturer i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include headers in the first row] </td> 
   <td>Välj det här alternativet om du vill ta med rubrikerna i resultatet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Group by] </td> 
   <td>Ange filtret för att gruppera resultaten. Ange till exempel ett datum. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Stop processing after an empty aggregation] </td> 
   <td>Välj det här alternativet om du vill stoppa scenariot när det inte finns några resultat. </td> 
  </tr> 
 </tbody> 
</table>


<p>Låt oss anta att du vill exportera dina Google-kontakter till en CSV-fil med två kolumner, "Fullständigt namn" och "E-post". Utdatapaketet från [!UICONTROL Google Contacts] &gt;[!UICONTROL Get contacts from a group] modulen har följande struktur. E-postadresserna lagras i <code>[!UICONTROL Emails[]]</code> objekt, som är en array med samlingar, där varje samling innehåller två objekt: <code>Label</code> och <code>Email</code>.</p>
<p> <img src="assets/transforming-350x546.png" style="width: 350;height: 546;"> </p>
<p>Om du använder det enkla [!DNL Create CSV] visas en lista med kryssrutor som motsvarar ett pakets objekt på den översta nivån. Om du försöker kryssa <code>Full name</code> och <code>Emails</code> objekt, [!UICONTROL Create CSV] -modulen skapar följande utdata, vilket förmodligen inte är vad du vill ha:</p>
<p>"emails","fullName"</p>
<p>"[object Object]","Shon Winer"</p>
<p>"[object Object]","Lizeth Fulmore"</p>
<p>"[object Object]","Hilario Gullatt"</p>
<p>"[object Object]","Abby Eisenbarth"</p>
<p>Sedan objektet <code>Full Name</code> är av enkel text. Den exporteras bara fint. Men objektet <code>Emails</code>, som är en komplex typ av Array med samlingar, exporteras som [object Object], vilket är hur samlingar och arrayer omformas till text som standard. Mer information finns i <a href="../../workfront-fusion/mapping/item-data-types.md" class="MCXref xref">Objektdatatyper i Adobe Workfront Fusion</a>.</p>
<p>Så här exporterar du innehåll i <code>Email </code>objekt i den första samlingen i <code>Emails[]</code> i stället måste du använda [!UICONTROL Create CSV (advanced)] -modul. Med modulen kan du definiera enskilda kolumner i CSV-filen och mappa objekt till dem, inklusive de kapslade.</p>
<ol>
<li value="1">Infoga modulen [!UICONTROL Create CSV (advanced)] i ett scenario och öppna konfigurationen.</li>
<li value="2">Klicka på <strong>[!UICONTROL Add]</strong> knappen bredvid [!UICONTROL Data structure] för att skapa en ny datastruktur.</li>
<li value="3"> <p>Skriv ett namn för datastrukturen och klicka på <strong>[!UICONTROL Add item]</strong> om du vill lägga till de enskilda kolumnerna. Om du vill exportera två kolumner: "Fullständigt namn" och "E-post" skulle den resulterande datastrukturen se ut så här:</p> <p> <img src="assets/google-contacts-350x524.png" style="width: 350;height: 524;"> </p> </li>
<li value="4"> <p>När du har definierat datastrukturen ska fält som motsvarar varje enskild kolumn visas i konfigurationen för [!UICONTROL Create CSV (advanced)] så att du kan mappa objekten. Ta det första objektet från <code>[!UICONTROL Emails[]]</code> array och mappa dess objekt <code>Email </code>till fältet/kolumnen E-post:</p> <p> <img src="assets/create-csv-advanced-350x308.png" style="width: 350;height: 308;"> </p> </li>
<li value="5"> <p>Kör scenariot. Sedan objektet <code>Emails[1]: Email</code> mappas till kolumnen"E-post" är av enkel typ Text, den exporteras korrekt nu:</p> <p>"Fullständigt namn","E-post"</p> <p>"Shon Winer","Shon@Winer.com"</p> <p>"Lizeth Fulmore","Lizeth@Fulmore.com"</p> <p>"Hilario Gullatt","Hilario@Gullatt.com"</p> <p>"Abby Eisenbarth","Abby@Eisenbarth.com"</p> </li>
</ol>
</div>

## [!UICONTROL Parse CSV]

The [!UICONTROL Parse CSV] kan du tolka CSV-text från ett mottaget textvärde eller en fil.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Number of columns]</td> 
   <td>Ange antalet kolumner i CSV-filen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV contains headers]</td> 
   <td> <p>Välj det här alternativet om den första raden i CSV-texten innehåller rubriker.</p> <p>Obs! Modulen använder inte dessa rubriker för att etikettera kolumnerna i utdata. I stället ser det här fältet till att sidhuvudena inte inkluderas i utdata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL delimiterType]</td> 
   <td> <p>Välj avgränsare för CSV-filen. Avgränsaren är det texttecken som anger gränsen mellan separata värden eller fält.</p> 
    <ul> 
     <li>[!UICONTROL Comma]</li> 
     <li>[!UICONTROL Tab]</li> 
     <li> <p>[!UICONTROL Other]</p> <p>Om du väljer [!UICONTROL Other]anger du det avgränsningstecken som CSV-filen använder för att avgränsa värden. Du måste ange exakt ett tecken.<br></p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Preserve quotes inside unquoted field]</td> 
   <td>Aktivera det här alternativet om du vill bevara citattecken.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL CSV]</td> 
   <td>Ange eller mappa den CSV-fil som du vill analysera.<p>Obs! <p>Om dina data kommer i binär form (vanligtvis från en fil) måste du använda funktionen "toString()" för att konvertera binära data till [!UICONTROL String]:</p><p><img src="assets/parse-csv-350x123.png" style="width: 350;height: 123;"></p></p></td> 
  </tr> 
 </tbody> 
</table>
