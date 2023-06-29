---
title: Bredda moduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!UICONTROL Widen], samt ansluta till flera tredjepartsprogram och -tjänster.
author: Becky
draft: Probably
feature: Workfront Fusion
exl-id: d46935bc-4f6c-4502-bd2f-3927f33241e1
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1346'
ht-degree: 1%

---

# [!DNL Widen] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!UICONTROL Widen], samt ansluta till flera tredjepartsprogram och -tjänster.

Om du behöver instruktioner om hur du skapar ett scenario kan du läsa [Skapa ett scenario i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/scenarios/create-a-scenario.md).

Mer information om moduler finns i [Moduler i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/modules/modules.md).

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
   <p>Gammalt licenskrav: [!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>
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

## Förutsättningar

Används [!UICONTROL Widen] moduler, du måste ha en [!UICONTROL Widen] konto.

## Anslut [!DNL Widen] till [!DNL Workfront Fusion] {#connect-widen-to-workfront-fusion}

Du kan skapa en anslutning till [!DNL Widen] direkt inifrån [!DNL Widen] -modul.

1. I alla [!DNL Widen] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Välj [!DNL Widen] domän som du vill ansluta till.
1. Ange din token [!DNL Widen] konto. Instruktioner om hur du hittar den här variabeln finns i [[!DNL Widen] Vanliga frågor om API](https://community.widen.com/collective/s/article/API-FAQs).
1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Widen] moduler och deras fält

När du konfigurerar [!DNL Widen] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Widen] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösarmoduler](#trigger-modules)
* [Åtgärdsmoduler](#action-modules)
* [Sökmoduler](#search-modules)

### Utlösarmoduler

#### [!UICONTROL Watch assets]

Den här utlösarmodulen startar ett scenario när en resurs skapas eller uppdateras.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Event type]</td> 
   <td> <p>Välj om du vill titta på nya resurser eller uppdaterade resurser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Välj de egenskaper som du vill inkludera i modulutdata utöver resursfälten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de fält som du vill inkludera i modulutdata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet resurser som du vill att modulen ska arbeta med under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Åtgärdsmoduler

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Read asset info]](#read-asset-info)
* [[!UICONTROL Add assets to collections]](#add-assets-to-collections)
* [[!UICONTROL Remove assets from collection]](#remove-assets-from-collection)
* [[!UICONTROL Update asset metadata]](#update-asset-metadata)
* [[!UICONTROL Download File]](#download-file)
* [[!UICONTROL Upload] en fil](#upload-a-file)

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Widen] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Widen] moduler.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Välj om du vill använda den senaste versionen av [!DNL Widen] API, eller version 1.0</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ange eller mappa URL:en för ditt API-anrop.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>[!UICONTROL Workfront Fusion] lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"name":"something-urgent"}</code></p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Read asset info]

Den här åtgärdsmodulen hämtar en enskild resurs med dess unika ID.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Ange eller mappa ID:t för resursen som du vill läsa information för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Välj de egenskaper som du vill inkludera i modulutdata utöver resursfälten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de fält som du vill inkludera i modulutdata.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Add assets to collections]

Den här åtgärdsmodulen lägger till en eller flera resurser i samlingar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>För varje samling som du vill lägga till resurserna i:</p> 
    <ol> 
     <li value="1"> <p> Klicka på <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Ange eller mappa [!UICONTROL Collection ID].</p> </li> 
     <li value="3"> <p>Klicka på <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Assets ID]</td> 
   <td> <p>För varje resurs som du vill lägga till i en samling:</p> 
    <ol> 
     <li value="1"> <p> Klicka på <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Ange eller mappa resurs-ID:t.</p> </li> 
     <li value="3"> <p>Klicka på <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet resurser som du vill att modulen ska arbeta med under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove assets from collection]

