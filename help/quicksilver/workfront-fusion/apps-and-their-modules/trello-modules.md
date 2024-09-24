---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Trello-moduler
description: I ett [!DNL Adobe Workfront Fusion] scenario kan du automatisera arbetsflöden som använder Trello och ansluta det till flera tredjepartsprogram och -tjänster.
author: Becky
feature: Workfront Fusion
exl-id: 60630b23-e057-4ecf-a014-6e63b6d69b48
source-git-commit: 16cd5dee183153540bcccea8ce469a461d0e8562
workflow-type: tm+mt
source-wordcount: '4233'
ht-degree: 0%

---

# [!UICONTROL Trello] moduler

I ett [!DNL Adobe Workfront Fusion]-scenario kan du automatisera arbetsflöden som använder [!UICONTROL Trello] samt ansluta det till flera tredjepartsprogram och -tjänster.

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

## Förutsättningar

Du måste ha ett [!UICONTROL Trello]-konto för att kunna använda [!DNL Trello]-moduler.

## Anslut [!UICONTROL Trello] till [!DNL Workfront Fusion]

Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i [Skapa en anslutning till  [!DNL Adobe Workfront Fusion] - Grundläggande instruktioner](../../workfront-fusion/connections/connect-to-fusion-general.md)

## [!UICONTROL Trello]-moduler och deras fält

När du konfigurerar [!UICONTROL Trello] moduler visar [!DNL Workfront Fusion] fälten som listas nedan. Dessutom kan ytterligare [!UICONTROL Trello] fält visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Varumärkena](#boards)
* [Listor](#lists)
* [Kort](#cards)
* [Medlemmar](#members)
* [Checklistor](#checklists)
* [Etiketter](#labels)
* [Kommentar](#comments)

### Varumärkena

+++ **[!UICONTROL Watch Boards]**

Den här utlösarmodulen startar ett scenario när en ny anslagstavla läggs till.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Det högsta antalet ritytor [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Board]**

Den här åtgärdsmodulen skapar en ny anslagstavla med de valda inställningarna.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange eller mappa ett namn för den nya ritytan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Description]</td> 
   <td> <p>Ange eller mappa kortbeskrivningen om det behövs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Ange eller mappa organisationens ID. Organisations-ID kan hämtas med hjälp av en annan modul, till exempel modulen Bevakade aktiviteter.</p> <p> <img src="assets/id-of-org.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Permission level]</p> </td> 
   <td> <p>Styrelserna har olika regler för omröstning och kommentarer för varje behörighetsnivå. Om din styrelse till exempel är [!UICONTROL Private] och du anger röstregler och kommentarsregler som [!UICONTROL All] får du ett felmeddelande. </p> <p>Omröstning och kommentarer är begränsade till följande grupper för varje behörighetsnivå:</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: 
      —&gt;Medlemmar, medlemmar och observatörer</li> 
     <li><strong>[!UICONTROL For organization]</strong>: 
      —&gt;Medlemmar, medlemmar och observatörer, organisationsmedlemmar</li> 
     <li><strong>[!UICONTROL Public]</strong>: 
      —&gt;Medlemmar, medlemmar och observatörer, organisationsmedlemmar, alla</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>Välj ett alternativ för att ange vem som får rösta i den här styrelsen. Se fältet [!UICONTROL Permission level] för röstbegränsningar på behörighetsnivåer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>Välj ett alternativ för att ange vem som kan kommentera kort för den här anslagstavlan. Gå till fältet [!UICONTROL Permission level] för att kommentera begränsningar för behörighetsnivåer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Invitations]</p> </td> 
   <td> <p>Välj vem som kan bjuda in andra personer till den här styrelsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Self-join]</p> </td> 
   <td> <p>Välj om teammedlemmarna ska kunna gå med i styrelsen själva eller om de ska bli inbjudna.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Default labels]</p> </td> 
   <td> <p>Välj om du vill använda standarduppsättningen med etiketter för den nya ritytan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Default lists]</p> </td> 
   <td> <p>Välj om du vill lägga till standarduppsättningen med listor på anslagstavlan ([!UICONTROL To Do], [!UICONTROL Doing], [!UICONTROL Done]).</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board source ID]</p> </td> 
   <td> <p>Markera eller mappa ID:t för den anslagstavla som du vill kopiera till den nya anslagstavlan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card Covers]</p> </td> 
   <td> <p>Välj <strong>[!UICONTROL Yes]</strong> om du vill aktivera kortomslag för kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Background]</p> </td> 
   <td> <p>Välj bakgrundsfärgen eller den anpassade bakgrunden.</p> <p>Obs! Anpassade bakgrunder är bara tillgängliga för [!UICONTROL Trello Gold and Business Class] prenumeranter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>Välj mellan två sätt att föråldra kort. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Korten blir allt mer transparenta allt eftersom de blir äldre. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>Korten kommer att riva, gult och spricka som en gammal piratkarta när de blir gamla.</li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Edit a Board]**

