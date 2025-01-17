---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe I/O Events-moduler
description: Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats. Den här artikeln har tagits bort, men innehåller en länk till den nya artikeln som innehåller den här funktionen.
author: Becky
feature: Workfront Fusion, Digital Content and Documents
exl-id: 18ad8098-9742-44d2-97cd-b0c2b5591538
source-git-commit: efbe888d370e20c895dc40f18f999f2d01ec6337
workflow-type: tm+mt
source-wordcount: '931'
ht-degree: 0%

---

# Adobe I/O Events-moduler

>[!IMPORTANT]
>
>Adobe Workfront Fusion-dokumentationen har flyttats till en ny plats.
>
>Informationen i den här artikeln finns nu i artikeln:
>
>* [Adobe I/O Events-moduler](https://experienceleague.adobe.com/docs/workfront-fusion/using/references/apps-and-their-modules/adobe-connectors/adobe-io-events-modules.html)
>
>Uppdatera eventuella bokmärken.
>
>Artikeln uppdateras inte längre och kommer att tas bort inom den närmaste framtiden.

Med Adobe I/O Events-modulen kan du starta ett Adobe Workfront Fusion-scenario baserat på händelser i Adobe-konton och -tjänster som inte har någon särskild Workfront Fusion-anslutning.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Planera, arbeta</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront Fusion-licens**</td> 
   <td> <p>Workfront Fusion for Work Automation and Integration </p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td>Din organisation måste köpa både Adobe Workfront Fusion och Adobe Workfront för att kunna använda de funktioner som beskrivs i den här artikeln.</td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

&#42;&#42;Mer information om Adobe Workfront Fusion-licenser finns i [Adobe Workfront Fusion-licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md)

## Förutsättningar

Innan du kan använda Adobe I/O Events-kopplingen måste du se till att följande krav uppfylls:

* Du måste ha ett aktivt Adobe-konto.

## API-information för händelser i Adobe I/O

I Adobe I/O Events-kopplingen används följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bas-URL</td> 
   <td>https://api.adobe.io/events</td> 
  </tr>
  <tr> 
   <td role="rowheader">API-tagg</td> 
   <td>v1.6.7</td> 
  </tr>
 </tbody> 
 </table>

## Skapa en anslutning till Adobe I/O-händelser

Så här skapar du en anslutning för dina Adobe I/O-händelsemoduler:

1. Klicka på Lägg till bredvid rutan Anslutning.

1. Fyll i följande fält:

   <table style="table-layout:auto"> 
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
    </col>
    <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
    </col>
    <tbody>
      <tr>
        <td role="rowheader">Anslutningsnamn</td>
        <td>
          <p>Ange ett namn för anslutningen.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Typ</td>
        <td>
          <p>Välj om du vill ansluta till ett tjänstkonto eller ett personligt konto.</p>
        </td>
      </tr>
      <tr>
        <td role="rowheader">Ytterligare omfattningar</td>
        <td>Om du vill lägga till ytterligare omfattningar klickar du på <b>Lägg till objekt</b> och anger omfånget.</td>
      </tr>
      <tr>
        <td role="rowheader">Klient-ID</td>
        <td>Ange ditt klient-ID för Adobe. Detta hittar du i delen Information om autentiseringsuppgifter i Adobe Developer Console</td>
      </tr>
      <tr>
        <td role="rowheader">Klienthemlighet</td>
        <td>Ange din Adobe-klienthemlighet. Detta hittar du i delen Information om autentiseringsuppgifter i Adobe Developer Console</td>
      </tr>
      </tr>
        <tr>
        <td role="rowheader">Konsumentorganisations-ID</td>
        <td>Ange ditt konsument-organisations-ID. Detta finns i projektets referens-URL: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">ID för autentiseringsuppgifter</td>
        <td>Ange ditt ID för autentiseringsuppgifter. Detta finns i projektets referens-URL: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">ID för IMS-organisation</td>
        <td>Ange ditt organisations-ID för Adobe. Detta hittar du i delen Information om autentiseringsuppgifter i Adobe Developer Console</td>
      </tr>
        <tr>
        <td role="rowheader">Projekt-ID</td>
        <td>Ange ditt projekt-ID. Detta finns i projektets referens-URL: <code>https://developer.adobe.com/console/projects/{consumer org ID}/ {project ID}/credentials/{credential ID}/details</code></td>
      </tr>
      <tr>
        <td role="rowheader">WORKSPACE ID</td>
        <td>Om du vill visa ditt projekts Workspace-id hämtar du projektinformationen från projektöversiktssidan i Adobe Developer Console. </td>
      </tr>
    </tbody>
    </table>

1. Klicka på **Fortsätt** för att spara anslutningen och återgå till modulen.

## Adobe I/O Events-moduler och deras fält

När du konfigurerar [!DNL Adobe I/O Events] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!DNL Adobe I/O Events] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Utlösare](#triggers)
* [Åtgärder](#actions)
* [Sökningar](#searches)

### Utlösare

#### Skapa en händelseregistrering

Den här åtgärdsmodulen använder en webkrok för att skapa en händelsebeskrivning. Du kan konfigurera en webkrok här. Om du använder en befintlig webkrok är fälten i den här modulen skrivskyddade.

Så här skapar du en webkrok:

1. Klicka på **Lägg till** bredvid Webkrok-fältet.
1. Fyll i följande fält:

   <table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Webhook name]</td>
        <td>Ange ett namn för den här webbkroken.</td>
       </tr>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe I/O Events] finns i <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe I/O Events]</a> i den här artikeln.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Webhook description]
         </td>
         <td>
           Ange en beskrivning för den här webbkroken.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event provider]
         </td>
         <td>
           Välj den produkt eller det konto som du vill skapa händelser från.
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event type]
         </td>
         <td>
           Välj de händelser som du vill att webbhollen ska titta på. Scenariot utlöses när dessa händelser inträffar.
         </td>
       </tr>
     </tbody>
   </table>