Den här åtgärdsmodulen tar bort en eller flera resurser från samlingar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collections ID]</td> 
   <td> <p>För varje samling som du vill ta bort resurserna från:</p> 
    <ol> 
     <li value="1"> <p> Klicka på <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Ange eller mappa samlings-ID.</p> </li> 
     <li value="3"> <p>Klicka på <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Resurs-ID</td> 
   <td> <p>För varje resurs som du vill ta bort från en samling:</p> 
    <ol> 
     <li value="1"> <p> Klicka på <strong>[!UICONTROL Add]</strong>.</p> </li> 
     <li value="2"> <p>Ange eller mappa resurs-ID:t.</p> </li> 
     <li value="3"> <p>Klicka på <strong>[!UICONTROL Add item]</strong>.</p> </li> 
    </ol> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet resurser som du vill att modulen ska arbeta med under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update asset metadata]

Den här åtgärdsmodulen uppdaterar metadatafälten för en resurs.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Ange eller mappa ID:t för resursen där du vill uppdatera metadata.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata type]</td> 
   <td> <p>Välj metadatatyp för de metadata som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Markera de metadatafält som du vill uppdatera. Ange fältets nya värde för varje fält.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antalet resurser som du vill att modulen ska arbeta med under varje körningscykel för scenario.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download File]

Den här åtgärdsmodulen hämtar en resurs från din [!DNL Widen] konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Asset ID]</td> 
   <td> <p>Ange eller mappa ID:t för resursen som du vill hämta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload a file]

Den här åtgärdsmodulen överför en fil till din [!DNL Widen] konto.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Profile]</td> 
   <td> <p>Välj den överföringsprofil som du vill att modulen ska använda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Upload Method]</td> 
   <td> <p>Välj hur du vill överföra filen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL From File]</strong> </p> <p>Markera eller mappa källfilen från en tidigare modul.</p> </li> 
     <li> <p><strong>[!UICONTROL By URL]</strong> </p> <p>Ange eller mappa URL:en för filen som du vill överföra.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File name]</td> 
   <td>Ange eller mappa ett namn för den överförda filen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata Type]</td> 
   <td>Välj metadatatyp för filen som du vill överföra.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Metadata]</td> 
   <td>Markera de metadatafält som du vill inkludera i filöverföringen. För varje fält anger du [!UICONTROL value] för fältet.</td> 
  </tr> 
 </tbody> 
</table>

### Sökmoduler

* [[!UICONTROL Read collection assets]](#read-collection-assets)
* [[!UICONTROL Search assets]](#search-assets)

#### [!UICONTROL Read collection assets]

Den här åtgärdsmodulen hämtar en lista med resurser i en samling.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Collection ID]</td> 
   <td> <p>Ange eller mappa ID:t för samlingen som innehåller de resurser som du vill läsa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Start]</td> 
   <td>Ange eller mappa numret för det första objektet som du vill visa. Detta är ett sätt att numrera posterna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Max]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>Välj den egenskap som du vill sortera resurserna efter. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Välj om du vill sortera resurser i stigande eller fallande ordning.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de fält som du vill inkludera i modulutdata.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Search assets]

Den här sökmodulen hämtar en lista med resurser som matchar de specifika sökvillkoren.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
  <td> <p>Instruktioner om hur du ansluter [!DNL Widen] konto till [!DNL Workfront Fusion], se <a href="#connect-widen-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Widen] till [!DNL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search query]</td> 
   <td> <p>Ange villkoren som du vill använda för att söka efter resurser.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Sort By]</td> 
   <td> <p>Välj hur du vill sortera resurserna. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Order]</td> 
   <td>Välj om du vill sortera resurser i stigande eller fallande ordning.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Include deleted]</td> 
   <td>Aktivera det här alternativet om du vill ta med borttagna resurser i sökningen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Include archived]</p> </td> 
   <td> <p>Aktivera det här alternativet om du vill inkludera arkiverade resurser i sökningen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Search document text]</td> 
   <td>Aktivera det här alternativet om du vill inkludera dokumenttext i sökningen, eller false om du bara vill inkludera resurser där titeln matchar sökvillkoren.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td> <p>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Offset]</td> 
   <td>Ange eller mappa numret för det första objektet som du vill hämta information för. Detta är ett sätt att numrera posterna.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Scroll]</td> 
   <td>Aktivera det här alternativet om du vill tillåta rullning.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Expand]</td> 
   <td> <p>Välj de egenskaper som du vill inkludera i modulutdata utöver resursfälten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de fält som du vill inkludera i modulutdata.</td> 
  </tr> 
 </tbody> 
</table>