Den här åtgärdsmodulen redigerar inställningarna för en befintlig anslagstavla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Ange eller mappa det unika [!UICONTROL Trello]-ID:t för den anslagstavla som du vill att modulen ska skapa. Du kan hämta anslagstavlans ID med hjälp av en annan modul, som till exempel bevakningsmodulen</p> <p> <img src="assets/watch-boards.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td> <p> Ange eller mappa ett nytt namn för ritytan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New description]</td> 
   <td> <p> Ange eller mappa en ny kortbeskrivning om det behövs.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Organization ID]</p> </td> 
   <td> <p>Ange eller mappa det unika [!UICONTROL Trello]-ID:t för den anslagstavla som du vill att modulen ska redigera. Du kan hämta kort-ID:t med en annan modul, till exempel modulen [!DNL Watch Activities].</p> <p> <img src="assets/org-id.png"> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>Välj ett alternativ för att ange om den agerande användaren prenumererar på styrelsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Permission level]</p> </td> 
   <td> <p>Styrelserna har olika regler för omröstning och kommentarer för varje behörighetsnivå. Om din styrelse till exempel är [!UICONTROL Private] och du anger röstregler och kommentarsregler som [!UICONTROL All] får du ett felmeddelande. </p> <p>Omröstning och kommentarer är begränsade till följande grupper för varje behörighetsnivå:</p> 
    <ul> 
     <li><strong>[!UICONTROL Private]</strong>: 
      —&gt;Medlemmar, medlemmar och observatörer</li> 
     <li><strong>[!UICONTROL For organization]</strong>: 
      —&gt;Medlemmar, medlemmar och observatörer, organisationsmedlemmar</li> 
     <li><strong>[!UICONTROL Public]</strong>: 
      —&gt;Medlemmar, medlemmar och observatörer, organisationsmedlemmar, alla</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Voting]</p> </td> 
   <td> <p>Välj ett alternativ för att ange vem som får rösta i den här styrelsen. Se fältet [!UICONTROL Permission level] för röstbegränsningar på behörighetsnivåer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Comments]</p> </td> 
   <td> <p>Välj ett alternativ för att ange vem som kan kommentera kort för den här anslagstavlan. Gå till fältet [!UICONTROL Permission level] för att kommentera begränsningar för behörighetsnivåer.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Invitations] </td> 
   <td> <p>Välj vem som kan bjuda in personer till den här styrelsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Self-join]</td> 
   <td> <p> Välj om teammedlemmarna ska kunna gå med i styrelsen själva eller om de ska bli inbjudna.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card covers]</td> 
   <td> <p> Välj om kortomslag ska visas på den här anslagstavlan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background] </td> 
   <td> <p>Välj bakgrundsfärgen eller den anpassade bakgrunden.</p> <p>Obs! Anpassade bakgrunder är bara tillgängliga för [!UICONTROL Trello Gold and Business Class] prenumeranter.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Background ID]</td> 
   <td> <p> Om du har valt att använda en anpassad bakgrund i fältet [!UICONTROL Background] anger eller mappar du ID:t för bakgrunden som du vill använda.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Card aging]</p> </td> 
   <td> <p>Välj mellan två sätt att föråldra kort. </p> 
    <ul> 
     <li><strong>[!UICONTROL Regular]</strong>: Korten blir allt mer transparenta allt eftersom de blir äldre. </li> 
     <li><strong>[!UICONTROL Pirate]</strong>Korten kommer att riva, gult och spricka som en gammal piratkarta när de blir gamla.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Calendar feed enabled]</td> 
   <td> <p> Ange om kalenderfeeden är aktiverad eller inte.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL <Color> label name]</td> 
   <td> <p> Tilldela ett namn till den önskade färgetiketten.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Välj ett alternativ som anger om du vill arkivera (stänga) styrelsen. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a Board]**

