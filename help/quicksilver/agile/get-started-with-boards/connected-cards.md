---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Använd anslutna kort på kort
description: Du kan lägga till ett kort på din anslagstavla som är kopplat till befintliga uppgifter och problem i Workfront.
author: Jenny
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 6e136bed16c2b20f05267ac181dcc462b1a2aed4
workflow-type: tm+mt
source-wordcount: '1412'
ht-degree: 0%

---

# Använd anslutna kort på ritytor

<!-- Audited: 2/2024 -->

Du kan lägga till ett kort på din anslagstavla som är anslutet till befintliga uppgifter och ärenden i [!DNL Workfront].

När någon av följande uppgifter uppdateras för kortet på en plats uppdateras det automatiskt på den andra platsen:

* [!UICONTROL Name]
* [!UICONTROL Description]
* [!UICONTROL Assignees]
* [!UICONTROL Status]
* [!UICONTROL Planned completion date]
* [!UICONTROL Estimation] / [!UICONTROL Story Points]
* [!UICONTROL Subtasks]
* [!UICONTROL Documents]

Om du vill synkronisera anslutna kort med Workfront klickar du på **[!UICONTROL More]**-menyn ![[!UICONTROL More menu]](assets/more-icon-spectrum.png) bredvid kortnamnet och väljer **[!UICONTROL Sync connected items]**. Arkiverade kort synkroniseras inte med Workfront-uppgifter och -problem. Om du återställer ett kort synkroniseras det igen.

>[!NOTE]
>
>En enda ansluten uppgift eller ett enstaka problem kan bara läggas till en gång per anslagstavla. Samma uppgift eller problem kan anslutas till flera anslagstavlor.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
   <p>Medarbetare eller högre</p> 
   <p>Begäran eller senare</p>
   </td> 
  </tr> 
  <tr>
   <td role="rowheader">Konfigurationer på åtkomstnivå</td>
   <td><p>Visa eller öka åtkomsten till uppgifter och problem</p></td>
  </tr>
  <tr>
   <td role="rowheader">Objektbehörigheter</td>
   <td><p>Visa eller högre behörigheter för Workfront-aktiviteten eller -utgåvan</p>
</td>
  </tr>
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till ett anslutet kort

{{step1-to-boards}}

