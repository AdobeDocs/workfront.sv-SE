---
content-type: reference
product-previous: workfront-fusion
product-area: workfront-integrations
keywords: koppling
navigation-topic: apps-and-their-modules
title: Adobe Workfront Boards-moduler
description: Du kan använda Adobe Workfront Boards-kontakten för att automatisera processerna i Workfront Boards och koppla dem till program och tjänster från tredje part.
author: Becky
feature: Workfront Fusion, Workfront Integrations and Apps
source-git-commit: 074bcf15c61f9c0c75cebf774b15baf7fe383f35
workflow-type: tm+mt
source-wordcount: '1958'
ht-degree: 0%

---

# [!DNL Adobe Workfront] Styrelsemoduler

>[!NOTE]
>
>Den här kopplingen är för närvarande i Beta.

Adobe Workfront Boards är flexibla verktyg som ger teamsamarbete genom att ge åtkomst till en delad anslagstavla som innehåller kolumner och kort.

Du kan använda modulen Adobe Workfront Boards för att läsa eller uppdatera poster, göra ett API-anrop till Workfront Boards API eller utlösa ett scenario när en åtgärd utförs på en anslagstavla.

Allmän information om Workfront Boards finns på [Översikt över styrelser](/help/quicksilver/agile/boards-overview.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna använda funktionerna i den här artikeln:

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td>
  <td> <p>Alla</p> </td>
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td>
   <td> <p>Nytt: Standard</p><p>eller</p><p>Aktuell: [!UICONTROL Plan], [!UICONTROL Work]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront Fusion] licens</td> 
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
   <p>Krav för äldre produkter: Din organisation måste köpa [!DNL Adobe Workfront Fusion] och [!DNL Adobe Workfront] om du vill använda de funktioner som beskrivs i den här artikeln.</p>
   </td> 
  </tr> 
 </tbody> 
</table>

Mer information om tabellen finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

För information om [!DNL Adobe Workfront Fusion] licenser, se [[!DNL Adobe Workfront Fusion] licenser](../../workfront-fusion/get-started/license-automation-vs-integration.md).
Adobe Workfront Books-moduler och deras fält

## Förutsättningar

Du måste ha konfigurerat en anslagstavla i Adobe Workfront innan du kan ansluta till den.

## Skapa en anslutning till Workfront Boards

>[!NOTE]
>
>Du kan använda en Workfront-anslutning för att ansluta till Workfront Boards eller skapa en separat anslutning till Workfront Boards.

Så här skapar du en anslutning till Workfront Boards:

1. I alla [!DNL Adobe Workfront Boards] modul, klicka på **[!UICONTROL Add]** bredvid rutan Anslutning.

1. Fyll i följande fält:

   <table style="table-layout:auto"> 
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column1">
      </col>
      <col class="TableStyle-TableStyle-List-options-in-steps-Column-Column2">
      </col>
      <tbody>
        <tr>
          <td role="rowheader">[!UICONTROL Connection name]</td>
          <td>
            <p>Ange ett namn för anslutningen.</p>
          </td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Environment]</td>
          <td>Ange om du ansluter till en produktionsmiljö eller icke-produktionsmiljö.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Type]</td>
          <td>Välj om du vill ansluta till ett tjänstkonto eller ett personligt konto.</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client ID]<p>(Valfritt)</p></td>
          <td>Ange [!DNL Adobe] [!UICONTROL Client ID]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].</td>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Client Secret]<p>(Valfritt)</p></td>
          <td>Ange [!DNL Adobe] [!UICONTROL Client Secret]. Detta finns i [!UICONTROL Credentials details] i [!DNL Adobe Developer Console].
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Authentication URL]<p>(Valfritt)</p></td>
          <td>Ange den URL som din instans av Workfront ska använda för att autentisera anslutningen. <p>Standardvärdet är <code>https://oauth.my.workfront.com/integrations/oauth2</code>.</p>
        </tr>
        <tr>
          <td role="rowheader">[!UICONTROL Host prefix]</td>
          <td>Ange värdprefixet.<p>Standardvärdet är <code>origin-</code>.</p>
        </tr>
      </tbody>
    </table>
1. Klicka **[!UICONTROL Continue]** för att spara anslutningen och återgå till modulen.

## Adobe Workfront Books-moduler och deras fält

När du konfigurerar Workfront Boards-moduler [!DNL Workfront Fusion] visar fälten som listas nedan. Dessutom kan ytterligare fält för Workfront Boards visas, beroende på faktorer som din åtkomstnivå i appen eller tjänsten. En rubrik med fet stil i en modul visar ett obligatoriskt fält.

Om du ser kartknappen ovanför ett fält eller en funktion kan du använda den för att ange variabler och funktioner för det fältet. Mer information finns i [Mappa information från en modul till en annan i [!DNL Adobe Workfront Fusion]](../../workfront-fusion/mapping/map-information-between-modules.md).

![](assets/map-toggle-350x74.png)