Den här åtgärdsmodulen hämtar information om en styrelse.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Board ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för den anslagstavla som du vill hämta information om.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!DNL Search for Boards]**

Den här sökmodulen hämtar information om en anslagstavla som du anger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Ange eller mappa namnet (eller en del av namnet) på den anslagstavla som du vill ha information om.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned boards]</td> 
   <td> <p> Ange det maximala antalet ritytor som [!DNL Workfront Fusion] returnerar under en körningscykel. Värdet måste vara mindre än eller lika med 1 000.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Partial] </p> </td> 
   <td> <p>Som standard söker den här modulen efter medlemsinnehåll efter exakta matchningar av varje ord i frågan. När [!UICONTROL Partial] är aktiverat söker modulen efter innehåll som börjar med ett ord i frågan.</p> <p> Om du t.ex. använder ordet"utveckling" för att söka efter en panel med namnet"Min utvecklingsstatusrapport", måste du som standard söka efter hela ordet. Om du har [!UICONTROL Partial] aktiverat kan du söka efter "dev" men inte "Development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Boards] </td> 
   <td> <p>Ange "min" eller mappa en kommaavgränsad lista med kort-ID:n.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archive or Unarchive a Board]**

Den här åtgärdsmodulen stänger eller öppnar en anslagstavla som du anger igen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Ange eller mappa ID:t för den anslagstavla som du vill stänga eller öppna igen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive or unarchive]</td> 
   <td> <p> Välj om du vill stänga (arkivera) eller öppna styrelsen igen (utan arkiv).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Assign a Member to a Board]**

Den här åtgärdsmodulen tilldelar en medlem till en anslagstavla som du anger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Välj den anslagstavla där du vill lägga till en medlem.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Email address]</td> 
   <td> <p> Ange eller mappa e-postadressen till den medlem du vill lägga till i styrelsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Member type]</p> </td> 
   <td> <p>Välj den typ av medlem som du vill lägga till i styrelsen.</p> 
    <ul> 
     <li><strong>[!UICONTROL Admin]</strong>: En styrelseledamot kan utföra vilken styrelseledamot som helst.</li> 
     <li><strong>[!UICONTROL Normal]</strong>: En normal medlem är helt enkelt styrelseledamot.</li> 
     <li><strong>[!UICONTROL Observer]</strong>: En observatör är medlem med skrivskyddad tillgång till styrelsen. <br>Observatörer är bara tillgängliga för team med [!UICONTROL Trello Business Class].</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Full name]</td> 
   <td> <p> Ange det fullständiga namnet på den användare som du vill lägga till i anslagstavlan.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Unassign a Member from a Board]**

Den här åtgärdsmodulen tar bort en medlem från en anslagstavla.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Ange (mappa eller välj) ID:t för den anslagstavla som du vill ta bort användaren från.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Member] </td> 
   <td> <p>Markera den medlem du vill ta bort från styrelsen.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Listor

+++ **[!UICONTROL Watch cards moved to a list]**

Den här utlösarmodulen aktiveras när ett kort flyttas till en viss lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board]</td> 
   <td>Välj den anslagstavla som innehåller listan som du vill bevaka efter kort.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List]</td> 
   <td>Välj den lista som du vill bevaka efter kort.</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Det maximala antalet kort [!DNL Workfront Fusion] returneras under en körningscykel.</p>  </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a List]**

Den här åtgärdsmodulen skapar en lista på en anslagstavla som du anger.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Ange eller mappa ID:t för den anslagstavla där du vill skapa en lista.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange eller mappa ett namn för den nya listan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Välj om du vill lägga till listan överst eller lägga till den längst ned på kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy list]</td> 
   <td> <p> Välj hur du vill ange ID:t för listan som du vill kopiera.</p> 
    <ul> 
     <li> <p><strong>Ange manuellt</strong> </p> <p>Ange eller mappa ID:t för den lista du vill kopiera i fältet <strong>[!UICONTROL List ID]</strong>.<br></p> </li> 
     <li> <p><strong>Välj</strong> </p> <p>Markera den anslagstavla som innehåller listan som du vill kopiera och markera sedan listan.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Edit a List]**

