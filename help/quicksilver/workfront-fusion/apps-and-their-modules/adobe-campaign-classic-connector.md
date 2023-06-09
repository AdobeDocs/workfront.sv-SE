---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe Campaign Classic-moduler
description: Med [!DNL Adobe Campaign Classic] -moduler kan du starta en [!DNL Adobe Workfront Fusion] scenario baserat på händelser i [!DNL Adobe Campaign Classic] konto, skapa, läsa eller uppdatera avtal och andra poster, söka efter poster med villkor som du anger och ladda upp dokument.
author: Becky
feature: Workfront Fusion
exl-id: 84e8fa35-0c3c-46bd-8886-88c6d8d9e1d5
source-git-commit: 482725764ede6b2700985fa67dc2cb9f92d3bb12
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# [!DNL Adobe Campaign Classic] moduler

Med [!DNL Adobe Campaign Classic] -moduler kan du starta en [!DNL Adobe Workfront Fusion] scenario baserat på händelser i [!DNL Adobe Campaign Classic] konto, skapa, läsa eller uppdatera poster, söka efter poster med villkor som du anger och utföra anpassade API-anrop.

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
   <td> <p>[!UICONTROL [!DNL Workfront Fusion] för automatisering och integrering av arbetet] </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

Kontakta [!DNL Workfront] administratör.

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).

## Anslut [!DNL Adobe Campaign Classic] till [!DNL Adobe Workfront Fusion]

1. I alla [!DNL Adobe Campaign Classic] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Ange den bas-URL som du använder för att ansluta till din [!DNL Adobe Campaign Classic] -instans.
1. Ange ditt användarnamn och lösenord.
1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Adobe Campaign Classic] moduler och deras fält

När du konfigurerar [!DNL Adobe Campaign Classic] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Adobe Campaign Classic] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)
* [Sökningar](#searches)

### Utlösare

#### [!UICONTROL Watch records]

Denna schemalagda utlösarmodul startar ett scenario när en post ändras.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Filter]</td> 
   <td>Välj om du vill söka efter nya poster, uppdaterade poster eller båda.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Välj den resurs som du vill bevaka.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output]</td> 
   <td>Markera de fält som du vill inkludera i modulens utdata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>För varje anpassat fält som du vill inkludera i utdata klickar du på <b>[!UICONTROL Add]</b> och ange namnet på det anpassade fältet.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned results]</td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>


### Åtgärder