* [Kort](#cards)
* [Varumärkena](#boards)
* [Kolumner](#columns)
* [Taggar](#tags)
* [Övriga](#other)

<!--

### Watch

#### Watch events

This trigger module starts a scenario when an event occurs on a board.

1. Click **[!UICONTROL Add]** to the right of the **Webhook** box.

1. Configure the webhook in the **[!UICONTROL Add a hook]** box that displays.

   When you are configuring this module, the following fields display.

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td>[!UICONTROL Webhook name]</td> 
      <td>(Optional) Type a new name for the webhook</td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Connection]</td> 
      <td> <p>You can use an existing Workfront connection to connect to Workfront Boards, or you can use a specific Workfront Boards connection. </p><p>For instructions about connecting your [!DNL Workfront] app to [!DNL Workfront Fusion], see <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Create a connection to Workfront Boards</a> in this article.</p> </td> 
     </tr> 
     <tr> 
      <td>[!UICONTROL Object type]</td> 
      <td>Select the type of [!DNL Workfront] object that you want the module to watch.</td> 
     </tr> 
     <tr> 
      <td> <p>[!UICONTROL Objects to watch]</p> </td> 
      <td> Select whether you want to trigger a scenario when there is a new object, an updated object, a new or updated object, or a deleted object. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td>Exclude events made by this connection</td> 
      <td>Enable this option to exclude events created or updated using the same connector that this trigger module uses. This can prevent situations where a scenario might trigger itself, causing it to repeat in an endless loop.</td> 
     </tr> 
    </tbody> 
   </table>

After the webhook is created, you can view the address of the endpoint that events are sent to.

-->

### Kort

* [Lägg till checklisteobjekt](#add-checklist-item)
* [Lägg till underaktivitet](#add-subtask)
* [Skapa ett kort](#create-a-card)
* [Flytta ett kort](#move-a-card)
* [Läs ett kort](#read-a-card)
* [Uppdatera ett kort](#update-a-card)

#### Lägg till checklisteobjekt

Den här åtgärdsmodulen lägger till ett checklisteobjekt på det angivna kortet.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Ange eller mappa ID:t för kortet som du vill lägga till ett checklisteobjekt i.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Checklist items]</td> 
   <td>För varje objekt i checklistan som du vill lägga till klickar du på Lägg till objekt, anger namnet på objektet i checklistan och väljer om objektet har slutförts.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Lägg till underaktivitet

Den här åtgärdsmodulen lägger till en underaktivitet till ett kort i Boards. Kortet måste vara ett anslutet kort. Underaktiviteten läggs också till i den Workfront-uppgift som kortet representerar.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Parent card ID]</td> 
   <td>Ange eller mappa ID:t för kortet som du vill lägga till en underaktivitet i.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den bräda som innehåller kortet som du vill lägga till en underaktivitet i.<p>Du kan hitta ID:t för anslagstavlan i URL:en när du tittar på anslagstavlan i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Ange eller mappa ett namn för den nya underaktiviteten.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Skapa ett kort

Den här åtgärdsmodulen skapar ett nytt kort på ett Workfront-kort.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den anslagstavla som du vill lägga till ett kort till.<p>Du kan hitta ID:t för anslagstavlan i URL:en när du tittar på anslagstavlan i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column ID]</td> 
   <td>Ange eller mappa ID:t för den kolumn som du vill lägga till en underaktivitet i.<p>Du hittar tagg-ID:t i informationen som returneras från modulen Läs en anslagstavla.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Ange eller mappa ett namn för det nya kortet.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Flytta ett kort

Den här åtgärdsmodulen flyttar ett kort till en annan kolumn på samma kort.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Ange eller mappa ID:t för kortet som du vill flytta.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den bräda som innehåller kortet som du vill flytta.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Destination column ID]</td> 
   <td>Ange eller mappa ID:t för kolumnen som du vill flytta kortet till.<p>Du hittar tagg-ID:t i informationen som returneras från modulen Läs en anslagstavla.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL To index]</td> 
   <td>Ange eller mappa positionen som du vill att kortet ska ha i den nya kolumnen.<p>Den översta positionen i kolumnen i index 0.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Läs ett kort

Den här åtgärdsmodulen hämtar information om ett specifikt kort.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Ange eller mappa ID:t för kortet som du vill läsa.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Uppdatera ett kort

Den här åtgärdsmodulen uppdaterar information för ett kort som du anger.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Ange eller mappa ID:t för kortet som du vill uppdatera.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den anslagstavla som innehåller kortet som du vill uppdatera.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Name]</td> 
   <td>Ange eller mappa ett nytt namn för kortet.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Ange eller mappa en ny beskrivning för kortet/\.</p></td> 
  </tr> 
 </tbody> 
</table>

### Varumärkena

* [Skapa en anslagstavla](#create-a-board)
* [Läs en anslagstavla](#read-a-board)

#### Skapa en anslagstavla

Den här åtgärdsmodulen skapar en styrelse i Workfront. Du kan ange vilken typ av anslagstavla du vill skapa.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board name]</td> 
   <td>Ange eller mappa ett namn för den nya ritytan.</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Type]</td> 
   <td>Välj den typ av anslagstavla du vill skapa.</td> 
  </tr> 
 </tbody> 
</table>

#### Läs en anslagstavla

Den här åtgärdsmodulen returnerar information om en enda anslagstavla, till exempel kort, kolumner, taggar och medlemmar.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den anslagstavla som du vill hämta information för.<p>Du kan hitta ID:t för anslagstavlan i URL:en när du tittar på anslagstavlan i Workfront.</p></td> 
  </tr> 
 </tbody> 
</table>

### Kolumner

#### Skapa en kolumn

Den här åtgärdsmodulen skapar en ny kolumn på den angivna ritytan.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den anslagstavla som du vill lägga till en kolumn i.<p>Du kan hitta ID:t för anslagstavlan i URL:en när du tittar på anslagstavlan i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Column name]</td> 
   <td>Ange eller mappa ett namn för den nya kolumnen.</td> 
  </tr> 
 </tbody> 
</table>

### Taggar

* [Lägga till en tagg på ett kort](#add-card-tag)
* [Skapa en tagg](#create-a-tag)

#### Lägga till en tagg på ett kort

Den här åtgärdsmodulen lägger till en tagg på ett kort.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Card ID]</td> 
   <td>Ange eller mappa ID:t för kortet som du vill lägga till en tagg i.<p>Kortets ID finns i URL:en när du visar kortet i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den bräda som innehåller kortet som du vill lägga till en tagg i.<p>Du kan hitta ID:t för anslagstavlan i URL:en när du tittar på anslagstavlan i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag ID]</td> 
   <td>Ange eller mappa ID:t för taggen som du vill lägga till.<p>Du hittar tagg-ID:t i informationen som returneras från modulen Läs en anslagstavla.</p></td> 
  </tr> 
 </tbody> 
</table>

#### Skapa en tagg

Den här åtgärdsmodulen skapar en ny tagg och tilldelar den en färg.

<table style="table-layout:auto">
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Board ID]</td> 
   <td>Ange eller mappa ID:t för den anslagstavla som du vill skapa en tagg för.<p>Du kan hitta ID:t för anslagstavlan i URL:en när du tittar på anslagstavlan i Workfront.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag name]</td> 
   <td>Ange eller mappa ett namn för den nya taggen.</p></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Tag Color]</td> 
   <td>Välj färg för den här taggen.</td> 
  </tr> 
 </tbody> 