Den här åtgärdsmodulen redigerar en befintlig lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL List ID]</td> 
   <td> <p> Ange eller mappa ID:t för listan som du vill uppdatera.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange eller mappa ett nytt namn för listan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p> Karta eller välj den anslagstavla där du vill flytta listan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Välj om du vill lägga till listan överst eller lägga till den längst ned på kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribed]</td> 
   <td> <p>Aktivera det här alternativet om du vill prenumerera på den aktiva medlemmen i listan.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a List]**

Den här åtgärdsmodulen hämtar information om en viss lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL List ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för listan som du vill hämta information om.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Kort

+++ **[!UICONTROL Watch cards]**

Denna utlösarmodul aktiveras när ett nytt kort läggs till.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched object]</td> 
   <td> <p>Välj den plats som du vill bevaka efter kort.</p> 
    <ul> 
     <li><strong>[!UICONTROL All cards]</strong> </li> 
     <li> <p><strong>Kort på en särskild anslagstavla</strong> </p> <p>Välj den anslagstavla som du vill bevaka efter kort</p> </li> 
     <li> <p><strong>[!UICONTROL Cards on specific list]</strong> </p> <p>Markera den anslagstavla som innehåller listan som du vill bevaka efter kort och markera sedan listan.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Det maximala antalet kort [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a card]**

Den här åtgärdsmodulen skapar ett kort i en markerad lista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a list ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för listan där du vill lägga till ett kort.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa ID:t för listan där du vill lägga till ett kort i fältet <strong>[!UICONTROL List ID]</strong>.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Markera den anslagstavla som innehåller listan som du vill kopiera och markera sedan listan.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Ange etikettens ID för varje etikett som du vill lägga till på kortet. ID kan till exempel hämtas med modulen [!UICONTROL Retrieve Labels].</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members]</td> 
   <td>Ange medlemmens ID för varje medlem som du vill lägga till på kortet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange ett namn för det nya kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Description]</p> </td> 
   <td> <p>Ange kortets beskrivning.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Välj om du vill lägga till kortet överst eller [!UICONTROL append] kortet längst ned i listan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due date]</td> 
   <td> <p> Ange kortets förfallodatum. En lista över vilka datum- och tidsformat som stöds finns i <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due complete]</td> 
   <td> <p> Aktivera det här alternativet för att markera att kortet är klart på förfallodatumet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL File URL]</td> 
   <td> <p>Ange eller mappa URL:en för en fil som du vill lägga till som en bilaga till kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Source file]</p> </td> 
   <td> <p>Ange eller mappa information för en fil som du vill lägga till som en bilaga till kortet.</p> 
    <ul> 
     <li>[!UICONTROL File name]: Ange eller mappa filnamnet, inklusive filtillägget.</li> 
     <li> 
     <p>Välj en fil från en tidigare modul eller mappa filens namn och data</p> 
     <p>Obs! Det finns en gräns på 10 MB för filöverföring per bifogad fil. [!UICONTROL Business Class]- och [!UICONTROL Trello Gold]-medlemmar har dock en filöverföringsgräns på 250 MB per bifogad fil.</p> 
     </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Copy card]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet som du vill kopiera.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa ID:t för kortet som du vill kopiera i fältet <strong>[!UICONTROL Card ID]</strong>.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet du vill kopiera, markera sedan listan som innehåller kortet och markera sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Edit a Card]**

