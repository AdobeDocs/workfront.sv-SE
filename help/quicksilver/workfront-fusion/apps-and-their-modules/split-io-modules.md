---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Dela.io-moduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Split.io], samt ansluta till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 4576a2e4-b495-430e-a9de-4e1ec7379ab8
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1490'
ht-degree: 0%

---

# [!DNL Split.io] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Split.io], samt ansluta till flera tredjepartsprogram och -tjänster.

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

Används [!DNL Split.io] moduler, du måste ha en [!DNL Split.io] konto.

## Anslut [!DNL Split.io] till [!DNL Workfront Fusion] {#connect-split-io-to-workfront-fusion}

Du kan skapa en anslutning till [!DNL Split.io] direkt inifrån [!DNL Split.io] -modul.

1. I alla [!DNL Split.io] modul, klicka på **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. Ange ett namn för anslutningen.
1. Ange [!DNL Split.io] API-nyckel.

   Mer information om [!DNL Split.io] API-nycklar, se [API-nycklar](https://help.split.io/hc/en-us/articles/360019916211-API-keys) i [!DNL Split.io] dokumentation.

1. Klicka **[!UICONTROL Continue]** för att skapa anslutningen och gå tillbaka till modulen.

## [!DNL Split.io] moduler och deras fält

När du konfigurerar [!DNL split.io] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL split.io] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Åtgärder](#actions)
* [Sökningar](#searches)

### Åtgärder

* [[!UICONTROL Custom API Call]](#custom-api-call)
* [[!UICONTROL Get Split]](#get-split)
* [[!UICONTROL Get Split Definition in Environment]](#get-split-definition-in-environment)
* [[!UICONTROL Create Split]](#create-split)
* [[!UICONTROL Delete Split]](#delete-split)
* [[!UICONTROL Create Split Definition in Environment]](#create-split-definition-in-environment)
* [[!UICONTROL Remove Split Definition from Environment]](#remove-split-definition-from-environment)
* [[!UICONTROL Partial Update Split Definition in Environment]](#partial-update-split-definition-in-environment)
* [[!UICONTROL Associate Tags]](#associate-tags)

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL split.io] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL split.io] moduler.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL URL]</td> 
   <td>Ange en sökväg som är relativ till <code>https://api.split.io/internal/api/v2/</code>.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> <p>Workfront Fusion lägger till auktoriseringsrubrikerna åt dig.</p> </td> 
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
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antal poster som du vill att modulen ska arbeta med under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Split]

Den här åtgärdsmodulen hämtar delningen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan som innehåller den delning som du vill hämta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa namnet på den delning som du vill hämta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Split Definition in Environment]

Den här åtgärdsmodulen hämtar en specifik delad definition från den angivna miljön.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan som innehåller den delningsdefinition som du vill hämta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Markera eller mappa miljön som innehåller den delningsdefinition som du vill hämta.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa namnet på den delning som du vill hämta delningsdefinitionen för.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Split]

Den här åtgärdsmodulen skapar en ny delning i organisationen utifrån en trafiktyp.

>[!NOTE]
>
>API:t konfigurerar inte delningen i någon miljö.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan där du vill dela.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Traffic Type ID or Name]</td> 
   <td>Markera eller mappa den trafiktyp som du vill använda för att skapa delningen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa ett namn för den delning som du vill skapa.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Description]</td> 
   <td>Ange eller mappa en [!UICONTROL split] beskrivning av delningen som du vill skapa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Delete Split]

Den här åtgärdsmodulen tar bort en delning från din organisation. Den delade definitionen avkonfigureras automatiskt från alla miljöer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan där du vill ta bort delningen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa namnet på den delning som du vill ta bort.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create Split Definition in Environment]

Den här åtgärdsmodulen konfigurerar en delad definition för en viss miljö.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan där du vill skapa en delad definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Markera eller mappa miljön där du vill skapa en delad definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa namnet på den delning som du vill skapa en definition för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Ange eller mappa eventuella kommentarer som du vill lägga till i delningsdefinitionen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Rules]</td> 
   <td> <p>För varje målregel som du vill lägga till i definitionen klickar du på <b>[!UICONTROL Add item]</b>och sedan ange eller mappa regeln.</p> <p>Mer information om regler för målinriktning finns i <a href="https://docs.split.io/reference#create-split-definition-in-environment">Skapa en delad definition i en miljö</a> i [!DNL Split.io] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default rule]</td> 
   <td> <p>Ange eller mappa regeln som du vill att delningen ska använda för trafiken som inte uppfyller specifikationerna för de andra reglerna.</p> <p>Mer information om regler för målinriktning finns i <a href="https://docs.split.io/reference#create-split-definition-in-environment">Skapa en delad definition i en miljö</a> i [!DNL Split.io] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Default treatment]</td> 
   <td> <p>Ange eller mappa den behandling som du vill att delningen ska använda om delningen avbryts eller om kunden inte inkluderas i trafikallokeringen.</p> <p>Mer information om behandlingar finns i <a href="https://docs.split.io/reference#create-split-definition-in-environment">Skapa en delad definition i en miljö</a> i [!DNL Split.io] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Treatments]</td> 
   <td> <p>För varje behandling som du vill lägga till i definitionen klickar du på <b>[!UICONTROL Add item]</b>och sedan ange eller mappa behandlingen.</p> <p>Mer information om behandlingar finns i <a href="https://docs.split.io/reference#create-split-definition-in-environment">Skapa en delad definition i en miljö</a> i [!DNL Split.io] dokumentation.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Remove Split Definition from Environment]