</table>

### Övriga

#### Göra ett anpassat API-anrop

Den här åtgärdsmodulen gör ett anpassat anrop till Workfront Boards API.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Connection]</td> 
      <td> <p>Du kan använda en befintlig Workfront-anslutning för att ansluta till Workfront Boards eller använda en viss Workfront Boards-anslutning. </p><p>Instruktioner om hur du ansluter [!DNL Workfront] app till [!DNL Workfront Fusion], se <a href="#create-a-connection-to-workfront-boards" class="MCXref xref">Skapa en anslutning till Workfront Boards</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">URL</td> 
   <td> <p>Ange en sökväg i förhållande till<code> https://&lt;WORKFRONT_DOMAIN&gt;/boards-service/graphql?</code>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Method]</td> 
   <td> <p>Välj den HTTP-förfrågningsmetod som du behöver för att konfigurera API-anropet. Mer information finns i <a href="../../workfront-fusion/modules/http-request-methods.md" class="MCXref xref" data-mc-variable-override="">HTTP-förfrågningsmetoder i [!DNL Adobe Workfront Fusion]</a>.</p><p>För de flesta ritytor är metoden POST. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Headers]</td> 
   <td> <p>Lägg till rubrikerna för begäran i form av ett standard-JSON-objekt. Detta avgör begärans innehållstyp.</p> <p>Exempel:<code> { "Content-type":"application/json-stringify()"}</code></p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Query String]</td> 
   <td> <p>Lägg till frågan för API-anropet i form av ett standard-JSON-objekt.</p> <p>För Workfront Boards är det här avsnittet vanligtvis tomt.</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Body]</td> 
   <td> <p>Lägg till brödinnehållet för API-anropet i form av en JSON-inbäddad Graphql </p> <p>Exempel:</p><p>I det här exemplet uppdateras ett kolumnnamn. Du kan inkludera <code>boardId</code> och <code>columnId</code> som GUID antingen hårdkodade eller mappade från en tidigare modul.<p><pre>{

  &quot;query&quot;: &quot;mutation { updateColumn(boardId: \&quot;\&quot;, columnId: \&quot;\&quot;, updateColumnInput: { name: \&quot;\&quot; }) { id name }}&quot;

}</pre><p>Obs!  <p>När du använder villkorssatser som <code>if</code> i JSON placerar citattecknen utanför villkorssatsen.</p>
<div class="example" data-mc-autonum="<b>Example: </b>">
<p> <img src="assets/quotes-in-json-350x120.png" style="width: 350;height: 120;"> </p>
</div> </p> </td>
</tr> 
 </tbody> 
</table>