Den här åtgärdsmodulen redigerar ett befintligt kort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter Card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet som du vill redigera.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa ID:t för kortet som du vill redigera i fältet <strong>[!UICONTROL Card ID]</strong>.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Markera den anslagstavla som innehåller kortet som du vill redigera, markera sedan listan som innehåller kortet och markera sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL New name]</td> 
   <td> <p>Ange eller mappa ett nytt namn för kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL New description]</p> </td> 
   <td> <p>Ange eller mappa en ny beskrivning för kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Move a card]</p> </td> 
   <td> <p>Välj den bräda eller den bräda och lista där du vill flytta kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Labels] </td> 
   <td> <p>Lägg till ID:n för etiketter som du vill lägga till på kortet. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Välj om du vill lägga till kortet överst eller [!UICONTROL append] kortet längst ned i listan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due date]</td> 
   <td> <p> Ange kortets förfallodatum. En lista över vilka datum- och tidsformat som stöds finns i <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Due complete]</td> 
   <td> <p> Om det här alternativet är aktiverat markeras kortet som fullständigt på förfallodatumet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Members] </td> 
   <td> <p>Lägg till eller mappa ID:t för medlemmar som du vill lägga till på kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment cover ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för bildbilagan som du vill att kortet ska använda som omslag.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Subscribe] </td> 
   <td> <p>Ange om medlemmen ska prenumerera på kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive] </td> 
   <td> <p>Välj ett alternativ som anger om du vill arkivera (stänga) kortet. </p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Get a Card]**

Den här åtgärdsmodulen hämtar information om det valda kortet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board ID]</td> 
   <td> <p>Ange ID:t för den bräda som innehåller kortet som du vill hämta information om. På så sätt kan du se namn på styrelsens anpassade fält.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet som du vill hämta information om.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa ID:t för kortet som du vill hämta information om i fältet <strong>[!UICONTROL Card ID]</strong>.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet som du vill hämta information om, markera sedan listan som innehåller kortet och välj sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for Cards]**

Den här åtgärdsmodulen returnerar kort som matchar sökfrågan.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Board] </td> 
   <td> <p>Markera de anslagstavlor som du vill söka igenom. Om ingen anslagstavla är markerad söks alla anslagstavlor igenom.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Query]</p> </td> 
   <td> <p>Ange sökfrågan. Du kan begränsa sökningen med följande sökoperatorer:</p> 
    <ul> 
     <li><code><strong>-operator</strong></code> <p>Du kan lägga till "-" till valfri operator om du vill göra en negativ sökning, till exempel <code>[!UICONTROL -has:members]</code>, om du vill söka efter kort utan tilldelade medlemmar.</p> </li> 
     <li><code><strong>@name</strong></code> <p>Returnerar kort som tilldelats en medlem. Du kan också använda <code>member:</code>. Använd <code>@me</code> om du bara vill inkludera dina kort.</p> </li> 
     <li><code><strong>#label</strong></code> <p>Returnerar märkta kort. Du kan också använda <code>label:</code>. <code>label:"FIX IT"</code> returnerar till exempel kort med etiketten FIX IT.</p> </li> 
     <li><code><strong>board:id</strong></code> <p>Returnerar kort inom en viss anslagstavla. <code>board:Trello</code> returnerar till exempel kort på ritytor med [!UICONTROL Trello] i kortnamnet.</p> </li> 
     <li><code><strong>list:name</strong></code> <p>Returnerar kort i listan med namnet"name".</p> </li> 
     <li><code><strong>has:attachments</strong></code> <p>Returnerar kort med bifogade filer. Operatorn <code>has</code>: kan även användas med andra attribut, till exempel <code>has:description</code>, <code>has:cover</code>, <code>has:members</code> eller <code>has:stickers</code>.</p> </li> 
     <li><code><strong>due:day</strong></code> <p>Returnerar kort som förfaller inom 24 timmar. Operatorn <code>due:</code> kan också användas med andra tidsramar, till exempel <code>due:week</code>, <code>due:month</code> eller <code>due:overdue</code>. Du kan också söka efter ett visst datumintervall. Om du till exempel lägger till <code>due:14</code> i sökningen inkluderas kort som förfaller inom de kommande 14 dagarna.</p> </li> 
     <li><code><strong>created:day</strong></code> <p>Returnerar kort som skapats de senaste 24 timmarna. Operatorn <code> created:</code> kan också användas med andra tidsramar som <code>created:week</code> eller <code>created:month</code>. Du kan också söka efter ett visst datumintervall. Om du till exempel lägger till <code>created:14</code> i sökningen inkluderas kort som skapats de senaste 14 dagarna.</p> </li> 
     <li><code><strong>edited:day</strong></code> <p>Returnerar kort som har redigerats de senaste 24 timmarna. Operatorn <code>edited:</code> kan också användas med andra tidsramar, till exempel <code>edited:week</code> eller <code>edited:month</code>. Du kan också söka efter ett visst datumintervall. Om du till exempel lägger till <code>edited:21</code> i sökningen inkluderas kort som har redigerats de senaste 21 dagarna.</p> </li> 
     <li><code><strong>description:</strong>, <strong>checklist:</strong>, <strong>comment:</strong>, and <strong>name:</strong></code> <p>Returnerar kort som matchar texten i kortbeskrivningar, checklistor, kommentarer eller namn. Exempel:"FIX IT" returnerar kort med"FIX IT" i en kommentar.</p> </li> 
     <li><code><strong>is:open</strong> and <strong>is:archived</strong></code> <p>Returnerar kort som är öppna eller arkiverade. Om inget anges returnerar [!UICONTROL Trello] båda typerna.</p> </li> 
     <li><code><strong>is:starred</strong> </code> <p>Inkluderar endast kort på styrbord.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned cards]</td> 
   <td> <p> Det maximala antalet kort [!DNL Workfront Fusion] returneras under en körningscykel. Värdet måste vara mindre än eller lika med 1 000.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>Som standard söker den här modulen efter medlemsinnehåll efter exakta matchningar av varje ord i frågan. När [!UICONTROL Partial] är aktiverat söker modulen efter innehåll som börjar med ett ord i frågan.</p> <p> Om du t.ex. använder ordet"utveckling" för att söka efter en panel med namnet"Min utvecklingsstatusrapport", måste du som standard söka efter hela ordet. Om du har [!UICONTROL Partial] aktiverat kan du söka efter "dev" men inte "Development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Cards] </td> 
   <td> <p>Lägg till kort som du vill söka efter.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Archive or Unarchive a Card]**