Den här åtgärdsmodulen avkonfigurerar en delad definition för en viss miljö.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan där du vill ta bort en delad definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Markera eller mappa miljön där du vill ta bort en delad definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa namnet på den delning som du vill ta bort en definition för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Ange eller mappa eventuella kommentarer som du vill lägga till i delningsdefinitionen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Partial Update Split Definition in Environment]

Den här åtgärdsmodulen uppdaterar en delad definition för en viss miljö.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan där du vill uppdatera en delad definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Markera eller mappa miljön där du vill uppdatera en delad definition.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Split Name]</td> 
   <td> <p>Ange eller mappa namnet på den delning som du vill uppdatera en definition för.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Update content]</td> 
   <td> <p>För varje attribut i delningen som du vill uppdatera klickar du på <b>[!UICONTROL Add item]</b> och ange eller mappa ändringarna.</p> <p>Mer information finns i <a href="https://docs.split.io/reference#partial-update-split-definition-in-environment">Delvis uppdatering, delad definition i miljön</a> i [!DNL Split.io] dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comments]</td> 
   <td>Ange eller mappa eventuella kommentarer som du vill lägga till i delningsdefinitionen.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Associate Tags]

Den här åtgärdsmodulen lägger till taggar i det angivna objektet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan där du vill lägga till en tagg.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Name]</td> 
   <td>Ange eller mappa namnet på objektet som du vill lägga till taggar i,</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Object Type]</td> 
   <td> <p>Ange eller mappa den typ av objekt som du vill lägga till taggar i.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Tags]</td> 
   <td> <p>För varje tagg som du vill lägga till klickar du på <b>[!UICONTROL Add item]</b> och ange eller mappa taggen.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

* [[!UICONTROL Get Workspaces]](#get-workspaces)
* [[!UICONTROL Get Environments]](#get-environments)
* [[!UICONTROL Get Splits]](#get-splits)
* [[!UICONTROL List Split Definitions in an Environment]](#list-split-definitions-in-an-environment)
* [[!UICONTROL Get Traffic Types]](#get-traffic-types)

#### [!UICONTROL Get Workspaces]

Den här sökmodulen hämtar arbetsytorna för en organisation.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antalet arbetsytor som du vill att modulen ska hämta under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Environments]

Den här sökmodulen hämtar en lista över miljöer.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan som innehåller de miljöer du vill visa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Splits]

Den här sökmodulen hämtar en lista med delningar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan som innehåller de uppdelningar som du vill visa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det högsta antal delningar som du vill att modulen ska hämta under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL List Split Definitions in an Environment]

Den här sökmodulen hämtar en lista med delade definitioner i en viss miljö.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan som innehåller de delade definitioner som du vill visa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Environment Name or ID]</td> 
   <td>Markera eller mappa miljön som innehåller de delade definitioner som du vill visa.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa det maximala antalet delningsdefinitioner som du vill att modulen ska hämta under varje körningscykel för scenario.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Get Traffic Types]

Den här sökmodulen hämtar en lista med trafiktyper.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Split.io] konto till [!DNL Workfront Fusion], se <a href="#connect-split-io-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Split.io] till [!UICONTROL Workfront Fusion] </a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Workspace ID]</td> 
   <td>Markera eller mappa arbetsytan som innehåller de trafiktyper som du vill visa.</td> 
  </tr> 
 </tbody> 
</table>
