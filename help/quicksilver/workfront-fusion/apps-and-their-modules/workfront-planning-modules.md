---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe Workfront Planning-moduler
description: Med [!DNL Adobe Workfront Planning] -moduler kan du starta en [!DNL Adobe Workfront Fusion] scenario baserat på händelser i [!DNL Adobe] Workfront Planning-konto, skapa, läsa eller uppdatera avtal och andra poster, söka efter poster med villkor som du anger och ladda upp dokument.
author: Becky
feature: Workfront Fusion
hide: true
hidefromtoc: true
exl-id: 892fdaf3-935e-4e66-a01c-9e9b6e0daf3e
source-git-commit: 593612fea52d917904605cf3d97403347c9c9ac0
workflow-type: tm+mt
source-wordcount: '920'
ht-degree: 0%

---

# [!DNL Adobe Workfront Planning] moduler

Med [!DNL Adobe Workfront Planning] -moduler kan du utlösa ett scenario när händelser inträffar i Workfront Planning. Du kan också skapa, läsa, uppdatera och ta bort poster eller utföra ett anpassat API-anrop till [!DNL Adobe Workfront Planning] konto.

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
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Kontakta din [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Skapa en anslutning till [!DNL Adobe Workfront Planning]

Du kan skapa en anslutning till [!DNL Workfront Planning] direkt inifrån ett [!DNL Workfront Fusion] -modul.

1. I alla [!DNL Workfront Planning] programmodul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] box.
1. Ange ett namn för anslutningen.
1. Välj om du vill ansluta till en produktionsmiljö eller en icke-produktionsmiljö.
1. Ange om du ansluter till ett tjänstkonto eller ett personligt konto.
1. Klicka **[!UICONTROL SAML log in]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Adobe Workfront Planning] moduler och deras fält

### Se händelser

Den här utlösarmodulen startar ett scenario när en post, posttyp eller arbetsyta skapas, uppdateras eller tas bort i Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Webhook]</td>
      <td>Välj den webkrok som du vill använda eller klicka på Lägg till för att skapa en ny.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Object type]</td>
      <td>Välj om du vill bevaka poster, posttyper eller arbetsytor.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Objects to watch]</td>
      <td>Välj om du vill hålla utkik efter nya. uppdaterade, nya och uppdaterade eller borttagna poster.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Exclude updates made by this connection]</p>
      </td>
      <td>Aktivera det här alternativet om du vill förhindra att scenariot aktiveras när en ändring görs av anslutningen som används av modulen. Detta förhindrar att en annan instans av scenariot utlöses om det här scenariot utför en utlösande åtgärd.</td> 
      </tr>
  </tbody>
</table>

### Ta bort en posttyp

Den här åtgärdsmodulen tar bort en enskild posttyp i Workfront Planning med dess ID.

>[!WARNING]
>
>Om du tar bort en posttyp i Workfront Planning tas även alla poster i posttyptabellen bort.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Ange eller mappa ID:t för fältet som du vill ta bort.</td> 
      </tr>
  </tbody>
</table>

### Göra ett anpassat API-anrop

Den här modulen gör ett anpassat API-anrop till [!DNL Adobe Workfront Planning] API.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Ange en sökväg som är relativ till https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API version]</p>
      </td>
      <td>
        <p>Välj den API-version som du vill använda. Om du inte väljer någon version används den senaste versionen som standard.</p>
      </td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL API Path override]</p>
      </td>
      <td>
        <p>Ange en sökväg som är relativ till https://&lt;WORKFRONT_DOMAIN&gt;/attask/api/&lt;API_VERSION&gt;/</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] lägger till auktoriseringshuvuden automatiskt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>För varje nyckel/värde-par som du vill lägga till i frågesträngen klickar du på <b>Lägg till objekt</b> och ange nyckeln och värdet.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

<!--

### Delete a field

This action module deletes a single field in Workfront Planning by its ID.

>[!WARNING]
>
>Deleting a field in Workfront Planning deletes it and any data in it from every object of that record type in Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the record type you want to delete.</td> 
      </tr>
  </tbody>
</table>

### Get a field 


This action module retrieves a single field in Workfront Planning by its ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Field ID]</p>
      </td>
      <td>Enter or map the ID of the field you want to delete.</td> 
      </tr>
  </tbody>
</table>

-->

### Skapa en post

Den här åtgärden skapar en enda post i Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record type ID]</p>
      </td>
      <td>Ange eller mappa den typ av post som du vill skapa. Tillgängliga posttyper baseras på ditt Workfront Planning-konto.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Andra fält</p>
      </td>
      <td>Dessa fält baseras på den posttyp som du har valt.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Ta bort en post

Den här åtgärdsmodulen tar bort den angivna posten i Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Ange eller mappa ID:t för den post som du vill ta bort.</td> 
      </tr>
  </tbody>
</table>

<!--

### Get all records

This action module retrieves all records from an [!DNL Adobe Workfront Planning] account.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>For instructions on creating a connection to [!DNL Adobe Workfront Planning], see <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Create a connection to [!DNL Adobe Workfront Planning]</a> in this article.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Enter or map the maximum number of records you want the module to return during each scenario execution cycle.</td> 
      </tr>
  </tbody>
</table>

-->

### Hämta en post

Den här åtgärdsmodulen hämtar en post från [!DNL Adobe Workfront Planning], som anges av dess ID.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record ID]</td>
      <td>Ange eller mappa ID:t för den post som du vill hämta.</td>
    </tr>
  </tbody>
</table>

### Hämta poster efter posttyp

Den här åtgärdsmodulen hämtar alla poster av den angivna typen.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Workspace]</td>
      <td>Markera eller mappa arbetsytan som innehåller de poster som du vill hämta.</td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Record type]</td>
      <td>Välj den typ av post som du vill hämta.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Maximum number of returned records]</p>
      </td>
      <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td> 
  </tbody>
</table>

### Hämta posttyper

Den här åtgärdsmodulen hämtar en lista med posttyper i en [!DNL Adobe Workfront Planning] konto.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
  </tbody>
</table>

### Uppdatera post

Den här åtgärden uppdaterar en enda post i Workfront Planning.

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
      <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Workfront Planning], se <a href="#create-a-connection-to-adobe-workfront planning" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Workfront Planning]</a> i den här artikeln.</td>
    </tr>
     <tr>
      <td role="rowheader">
        <p>[!UICONTROL Record ID]</p>
      </td>
      <td>Ange eller mappa den typ av post som du vill uppdatera. Tillgängliga posttyper baseras på ditt Workfront Planning-konto.</td> 
      </tr>
     <tr>
      <td role="rowheader">
        <p>Andra fält</p>
      </td>
      <td>Dessa fält baseras på den posttyp som du har valt.</td> 
      </tr>
     <tr>
  </tbody>
</table>

### Sök poster

Den här åtgärdsmodulen hämtar en lista med poster baserat på villkor som du anger.

>[!NOTE]
>
>Den här modulen håller på att byggas.