Den här åtgärdsmodulen arkiverar eller skickar tillbaka ett kort till styrelsen.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Card ID]</td> 
   <td> <p> Ange eller mappa ID:t för kortet som du vill arkivera eller skicka tillbaka till styrelsen.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Archive or unarchive]</td> 
   <td> <p> Välj om du vill stänga kortet (arkivet) eller skicka tillbaka det till styrelsen (ej arkiverat).</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Add an Attachment]**

Den här åtgärdsmodulen lägger till en bifogad fil till det markerade kortet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet som du vill hämta information om.</p> 
    <ul> 
     <li> <p><strong>Ange manuellt</strong> </p> <p>Ange eller mappa ID:t för kortet som du vill hämta information om i fältet <strong>[!UICONTROL Card ID]</strong>.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet som du vill hämta information om, markera sedan listan som innehåller kortet och välj sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Attachment type]</p> </td> 
   <td> <p>Välj om du vill överföra filen direkt eller ange en URL till filen.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL File]</strong> </p> <p>Välj en källfil från en tidigare modul eller mappa källfilens namn och data.</p> </li> 
     <li> <p><strong>[!UICONTROL URL]</strong> </p> <p>Ange URL-adressen till filen och ange ett namn för den bifogade filen.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Medlemmar

+++ **[!UICONTROL Assign a Member to a Board]**

Se &quot;[!UICONTROL Assign a Member to a Board]&quot; under [Vykort](#boards).

+++

+++ **[!UICONTROL Unassign a Member from a Board]**

Se &quot;[!UICONTROL Unassign a Member from a Board]&quot; under [Vykort](#boards).

+++

+++ **[!UICONTROL Add a Member to a Card]**

Den här åtgärdsmodulen lägger till den angivna medlemmen på det angivna kortet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Enter card ID and member ID]</p> </td> 
   <td> <p>Välj hur du vill ange kort-ID och medlems-ID.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>Ange eller mappa <strong>[!UICONTROL Card ID]</strong> och <strong>[!UICONTROL Member ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Markera den anslagstavla som innehåller kortet som du vill lägga till en medlem i och markera sedan listan som innehåller kortet, själva kortet och den medlem som du vill lägga till på kortet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Search for Members]**

Den här åtgärdsmodulen hämtar information om [!UICONTROL Trello] medlemmar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query] </td> 
   <td> <p>Ange det fullständiga namnet eller användarnamnet för den användare som du vill hitta.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Partial] </td> 
   <td> <p>Som standard söker den här modulen efter medlemsinnehåll efter exakta matchningar av varje ord i frågan. När [!UICONTROL Partial] är aktiverat söker modulen efter innehåll som börjar med ett ord i frågan.</p> <p> Om du t.ex. använder ordet"utveckling" för att söka efter en panel med namnet"Min utvecklingsstatusrapport", måste du som standard söka efter hela ordet. Om du har [!UICONTROL Partial] aktiverat kan du söka efter "dev" men inte "Development".</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned members]</td> 
   <td> <p> Det maximala antalet medlemmar [!DNL Workfront Fusion] returneras under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Checklistor