1. Gå till en styrelse. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Add card]>[!UICONTROL Connected card]**.
1. Välj ett projekt och välj sedan en uppgift eller ett problem som ska läggas till som ett kort på ritytan.

   Du kan markera flera objekt och de kommer att läggas till som separata kort.

   >[!NOTE]
   >
   >* Endast objekt som du har behörighet att använda är tillgängliga i sökresultatet. Om ett objekt är nedtonat har det redan lagts till på anslagstavlan.
   >* När du filtrerar efter **[!UICONTROL Projects I Own]** eller **[!UICONTROL Projects I'm On]** inkluderas inte projekt som är lika med statusen Fullständigt, Dött eller Avvisat. Du kan fortfarande söka efter dessa projekt med filtret **[!UICONTROL All]**.

1. Klicka på **[!UICONTROL Add]**.

   ![Sök efter uppgift eller problem att ansluta](assets/boards-tasksissues-350x94.png)

   Kortet läggs till längst ned i kolumnen längst till vänster. Det anslutna [!DNL Workfront]-objektet och dess tilldelningar visas på kortet.

   ![Anslutet kort](assets/boards-connected-card-first-added.png)

1. Klicka på ![Öppna aktivitet eller problem](assets/boards-launch-icon.png) för att öppna [!DNL Workfront]-aktiviteten eller problemet på en ny webbläsarflik.
1. Om du vill redigera kortinformationen klickar du på kortet (inte i kortnamnet).

   eller

   Klicka på menyn **[!UICONTROL More]** ![Mer meny](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Edit]**.

1. Lägg till eller uppdatera följande information i rutan **[!UICONTROL Card Details]**:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Om du ändrar namnet ändras även namnet på det anslutna [!DNL Workfront]-objektet.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>Om du ändrar beskrivningen ändras även beskrivningen för det anslutna [!DNL Workfront]-objektet. Du kan lägga till URL:er i beskrivningen och de blir klickbara länkar när kortet sparas.</td> 
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Markera kortets kolumn.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Välj en status för kortet. Standardvärdena är [!UICONTROL New], [!UICONTROL In Progress] och [!UICONTROL Complete], men alla anpassade statusvärden som definierats för objektet i [!DNL Workfront] är också tillgängliga.</p>
      <p>Om du har aktiverat kolumnprofiler för att uppdatera fältvärden flyttas kortet automatiskt till motsvarande kolumn om du ändrar statusen på kortet. Mer information finns i Definiera kolumninställningar och -profiler i artikeln <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Hantera panelkolumner</a>.</p>
      <p>Om du klickar på <strong>[!UICONTROL Mark Complete]</strong> högst upp på kortet ändras statusen automatiskt till Fullständig.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td>Om du ändrar det här datumet ändras även det planerade slutförandedatumet för det anslutna [!DNL Workfront]-objektet.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Antal timmar som kortet ska fyllas i.</p><p>Om du ändrar uppskattningen ändras även artikelpunktsvärdet för det anslutna [!DNL Workfront]-objektet.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignments]</strong></td>
      <td><p>Om du vill tilldela fler personer eller ett team till kortet klickar du på <strong>[!UICONTROL Add Assignment]</strong> och börjar skriva ett namn i sökfältet. Markera den sedan när den visas i resultatlistan. Du kan lägga till både enskilda personer och team. Endast ett teamuppdrag tillåts på ett anslutet kort.</p>
      <p>Alla tilldelningar du väljer tilldelas även uppgiften eller utgåvan i [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Sök efter och välj taggar för kortet.</p>
      <p>Mer information om hur du skapar nya taggar finns i <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Lägg till taggar</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Custom fields]</strong></td>
      <td><p>Alla anpassade fält som du lägger till visas i det här området.</p>
      <p>Mer information finns i <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassa vilka fält som ska visas på ett kort</a>.</p></td>
     </tr>
     <tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Subtask]</strong></td>
      <td><p>Alla befintliga underaktiviteter för aktiviteten visas i det här avsnittet. Klicka på <strong>[!UICONTROL Add Subtask]</strong> om du vill lägga till en ny underaktivitet.</p>
      <p>Räknaren högst upp i avsnittet visar antalet slutförda underaktiviteter och det totala antalet underaktiviteter.</p>
      <p>Mer information om underaktiviteter finns i <a href="/help/quicksilver/agile/get-started-with-boards/manage-subtasks-on-boards.md">Hantera underaktiviteter på ritytor</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist]</strong></td>
      <td><p>Klicka på <strong>[!UICONTROL Add checklist item]</strong>. Skriv sedan objektets titel och tryck på Retur. Ett annat objekt läggs till automatiskt. Fortsätt att ange titlar för att lägga till fler objekt.</p>
      <p>Räknaren högst upp i checklistan visar antalet slutförda objekt och det totala antalet objekt.</p> <p>Mer information om checklisteobjekt finns i <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Hantera checklisteobjekt på kort</a>.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Documents]</strong></td>
      <td>För ett befintligt dokument håller du pekaren över dokumentminiatyrbilden och klickar på <strong>Förhandsgranska</strong> för att visa filen i webbläsaren eller <strong>Hämta</strong> för att hämta filen till datorn. Information om ett nytt dokument finns i <a href="/help/quicksilver/agile/get-started-with-boards/add-documents-on-cards.md">Lägga till dokument på kort</a>.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Hours]</strong></td>
      <td>Se"Logga in timmar på ett anslutet kort" nedan.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Comments]</strong></td>
      <td><p>Klicka i fältet <strong>[!UICONTROL New comment]</strong> och skriv din kommentar. Använd formateringsverktygen för att formatera texten. Om du vill tagga en person eller ett team använder du sökrutan längst ned i kommentarsområdet. Användaren behöver inte vara medlem i styrelsen. Taggade användare på anslutna kort får e-postmeddelanden.</p><p>Klicka på <strong>[!UICONTROL Submit]</strong> för att lägga till kommentaren på kortet.</p>
      <p>Mer information om att kommentera finns i <a href="/help/quicksilver/workfront-basics/updating-work-items-and-viewing-updates/update-work.md">Uppdatera arbete</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL System activity]</strong></td> 
      <td><p>Om du har <strong>Systemaktivitet</strong> aktiverad som kortavsnitt visas aktiviteten i det här området.</p> <p>Mer information finns i <a href="/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md">Anpassa vilka fält som visas på ett kort</a> och <a href="/help/quicksilver/administration-and-setup/set-up-workfront/system-tracked-update-feeds/system-tracked-update-feeds.md">Systemspårade uppdateringar</a>.</p></td>
     </tr>     
    </tbody> 
   </table>

   Använd den vänstra navigeringspanelen för att flytta mellan fältavsnitt på kortinformationen.

