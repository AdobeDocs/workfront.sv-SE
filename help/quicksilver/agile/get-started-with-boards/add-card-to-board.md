---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Lägga till ett ad hoc-kort till en anslagstavla
description: Du kan snabbt lägga till ett ad hoc-kort till en styrelse och tilldela det till en styrelseledamot. Kortet kan representera en uppgift, en utgåva, en person, en grupp eller vilken typ av objekt som helst som du vill ha med i styrelsen.
author: Lisa
feature: Agile
exl-id: 9bc1f92a-85b0-44fd-b5de-09a69af6def5
source-git-commit: c1fab97289f1806676f9d80ccaa640fffa5192e5
workflow-type: tm+mt
source-wordcount: '872'
ht-degree: 0%

---

# Lägga till ett ad hoc-kort till en anslagstavla

Du kan snabbt lägga till ett kort till en anslagstavla och tilldela det till en styrelseledamot. Kortet kan representera en uppgift, en utgåva, en person, en grupp eller vilken typ av objekt som helst som du vill ha med i styrelsen.

>[!NOTE]
>
>Ad hoc-korten på en anslagstavla är inte kopplade till arbetsuppgifter i [!DNL Adobe Workfront]. Mer information om anslutna kort finns i [Använd anslutna kort på ritytor](/help/quicksilver/agile/get-started-with-boards/connected-cards.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Lägg till ett ad hoc-kort med fullständig information

Ett ad hoc-kort är inte anslutet till en arbetsuppgift i [!DNL Adobe Workfront].

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe] Workfront, klicka sedan på **[!UICONTROL Boards]**.
1. Gå till en anslagstavla. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Add card]>[!UICONTROL New card]**.
1. I **[!UICONTROL Card Details]** lägger du till följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong> </td> 
      <td>Kortets namn.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong> </td> 
      <td>En beskrivning av kortet. Du kan lägga till URL:er i beskrivningen och de blir klickbara länkar när kortet sparas.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Column]</strong> </td> 
      <td>Markera kortets kolumn. Om du lämnar <strong>[!UICONTROL Column]</strong> om fältet är tomt placeras kortet i den första kolumnen till vänster om kortet.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Status]</strong> </td> 
      <td>Välj en status för kortet. Om du klickar <strong>[!UICONTROL Mark Complete]</strong> högst upp på kortet ändras statusen automatiskt till [!UICONTROL Complete].</td> 
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Due date]</strong></td> 
      <td>Välj ett förfallodatum för kortet. </td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td> 
      <td>Ange det uppskattade antalet timmar som kortet ska fyllas i. Det här är bara ett manuellt tävlingsbidrag.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Assignees]</strong> </td> 
      <td> <p>Om du vill tilldela kortet börjar du skriva ett namn i sökfältet och markerar det sedan när det visas i listan. Du kan lägga till både enskilda personer och team, och du kan tilldela flera personer eller team till ett kort.</p> <p>Tilldelningsmedlemmar måste vara medlemmar i styrelsen, annars visas de inte i urvalslistan. När ett team är medlem i styrelsen kan de enskilda teammedlemmarna tilldelas kortet.</p></td>
     </tr>     
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td> 
      <td>Sök efter och välj taggar för kortet. Mer information om hur du skapar nya taggar finns i <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Lägg till taggar</a>.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Connection]</strong> </td>
      <td>Du kan ansluta ett ad hoc-kort till en [!DNL Workfront] aktivitet eller problem. Mer information finns i"Konvertera ett ad hoc-kort till ett anslutet kort" i artikeln <a href="/help/quicksilver/agile/get-started-with-boards/connected-cards.md">Använd anslutna kort på ritytor</a>.</td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist]</strong> </td> 
      <td> <p>Klicka på <strong>[!UICONTROL Add checklist item]</strong>. Skriv sedan objektets titel och tryck på Retur. Ett annat objekt läggs till automatiskt. Fortsätt att ange titlar för att lägga till fler objekt.</p> <p>Räknaren högst upp i checklistan visar antalet slutförda objekt och det totala antalet objekt.</p> <p>Mer information om objekt i checklistor finns i <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Hantera checklisteobjekt på kort</a>.</p> </td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>Klicka på <strong>[!UICONTROL New comment]</strong> och skriv din kommentar. Formatera texten med formateringsverktygen och klicka på <strong>Lägg till bifogad fil</strong> icon <img src="assets/attachment-icon.png" alt="Ikon för bifogad fil"> för att bifoga en fil till kommentaren. Om du vill tagga en person eller ett team använder du sökrutan längst ned i kommentarsområdet. Användaren behöver inte vara medlem i styrelsen.</p><p><strong>OBS!</strong> För närvarande får användare som är taggade i kommentarer på ad hoc-kort inget e-postmeddelande.
      </p><p>Klicka <strong>[!UICONTROL Submit]</strong> för att lägga till kommentaren på kortet.</p>
      <p><strong>OBS!</strong> Kommentarsområdet på kort använder den nya kommentarsfunktionen från Adobe Workfront. Mer information finns i <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Uppdatera arbete</a>.</p><p><strong>OBS!</strong> Kommentarer på kort är bara tillgängliga genom den tidiga funktionsavanmälningen för Workfront Boards.</p></td>
     </tr>
    </tbody> 
   </table>

   Exempelbild i produktionsmiljön när anmälan om tidiga funktioner inte används:
   ![Ad hoc-kortdetaljer](assets/boards-edit-ad-hoc-card-041723.png)

   Exempelbild i produktionsmiljön när anmälan om tidiga funktioner är aktiverad:
   ![Ad hoc-kortdetaljer](assets/ad-hoc-card-details-with-comments.png)

   Använd den vänstra navigeringspanelen för att flytta mellan fältavsnitt på kortinformationen.

1. Klicka **[!UICONTROL Close]** för att lägga till kortet i styrelsen.

   Tilldelarna, taggarna, förfallodatumet, räknaren för checklistor, beräknade timmar och status visas på kortet.

## Lägg snabbt till ett ad hoc-kort

Du kan lägga till ad hoc-kort med endast en titel för att snabbt fylla i din anslagstavla.

1. Gå till den anslagstavla som du vill lägga till kort i.
1. Klicka på **[!UICONTROL Add]** icon ![Lägg till kort](assets/addicon-spectrum.png) i kolumnen där du vill lägga till kortet.
1. Skriv kortnamnet och tryck på Retur.

   Ett annat kort läggs automatiskt till under det nya kortet.

1. Fortsätt att ange kortnamn för att lägga till fler kort.
1. Om du inte vill lägga till några kort klickar du utanför kolumnen.
1. Om du vill lägga till mer information måste du redigera kortet. Mer information finns i [Redigera ett befintligt kort](#edit-an-existing-card) i den här artikeln.

## Redigera ett befintligt kort {#edit-an-existing-card}

1. Gå till styrelsen.
1. Klicka på kortnamnet för att redigera namnet.
1. Om du vill redigera kortinformationen klickar du på kortet (inte i kortnamnet).

   eller

   Klicka på **[!UICONTROL More]** meny ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Edit]**.

1. I [!UICONTROL Card Details] , uppdatera informationen efter behov och klicka på **[!UICONTROL Close]** för att gå tillbaka till styrelsen.

   Om du har aktiverat kolumnprofiler för att uppdatera fältvärden flyttas kortet automatiskt till motsvarande kolumn om du ändrar statusen på kortet. Mer information finns i&quot;Definiera kolumninställningar och -profiler&quot; i artikeln [Hantera kortkolumner](/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md).