+++ **[!UICONTROL Create a Checklist]**

Den här åtgärdsmodulen skapar en checklista för det valda kortet.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet där du vill lägga till en checklista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>I fältet <strong>[!UICONTROL Card ID]</strong> anger eller mappar du ID:t för kortet där du vill lägga till en checklista.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet där du vill lägga till en checklista, markera sedan listan som innehåller kortet och markera sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Name] </td> 
   <td> <p>Ange eller mappa ett namn för checklistan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Position] </td> 
   <td> <p>Välj om du vill lägga till checklistan överst eller [!UICONTROL append the] checklista längst ned på kortet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Enter checklist ID]</p> </td> 
   <td> <p>Ange eller mappa ID:t för en källchecklista som du vill kopiera till den nya.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Checklist Item]**

Den här åtgärdsmodulen lägger till ett objekt i en viss checklista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter checklist ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för checklistan där du vill lägga till ett objekt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>I fältet <strong>[!UICONTROL Checklist ID]</strong> anger eller mappar du ID:t för kortet där du vill lägga till en checklista.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet där du vill lägga till en checklista, markera sedan listan som innehåller kortet, markera kortet och markera sedan checklistan.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Item name]</p> </td> 
   <td> <p>Ange eller mappa ett namn för det nya objektet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Välj om du vill lägga till objektet överst eller [!UICONTROL append] längst ned i checklistan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Checked]</p> </td> 
   <td> <p>Aktivera det här alternativet om du vill lägga till objektet som det är markerat.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Edit a Checklist Item]**

Den här åtgärdsmodulen redigerar en befintlig checklista.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a Card ID and Checklist Item ID]</td> 
   <td> <p> Välj hur du vill ange ID för kortet och checklistan där du vill redigera ett objekt.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>I fältet <strong>[!UICONTROL Checklist ID]</strong> anger eller mappar du ID:t för kortet där du vill lägga till en checklista.</p> <p>Ange eller mappa ID:t för checklistan i fältet <strong>[!UICONTROL Checklist Item ID]</strong>.</p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet där du vill lägga till en checklista, markera sedan listan som innehåller kortet, markera kortet och markera sedan checklistan.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Checklist ID]</td> 
   <td>Markera eller mappa checklistan som du vill flytta checklisteobjektet till.</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Item name]</p> </td> 
   <td> <p>Ange eller mappa ett namn för det nya objektet.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL Position]</p> </td> 
   <td> <p>Välj om du vill lägga till objektet högst upp eller längst ned i checklistan.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>[!UICONTROL State]</p> </td> 
   <td> <p>Välj om checklisteobjektet är fullständigt eller ofullständigt.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Etiketter

+++ **[!UICONTROL Add a Label to a Card]**

Den här åtgärdsmodulen lägger till en etikett till ett markerat kort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet där du vill lägga till en checklista.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>I fältet <strong>[!UICONTROL Card ID]</strong> anger eller mappar du ID:t för kortet där du vill lägga till en checklista. Ange eller mappa ID:t för etiketten som du vill lägga till i fältet <strong>[!UICONTROL Label ID]</strong>.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den bräda som innehåller kortet där du vill lägga till en checklista, markera sedan listan som innehåller kortet och markera sedan kortet. </p> <p>Markera etiketten som du vill lägga till på kortet.</p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

+++

### Kommentar

+++ **[!UICONTROL Watch Comments]**