1. Klicka på **[!UICONTROL Close]** för att gå tillbaka till anslagstavlan.
Det anslutna objektet, tilldelningar, taggar, förfallodatum, räknare för checklistor, beräknade timmar och status visas på kortet.

   ![Kortet har lagts till i kortet](assets/boards-connected-card-details-110922.png)

## Koppla från ett anslutet kort

Du kan koppla loss ett anslutet kort från Workfront-objektet och kortet finns kvar på kortet som ett särskilt kort som du kan redigera.

>[!NOTE]
>
>Om du kopplar från ett anslutet kort på ett dynamiskt kort visas det igen när du uppdaterar kortet, eftersom den här typen av kort hämtar alla uppgifter och problem från ett visst projekt.
>
>Om du kopplar från ett anslutet kort från någon annan typ av kort som har en inloppskolonn, kommer kortet att visas igen i inmatningskolumnen när du uppdaterar kortet om den anslutna aktiviteten eller utdraget ännu inte har markerats som slutfört.
>
>I båda dessa scenarier kommer du efter en uppdatering att ha två kort för samma uppgift eller utgåva: ett ad hoc-kort och ett anslutet kort.

Så här kopplar du från ett kort på styrelsenivå:

1. Gå till styrelsen.
1. Klicka på menyn **[!UICONTROL More]** ![Mer meny](assets/more-icon-spectrum.png) på det anslutna kortet och välj **[!UICONTROL Disconnect]**.
1. Klicka på **[!UICONTROL Disconnect]** i bekräftelsemeddelandet.

Så här kopplar du från ett kort på kortnivå:

1. Gå till kortet och öppna det anslutna kortet.
1. Klicka på menyn **[!UICONTROL More]** ![Mer meny](assets/more-icon-spectrum.png) i området Anslutning för kortinformationen och välj **[!UICONTROL Disconnect]**.
1. Klicka på **[!UICONTROL Disconnect]** i bekräftelsemeddelandet.

## Konvertera ett särskilt kort till ett anslutet kort

När du har skapat ett ad hoc-kort kan du konvertera det till ett anslutet kort. Mer information om ad hoc-kort finns i [Lägga till ett ad hoc-kort till en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Gå till styrelsen och öppna ad hoc-kortet.
1. Kontrollera kortets namn och beskrivning. De läggs till i uppgiften eller utgåvan som du skapar i [!DNL Workfront].
1. Klicka på [!UICONTROL Connection] i området **[!UICONTROL Connect with Workfront]** i kortinformationen.
1. I fönstret [!UICONTROL Connect Card] väljer du om du skapar en uppgift eller ett problem.
1. Sök efter och välj ett projekt som uppgiften eller utgåvan ska läggas till i.

   >[!NOTE]
   >
   >* Endast objekt som du har behörighet att använda är tillgängliga i sökresultatet.
   >* När du filtrerar efter **[!UICONTROL Projects I Own]** eller **[!UICONTROL Projects I'm On]** inkluderas inte projekt som motsvarar en [!UICONTROL Complete]-, [!UICONTROL Dead]- eller [!UICONTROL Rejected]-status. Du kan fortfarande söka efter dessa projekt med filtret **[!UICONTROL All]**.

1. Klicka på **[!UICONTROL Connect]**.

   ![Ansluta ad hoc-kort till Workfront](assets/boards-connect-ad-hoc-card.png)

   Projektnamnet visas i området Connection på kortinformationen.

1. Klicka på **[!UICONTROL Close]** för att gå tillbaka till anslagstavlan.

## Logga timmar på ett anslutet kort

Du måste ha rätt behörighet för att kunna logga timmar på den anslutna aktiviteten eller problemet.

Fälten för tidsloggning visas inte på anslutna kort som standard. Du måste aktivera [!UICONTROL **Timmar**] i området [!UICONTROL Configure] under [!UICONTROL Cards]. Mer information finns i [Anpassa vilka fält som ska visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Ange antalet timmar för uppgiften eller utgåvan.
1. Välj en [!UICONTROL Hour Type] på den nedrullningsbara menyn, om den inte är standard.
1. Klicka på [!UICONTROL **Loggtid**].

   ![Logga in timmar på kortet](assets/log-hours-on-card.png)

   Den tid som är inloggad på kortet sparas också på den anslutna aktiviteten eller problemet.

Loggningstiden på kortet är densamma som loggningstiden för en uppgift eller ett problem. Mer information finns i&quot;Logga tid för ett projekt, en uppgift eller ett problem&quot; i artikeln [Loggtid](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