* [[!UICONTROL Create a record]](#create-a-record)
* [[!UICONTROL Make a custom API call]](#make-a-custom-api-call)
* [[!UICONTROL Delete a record]](#delete-record)
* [[!UICONTROL Perform an action]](#perform-an-action)
* [[!UICONTROL Read a record]](#-read-a-record)
* [[!UICONTROL Subscribe or unsubscribe]](#subscribe-or-unsubscribe)
* [[!UICONTROL Update a record]](#update-record)

#### [!UICONTROL Create a record]

Den här åtgärdsmodulen skapar en ny post i [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Välj typ av [!DNL Adobe Campaign Classic] poster som du vill skapa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Markera de fält som du vill ange värden för när posten skapas och fyll sedan i värdena för dessa fält. Fälten varierar beroende på vilken typ av post du väljer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> För varje anpassat fält som du vill lägga till i den nya posten klickar du på <b>[!UICONTROL Add item]</b> och ange eller mappa fältets namn och värde. </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Make a custom API call]

Den här modulen gör ett anpassat API-anrop till [!DNL Adobe Campaign Classic] API

<table style="table-layout:auto"> 
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Action]</td>
      <td><p>Välj den åtgärd som du vill att API-anropet ska utföra.</p>
      <p>[!UICONTROL Execute query]</p>
      <p>[!UICONTROL Write]</p>
      <p>[!UICONTROL Get entity if more recent]</p>
      <p>[!UICONTROL Select all]</p>
      <p>[!UICONTROL Push event]</p>
    </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>[!DNL Workfront Fusion] lägger till [!UICONTROL x-security] tokenhuvud automatiskt.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL XML Body]</td>
   <td> <p>Lägg till brödtexten för API-anropet i XML, utan sessionselementet. </td>     </tr>
  </tbody>
</table>

#### [!UICONTROL Delete Record]

Den här åtgärdsmodulen tar bort en enstaka post från [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Välj den typ av resurs som du vill ta bort.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange eller mappa ID:t för resursen som du vill ta bort.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Perform an action]

Den här åtgärdsmodulen utför en markerad åtgärd på ett objekt i [!DNL Adobe Campaign Classic] API.

Mer information om specifika åtgärder och fält finns i [[!DNL Adobe Campaign] - API-dokumentation](https://experienceleague.adobe.com/developer/campaign-api/api/p-14.html).

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Action]</td> 
   <td><p>Välj vilken åtgärd som ska utföras på objektet.</p>
   <ul>
   <li><p><b>[!DNL List]</b></p><p> Information om tillgängliga fält finns i <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> i den här artikeln. </p></li>
     <li><p><b>[!UICONTROL Get]</b></p><p> Information om tillgängliga fält finns i <a href="#search" class="MCXref xref" >[!UICONTROL Search]</a> i den här artikeln. </p></li> 
   <li><p><b>[!UICONTROL Create]</b></p><p> Information om tillgängliga fält finns i <a href="#create-a-record" class="MCXref xref" >[!UICONTROL Create a record]</a> i den här artikeln. </p></li>
   <li><p><b>[!UICONTROL Update]</b></p><p> Information om tillgängliga fält finns i <a href="#update-record" class="MCXref xref" >[!UICONTROL Update a record]</a> i den här artikeln. </p></li>
   <li><p><b>[!UICONTROL Delete]</b></p><p> Information om tillgängliga fält finns i <a href="#delete-record" class="MCXref xref" >[!UICONTROL Delete a record]</a> i den här artikeln. </p></li>
   </ul>
   </td>
</tr> 
 </tbody> 
</table>

#### [!UICONTROL Read a record]

Den här åtgärdsmodulen läser en post från [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Välj typ av [!DNL Adobe Campaign Classic] poster som du vill läsa.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Ange på kartan ID:t för den post som du vill läsa.</td> 
  </tr> 
 <tr> 
   <td role="rowheader">[!UICONTROL Fields to include in output] </td> 
   <td>Markera de fält som du vill inkludera i modulens utdata.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields to include in output]</td> 
   <td>För varje anpassat fält som du vill inkludera i utdata klickar du på <b>[!UICONTROL Add]</b> och ange namnet på det anpassade fältet.</td> 
  </tr> 
 </tbody> 
</table>


#### [!UICONTROL Subscribe or unsubscribe]

Den här åtgärdsmodulen prenumererar på eller avbryter en användares prenumeration på en informationstjänst.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe or unsubscribe]</td> 
   <td>Välj om du vill prenumerera eller avbryta prenumerationen på informationstjänsten.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Service name]</td> 
   <td>Välj den tjänst som du vill prenumerera på eller avbryta prenumerationen på.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Recipient email address] </td> 
   <td>Ange eller mappa e-postadressen till den användare som du vill prenumerera på eller avbryta prenumerationen på informationstjänsten.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update record]

Den här åtgärdsmodulen uppdaterar en enda post i [!DNL Adobe Campaign Classic].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Välj typ av [!DNL Adobe Campaign Classic] poster som du vill skapa.</td> 
  </tr> 
    <tr> 
   <td role="rowheader">[!UICONTROL ID] </td> 
   <td>Ange på kartan ID:t för den post som du vill uppdatera.</td> 
  </tr> 
<tr> 
   <td role="rowheader">[!UICONTROL Fields] </td> 
   <td>Markera de fält som du vill uppdatera värden för och fyll sedan i värdena för dessa fält. Fälten varierar beroende på vilken typ av post du väljer.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Custom fields]</td> 
   <td> För varje anpassat fält som du vill uppdatera klickar du på <b>[!UICONTROL Add item]</b> och ange eller mappa fältets namn och värde. </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

#### [!UICONTROL Search]

Sökmodulen returnerar poster baserat på angivna villkor.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td>
   <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe Campaign Classic], se <a href="#connect-adobe-campaign-classic-to-adobe-workfront-fusion" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe Campaign Classic]</a> i den här artikeln.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Resource]</td> 
   <td>Välj typ av [!DNL Adobe Campaign Classic] poster som du vill skapa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>
