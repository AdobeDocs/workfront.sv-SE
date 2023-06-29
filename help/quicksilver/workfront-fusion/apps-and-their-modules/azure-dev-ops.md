---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Azure DevOps-moduler
description: I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Azure DevOps], samt ansluta till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: ecaa93c9-47bb-4fe1-87b4-d2e117cc68ae
source-git-commit: 0915dcce45b271ee18cdd8af5db4f0eb01f3cced
workflow-type: tm+mt
source-wordcount: '1561'
ht-degree: 0%

---

# [!DNL Azure DevOps] moduler

I en [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder [!DNL Azure DevOps], samt ansluta till flera tredjepartsprogram och -tjänster.

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

Används [!DNL Azure DevOps] moduler, du måste ha en [!DNL Azure] DevOps-konto.

## Anslut [!DNL Azure DevOps] till [!DNL Workfront Fusion] {#connect-azure-devops-to-workfront-fusion}

1. Lägg till en [!DNL Azure DevOps] till ditt scenario.
1. Klicka **[!UICONTROL Add]** bredvid [!UICONTROL Connection] fält.
1. I [!UICONTROL Connection Type] fält, markera **[!DNL Azure DevOps]**.

   >[!IMPORTANT]
   >
   >The [!UICONTROL [!DNL Azure DevOps] (Request All Scopes)] anslutningstypen kommer att bli inaktuell inom den närmaste framtiden. Därför rekommenderar vi inte att du använder den.

1. Fyll i följande fält:

   <table style="table-layout:auto">
        <tr>
            <td>[!UICONTROL Connection name]</td>
            <td>Ange ett namn för anslutningen som du skapar.</td>
        </tr>
      <tr>
            <td>[!UICONTROL Organization]</td>
            <td>Ange namnet på den organisation som du skapade din [!DNL Azure DevOps] program.</td>
        </tr>
    </table>

1. Klicka **[!UICONTROL Continue]** för att slutföra konfigurationen av anslutningen och fortsätta skapa ditt scenario.

## [!UICONTROL Azure DevOps] moduler och deras fält

När du konfigurerar [!DNL Azure DevOps] moduler, [!DNL Workfront Fusion] visar fälten som listas nedan. Tillsammans med dessa finns ytterligare [!DNL Azure DevOps] fält kan visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)
* [Sökningar](#searches)

### Utlösare

#### [!UICONTROL Watch for work items]

Denna snabbutlösarmodul kör ett scenario när en post läggs till, uppdateras eller tas bort i [!UICONTROL Azure DevOps].

Modulen returnerar alla standardfält som är associerade med posten, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Webhook]</td> 
   <td> <p>Välj eller lägg till en webkrok för modulen.</p> <p>Mer information om webhooks i utlösarmoduler finns i <a href="../../workfront-fusion/webhooks/instant-triggers-webhooks.md" class="MCXref xref">Direktutlösare (webhooks) i [!DNL Adobe Workfront Fusion]</a>.</p> <p>Mer information om hur du skapar en webkrok finns i <a href="../../workfront-fusion/apps-and-their-modules/webhooks-updated.md" class="MCXref xref">Webhooks</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Åtgärder