1. Klicka på Spara om du vill spara webkroken och återgå till modulen.

### Åtgärder

#### Hämta alla händelser från en journal

Den här sökmodulen hämtar alla händelser för registrering från en journal.

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe I/O Events] finns i <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe I/O Events]</a> i den här artikeln.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Registration ID]
         </td>
         <td>
           Välj den registrering som du vill hämta händelser för.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Maximum number of returned records]
         </td>
         <td>
              Ange eller mappa det maximala antal poster som du vill att modulen ska returnera under varje körningscykel för scenario. 
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Return events that occur after]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Seek]
         </td>
         <td>
         </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Latest]
         </td>
         <td>
         Aktivera det här alternativet om du vill returnera den senaste händelsen.
         </td>
       </tr>
     </tbody>
   </table>

#### Göra ett anpassat API-anrop

Den här åtgärdsmodulen gör ett anpassat API-anrop till API:t [!DNL Adobe I/O Events]

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
     <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe I/O Events] finns i <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe I/O Events]</a> i den här artikeln.</td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Path]</p>
      </td>
      <td>
        <p>Ange en sökväg i förhållande till <code>https://api.adobe.io/events</code></p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">
        <p>[!UICONTROL Method]</p>
      </td>
      <td>
  <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">Metoder för HTTP-begäran i [!DNL Adobe Workfront Fusion]</a>.</p>  
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Headers]</td>
      <td>
        <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt.</p>
        <p>Exempel: <code>{"Content-type":"application/json"}</code></p>
        <p>Workfront Fusion lägger automatiskt till auktoriseringshuvuden och x-api-key-huvuden.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Query String]  </td>
      <td>
        <p>Ange frågesträngen för begäran.</p>
      </td>
    </tr>
    <tr>
      <td role="rowheader">[!UICONTROL Body]</td>
   <td> <p>Lägg till brödinnehållet för API-anropet i form av ett standard-JSON-objekt.</p> <p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar du citattecknen utanför villkorssatsen.</p> 
     <div class="example" data-mc-autonum="<b>Example: </b>"> 
      <p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p> 
     </div> </p> </td>     </tr>
  </tbody>
</table>

### Sökningar

#### Hämta provider- och händelse-ID:n

Den här sökmodulen hämtar Adobe I/O-händelse-ID:n för den angivna providern och händelser.

<table>
     <col/>
     <col/>
     <tbody>
       <tr>
         <td role="rowheader">[!UICONTROL Connection]</td>
        <td>Instruktioner om hur du skapar en anslutning till [!DNL Adobe I/O Events] finns i <a href="#create-a-connection-to-adobe-io-events" class="MCXref xref" >Skapa en anslutning till [!DNL Adobe I/O Events]</a> i den här artikeln.</td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event provider]
         </td>
         <td>
           Välj den leverantör som du vill hämta ID:t för.
        </td>
       </tr>
       <tr>
         <td role="rowheader">
           [!UICONTROL Event type]
         </td>
         <td>
              Välj de händelser som du vill ange ID:n för. Händelser är tillgängliga baserat på händelseprovidern. 
         </td>
       </tr>
     </tbody>
   </table>

<!--

Watch Events

This trigger module starts a scenario when an event occurs in the chosen Adobe product or service.

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
   <tr> 
   <td role="rowheader">Webhook</td> 
   <td><p>Select the webhook that you want to use for this trigger, or add a new webhook. </p><p>To add a new webhook, <ol><li>Click <b>Add</b> next to the webhook field.</li><li>Enter the following: <ul><li>A name for the webhook</li><li>The connection that you want to use for this webhook</li><li>The source of the events you want to watch</li></ul></li><li>Click <b>Save</b> to save the webhook and return to the module. </td> 
   </tr> 
   </tbody> 
</table>

-->