Hämtar kommentarsinformation när det finns en ny kommentar på en angiven plats.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Watched object]</td> 
   <td> <p>Välj den plats där du vill hålla utkik efter kommentarer.</p> 
    <ul> 
     <li><strong>[!UICONTROL All cards] överallt</strong> </li> 
     <li> <p><strong>[!UICONTROL Board]</strong> </p> <p>Välj den anslagstavla som du vill bevaka för kommentarer</p> </li> 
     <li> <p><strong>[!UICONTROL List]</strong> </p> <p>Markera den anslagstavla som innehåller listan som du vill bevaka för kommentarer och markera sedan listan.</p> </li> 
     <li><strong>[!UICONTROL Card]</strong> </li> 
     <li>Markera den anslagstavla som innehåller kortet som du vill titta på för kommentarer, markera sedan listan som innehåller kortet och markera kortet.</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Limit] </td> 
   <td> <p>Det maximala antalet kommentarer som [!DNL Workfront Fusion] returnerar under en körningscykel.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL Create a Comment in a Card]**

Den här åtgärdsmodulen lägger till en kommentar på ett markerat kort.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet där du vill lägga till en kommentar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>I fältet <strong>[!UICONTROL Card ID]</strong> anger eller mappar du ID:t för kortet där du vill lägga till en kommentar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den anslagstavla som innehåller kortet där du vill lägga till en kommentar, markera sedan listan som innehåller kortet och markera sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Comment] </td> 
   <td> <p>Ange kommentaren som du vill lägga till på det markerade kortet.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

+++ **[!UICONTROL List Comments in a Card]**

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection] </td> 
   <td> <p>Instruktioner om hur du ansluter ditt [!UICONTROL Trello]-konto till [!DNL Workfront Fusion] finns i <a href="../../workfront-fusion/connections/connect-to-fusion-general.md" class="MCXref xref" data-mc-variable-override="">Skapa en anslutning till [!DNL Adobe Workfront Fusion] - grundläggande instruktioner</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Enter a card ID]</td> 
   <td> <p> Välj hur du vill ange ID:t för kortet där du vill lägga till en kommentar.</p> 
    <ul> 
     <li> <p><strong>[!UICONTROL Enter manually]</strong> </p> <p>I fältet <strong>[!UICONTROL Card ID]</strong> anger eller mappar du ID:t för kortet där du vill lägga till en kommentar.<br></p> </li> 
     <li> <p><strong>[!UICONTROL Select]</strong> </p> <p>Välj den anslagstavla som innehåller kortet där du vill lägga till en kommentar, markera sedan listan som innehåller kortet och markera sedan kortet.</p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Maximum number of returned comments]</td> 
   <td> <p> Ange det maximala antalet kommentarer som [!DNL Workfront Fusion] returnerar under en körningscykel.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Since] </td> 
   <td> <p>Ange startdatum för den period då kommentaren skapades. En lista över vilka datum- och tidsformat som stöds finns i <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Before] </td> 
   <td> <p>Ange slutdatumet för den period då kommentaren skapades. En lista över vilka datum- och tidsformat som stöds finns i <a href="../../workfront-fusion/mapping/type-coercion.md" class="MCXref xref">Typtvång i [!DNL Adobe Workfront Fusion]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## [!UICONTROL Trello] objekt-ID:n

* [Hitta ID:t eller kortlänken för ett kort i  [!DNL Trello]](#how-to-find-the-id-or-the-shortlink-of-a-card-in-trello)
* [Hitta ID:n för andra objekt i  [!DNL Trello]](#how-to-find-ids-of-other-objects-in-trello)

### Hitta ID:t eller kortlänken för ett kort i [!DNL Trello]

Om du vill redigera ett kort eller skapa en ny kommentar måste du känna till kortets ID eller dess kortlänk. Du kan hämta den här informationen från utdata för utlösaren [!UICONTROL New Card]. Du kan även få genvägen för ett kort genom att öppna kortet och klicka på knappen [!UICONTROL Share]. Kortlänken finns i rutan [!UICONTROL Link to this card], i slutet av URL:en efter `https://trello.com/c/`.

![](assets/share-and-more-350x575.png)

### Söka efter ID:n för andra objekt i [!DNL Trello]

ID:n för styrelse, lista och kommentarer kan bara hämtas med hjälp av utlösare. Dessa ID:n visas inte på webbplatsen [!DNL trello.com].