* [Anpassat API-anrop](#custom-api-call)
* [Läs post](#read-record)
* [Skapa en post](#create-a-record)
* [Uppdatera en arbetsuppgift](#update-a-work-item)
* [[!UICONTROL Upload an attachment]](#upload-an-attachment)
* [Hämta en bifogad fil](#download-an-attachment)
* [Länka arbetsobjekt]([!UICONTROL #link-work-items])

#### [!UICONTROL Custom API Call]

Med den här åtgärdsmodulen kan du göra ett anpassat autentiserat anrop till [!DNL Azure DevOps] API. På så sätt kan du skapa en dataflödesautomatisering som inte kan uppnås av andra [!DNL Azure DevOps] moduler.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Base URL]</td> 
   <td> <p>Välj eller mappa bas-URL:en som du använder för att ansluta till [!DNL Azure DevOps] konto</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Relative URL]</td> 
   <td> <p>Ange den relativa URL som du vill ansluta till för detta API-anrop.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span><code>{organization}/_apis[/{area}]/{resource}</code> </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!UICONTROL API Version]</td> 
   <td>Markera eller mappa versionen av [!DNL Azure DevOps] API som du vill ansluta till för detta API-anrop. Om ingen version är markerad [!DNL Workfront Fusion] ansluter till [!DNL Azure DevOps] API-version 5.1.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p> <p>Exempel: <code>{"Content-type":"application/json"}</code></p> </td> 
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

#### [!UICONTROL Read record]

Den här åtgärdsmodulen läser data från en enda post i [!DNL Azure DevOps].

Du anger postens ID.

Modulen returnerar postens ID och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj om du vill läsa ett projekt eller en arbetsuppgift</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong>: Välj det projekt som du vill läsa.</p> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong>: Välj det projekt som innehåller den arbetsuppgift som du vill läsa och välj sedan arbetsuppgiftstyp.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Välj den information som du vill inkludera i utdatapaketet för den här modulen. Vilka fält som är tillgängliga beror på arbetsobjekttypen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL ID]</td> 
   <td>Ange eller mappa ID:t för den post som du vill läsa.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Create a record]

Den här åtgärdsmodulen skapar ett nytt projekt eller en ny arbetsuppgift.

Modulen matar ut objekt-ID:t för det nya arbetsobjektet eller URL:en och statuskoden för ett nyligen skapat projekt.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Record type]</td> 
   <td> <p>Välj om du vill skapa en arbetsuppgift eller ett projekt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Project]</strong> </p> <p>Fyll i följande fält:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Name]</strong>:Ange eller mappa ett namn för det nya projektet.</p> </li> 
       <li> <p><strong>[!UICONTROL Description]</strong>:Ange eller mappa en beskrivning för det nya projektet. </p> </li> 
       <li> <p><strong>[!UICONTROL Visibility]</strong>: Välj om du vill att projektet ska vara offentligt eller privat. Användarna måste vara inloggade i organisationen och ha beviljats åtkomst till projektet för att kunna interagera med ett privat projekt. Offentliga projekt är synliga för användare som inte är inloggade på din organisation.</p> </li> 
       <li> <p><strong>[!UICONTROL Version control]</strong>: Välj om du vill att projektet ska användas [!DNL Git] eller [!UICONTROL Team Foundation Version Control (TFCV)] för versionskontroll.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item process]</strong>: Välj den arbetsprocess som du vill använda för projektet. Alternativen är [!UICONTROL Basic], [!UICONTROL Scrum], [!UICONTROL Capability Maturity Model Integration (CMMI)]och [!UICONTROL Agile].</p> <p>Mer information om [!DNL Azure DevOps] processer, se <a href="https://docs.microsoft.com/en-us/azure/devops/boards/work-items/guidance/choose-process?view=azure-devops&amp;tabs=basic-process">Välj en process</a> i [!DNL Azure DevOps] Dokumentation.</p> </li> 
      </ul> </li> 
     <li> <p><strong>[!UICONTROL Work item]</strong> </p> <p>Fyll i följande fält:</p> 
      <ul> 
       <li> <p><strong>[!UICONTROL Project]</strong>: Välj det projekt där du vill skapa arbetsuppgiften.</p> </li> 
       <li> <p><strong>[!UICONTROL Work item type]</strong>: Välj den typ av arbetsuppgift som du vill skapa.</p> </li> 
       <li> <p><strong>[!UICONTROL Other fields]</strong>:I dessa fält anger du det värde som du vill att arbetsposten ska ha för en viss egenskap. Vilka fält som är tillgängliga beror på arbetsobjekttypen.</p> </li> 
      </ul> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Update a work item]

Den här åtgärdsmodulen uppdaterar ett befintligt arbetsobjekt med dess ID.

Modulen returnerar ID:t för det uppdaterade arbetsobjektet.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Välj det projekt som innehåller den arbetsuppgift som du vill uppdatera.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work Item Type]</td> 
   <td> <p>Välj den typ av arbetsuppgift som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Other Fields]</td> 
   <td>I vart och ett av dessa fält anger du det värde som du vill att arbetsposten ska ha för en viss egenskap. Vilka fält som är tillgängliga beror på arbetsobjekttypen.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Ange eller mappa ID:t för den arbetsuppgift som du vill uppdatera.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Upload an attachment]

Den här åtgärdsmodulen överför en fil och bifogar den till ett arbetsobjekt.

Modulen returnerar den bifogade filens ID och en hämtnings-URL för den bifogade filen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project] </td> 
   <td> <p>Välj det projekt där du vill överföra en bifogad fil.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td> <p>Ange eller mappa ID:t för arbetsuppgiften där du vill överföra en bifogad fil.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Ange texten för en kommentar som du vill lägga till i den överförda bilagan.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Source file] </td> 
   <td>Välj en källfil från en tidigare modul eller ange eller mappa källfilens namn och innehåll.</td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Download an attachment]

Den här åtgärdsmodulen hämtar en bifogad fil.

Modulen returnerar filinnehållet i den bifogade filen.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Attachment URL]</td> 
   <td> <p>Ange eller mappa URL:en för den bifogade fil som du vill hämta.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### [!UICONTROL Link work items]

Den här åtgärdsmodulen länkar två arbetsobjekt och definierar relationen mellan dem.

Modulen returnerar ID:t för huvudobjektet och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item ID]</td> 
   <td>Ange eller mappa ID:t för det huvudsakliga arbetsobjekt som du vill länka ett annat arbetsobjekt till.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Linked work item ID]</td> 
   <td>Ange eller mappa ID:t för arbetsuppgiften som du vill länka till huvudarbetsuppgiften.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Link Type]</td> 
   <td> <p>Definiera relationen mellan arbetsobjekten som du vill länka.</p> <p>Mer information finns i <a href="https://docs.microsoft.com/en-us/azure/devops/boards/queries/link-type-reference?view=azure-devops">Referens för länktyp</a> i [!UICONTROL Azure DevOps] Dokumentation.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment]</td> 
   <td>Ange eller mappa texten i en kommentar. Detta är användbart för att förklara länkens resonemang eller avsikt.</td> 
  </tr> 
 </tbody> 
</table>

### Sökningar

#### [!UICONTROL List work items]

Den här åtgärdsmodulen hämtar alla arbetsobjekt av en viss typ i en [!DNL Azure DevOps] projekt.

Modulen returnerar ID:t för huvudobjektet och eventuella associerade fält, tillsammans med eventuella anpassade fält och värden som anslutningen har åtkomst till. Du kan mappa den här informationen i efterföljande moduler i scenariot.

När du konfigurerar den här modulen visas följande fält.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
   <td> <p>Instruktioner om hur du ansluter [!DNL Azure DevOps] konto till [!DNL Workfront Fusion], se <a href="#connect-azure-devops-to-workfront-fusion" class="MCXref xref">Anslut [!DNL Azure DevOps] till [!UICONTROL Workfront Fusion]</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Project]</td> 
   <td>Välj det projekt som du vill hämta arbetsobjekt från.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Work item type]</td> 
   <td> <p>Välj den typ av arbetsuppgift som du vill hämta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Outputs]</td> 
   <td>Markera de egenskaper som du vill ska visas i modulens utdata. Vilka fält som är tillgängliga beror på vilken typ av arbetsobjekt du vill hämta. Du måste välja minst en egenskap.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit]</td> 
   <td>Ange eller mappa maximalt antal arbetsobjekt som [!DNL Workfront Fusion] returneras under en körningscykel.</td> 
  </tr> 
 </tbody> 
</table>
