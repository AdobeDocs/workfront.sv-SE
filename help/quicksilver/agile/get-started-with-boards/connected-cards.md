---
product-area: agile-and-teams
navigation-topic: get-started-with-boards
title: Använd anslutna kort på ritytor
description: Du kan lägga till ett kort på din anslagstavla som är kopplat till befintliga uppgifter och problem i Workfront.
author: Lisa
feature: Agile
exl-id: c6d979dd-e4a4-48a5-a91b-b31d7ef848d1
source-git-commit: 7d671fe66c6a23efad2e8f8f0fa3d2b7b1afcc86
workflow-type: tm+mt
source-wordcount: '0'
ht-degree: 0%

---

# Använd anslutna kort på ritytor

Du kan lägga till ett kort på din anslagstavla som är kopplat till befintliga uppgifter och problem i [!DNL Workfront].

När någon av följande uppgifter uppdateras för kortet på en plats uppdateras det automatiskt på den andra platsen:

* [!UICONTROL Name]
* [!UICONTROL Description]
* [!UICONTROL Assignees]
* [!UICONTROL Status]
* [!UICONTROL Planned completion date]
* [!UICONTROL Estimation] / [!UICONTROL Story Points]

>[!NOTE]
>En enda ansluten uppgift eller ett enstaka problem kan bara läggas till en gång per anslagstavla. Samma uppgift eller problem kan anslutas till flera anslagstavlor.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr>
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td>
   <td><p>[!UICONTROL View] eller högre tillgång till uppgifter och problem</p></td>
  </tr>
  <tr>
   <td role="rowheader"><strong>Objektbehörigheter</strong></td>
   <td><p>[!UICONTROL View] eller högre behörigheter för Workfront-uppgifter eller -utfärdande</p></td>
  </tr>
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Lägg till ett anslutet kort

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **[!UICONTROL Boards]**.
1. Gå till en anslagstavla. Mer information finns i [Skapa eller redigera en anslagstavla](../../agile/get-started-with-boards/create-edit-board.md).
1. Klicka på **[!UICONTROL Add card]>[!UICONTROL Connected card]**.
1. Välj ett projekt och välj sedan en uppgift eller ett problem som ska läggas till som ett kort på ritytan.

   Du kan markera flera objekt och de kommer att läggas till som separata kort.

   >[!NOTE]
   >
   >* Endast objekt som du har behörighet att använda är tillgängliga i sökresultatet. Om ett objekt är nedtonat har det redan lagts till på anslagstavlan.
   >* När du filtrerar efter **[!UICONTROL Projects I Own]** eller **[!UICONTROL Projects I'm On]**, inkluderas inte projekt som motsvarar en fullständig, inaktuell eller avvisad status. Du kan fortfarande söka efter dessa projekt med **[!UICONTROL All]** filter.


1. Klicka på **[!UICONTROL Add]**.

   ![Sök efter uppgift eller problem att ansluta](assets/boards-tasksissues-350x94.png)

   Kortet läggs till längst ned i kolumnen längst till vänster. Den anslutna [!DNL Workfront] objektet och dess tilldelningar visas på kortet.

   >[!NOTE]
   >
   >Om en tilldelad är på [!DNL Workfront] uppgiften eller emissionen är inte medlem i styrelsen, utan tilldelas inte kortet.

   ![Anslutet kort](assets/boards-connected-card-first-added.png)

1. Klicka ![Öppna uppgift eller ärende](assets/boards-launch-icon.png) för att öppna [!DNL Workfront] uppgifter eller problem på en ny flik i webbläsaren.
1. Om du vill redigera kortinformationen klickar du på kortet (inte i kortnamnet).

   eller

   Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) på kortet och välj **[!UICONTROL Edit]**.

1. I **[!UICONTROL Card Details]** lägg till eller uppdatera följande information:

   <table style="table-layout:auto"> 
    <tbody> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Name]</strong></td> 
      <td>Om du ändrar namnet ändras även namnet på den anslutna enheten [!DNL Workfront] -objekt.</td> 
     </tr> 
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Description]</strong></td> 
      <td>Om du ändrar beskrivningen ändras även beskrivningen på den anslutna enheten [!DNL Workfront] -objekt. Du kan lägga till URL:er i beskrivningen och de blir klickbara länkar när kortet sparas.</td> 
     </tr> 
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Assignees]</strong></td>
      <td><p>Om du vill tilldela fler personer eller ett team till kortet börjar du med att skriva ett namn i sökfältet och markerar det sedan när det visas i listan. Du kan lägga till både enskilda personer och team. Endast ett teamuppdrag tillåts på ett anslutet kort.</p>
      <p>Tilldelningsmedlemmar måste vara medlemmar i styrelsen, annars visas de inte i urvalslistan. När ett team är medlem i styrelsen kan de enskilda teammedlemmarna tilldelas kortet.</p>
      <p>Alla tilldelningar du väljer tilldelas även uppgiften eller utgåvan i [!DNL Workfront].</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Column]</strong></td>
      <td>Markera kortets kolumn.</td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Status]</strong></td>
      <td><p>Välj en status för kortet. Standardvärdena är [!UICONTROL New], [!UICONTROL In Progress]och [!UICONTROL Complete], men alla anpassade statusvärden som har definierats för objektet i [!DNL Workfront] finns också.</p>
      <p>Om du har aktiverat kolumnprofiler för att uppdatera fältvärden flyttas kortet automatiskt till motsvarande kolumn om du ändrar statusen på kortet. Mer information finns i"Definiera kolumninställningar och -profiler" i artikeln <a href="/help/quicksilver/agile/get-started-with-boards/manage-board-columns.md" class="MCXref xref">Hantera kortkolumner</a>.</p>
      <p>Om du klickar <strong>[!UICONTROL Mark Complete]</strong> högst upp på kortet ändras statusen automatiskt till Fullständigt.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Planned Completion]</strong></td>
      <td>Om du ändrar det här datumet ändras även det planerade slutförandedatumet på den anslutna [!DNL Workfront] -objekt.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>[!UICONTROL Estimation]</strong></td>
      <td><p>Antal timmar som kortet ska fyllas i.</p><p>Om du ändrar uppskattningen ändras även artikelpunktsvärdet på den anslutna [!DNL Workfront] -objekt.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>[!UICONTROL Tags]</strong></td>
      <td><p>Sök efter och välj taggar för kortet.</p>
      <p>Mer information om hur du skapar nya taggar finns i <a href="../../agile/get-started-with-boards/add-tags.md" class="MCXref xref">Lägg till taggar</a>.</p></td>
     </tr>
     <tr> 
      <td role="rowheader"><strong>[!UICONTROL Checklist Items]</strong> </td> 
      <td> <p>Klicka på <strong>[!UICONTROL Add checklist item]</strong>. Skriv sedan objektets titel och tryck på Retur. Ett annat objekt läggs till automatiskt. Fortsätt att ange titlar för att lägga till fler objekt.</p> <p>Räknaren högst upp i checklistan visar antalet slutförda objekt och det totala antalet objekt.</p> <p>Mer information om objekt i checklistor finns i <a href="/help/quicksilver/agile/get-started-with-boards/manage-checklist-items.md">Hantera checklisteobjekt på kort</a>.</p></td>
     </tr>
    </tbody> 
   </table>

   Använd navigeringspanelen till vänster för att flytta mellan fältgrupper på kortinformationen.

1. Klicka **[!UICONTROL Close]** för att gå tillbaka till styrelsen.
Det anslutna objektet, tilldelningar, taggar, förfallodatum, räknare för checklistor, beräknade timmar och status visas på kortet.

   ![Kort tillagt på kortet](assets/boards-connected-card-details-110922.png)

## Koppla från ett anslutet kort

Du kan koppla loss ett anslutet kort från Workfront-objektet och kortet finns kvar på kortet som ett särskilt kort som du kan redigera.

Så här kopplar du från på styrnivå:

1. Gå till styrelsen.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) på det anslutna kortet och välj **[!UICONTROL Disconnect]**.
1. Klicka **[!UICONTROL Disconnect]** på bekräftelsemeddelandet.

Så här kopplar du från på kortnivå:

1. Gå till kortet och öppna det anslutna kortet.
1. Klicka på **[!UICONTROL More]** meny ![Menyn Mer](assets/more-icon-spectrum.png) under Anslutning av kortinformationen och välj **[!UICONTROL Disconnect]**.
1. Klicka **[!UICONTROL Disconnect]** på bekräftelsemeddelandet.

## Konvertera ett ad hoc-kort till ett anslutet kort

När du har skapat ett ad hoc-kort kan du konvertera det till ett anslutet kort. Mer information om ad hoc-kort finns i [Lägga till ett ad hoc-kort till en anslagstavla](/help/quicksilver/agile/get-started-with-boards/add-card-to-board.md).

1. Gå till styrelsen och öppna ad hoc-kortet.
1. Kontrollera kortets namn och beskrivning. De läggs till i uppgiften eller utgåvan som du skapar i [!DNL Workfront].
1. I [!UICONTROL Connection] området med kortinformationen, klicka **[!UICONTROL Connect with Workfront]**.
1. På [!UICONTROL Connect Card] väljer du om du skapar en uppgift eller ett problem.
1. Sök efter och välj ett projekt som uppgiften eller utgåvan ska läggas till i.

   >[!NOTE]
   >
   >* Endast objekt som du har behörighet att använda är tillgängliga i sökresultatet.
   >* När du filtrerar efter **[!UICONTROL Projects I Own]** eller **[!UICONTROL Projects I'm On]**, projekt som motsvarar en [!UICONTROL Complete], [!UICONTROL Dead], eller [!UICONTROL Rejected] status inkluderas inte. Du kan fortfarande söka efter dessa projekt med **[!UICONTROL All]** filter.


1. Klicka på **[!UICONTROL Connect]**.

   ![Anslut ad hoc-kort till Workfront](assets/boards-connect-ad-hoc-card.png)

   Projektnamnet visas i området Connection på kortinformationen.

1. Klicka **[!UICONTROL Close]** för att gå tillbaka till styrelsen.

## Logga timmar på ett anslutet kort

Du måste ha rätt behörighet för att kunna logga timmar på den anslutna aktiviteten eller problemet.

Fälten för tidsloggning visas inte på anslutna kort som standard. Du måste aktivera [!UICONTROL **Timmar**] i [!UICONTROL Configure] areal under [!UICONTROL Cards]. Mer information finns i [Anpassa vilka fält som visas på ett kort](/help/quicksilver/agile/get-started-with-boards/customize-fields-on-card.md).

1. Ange antalet timmar för uppgiften eller utgåvan.
1. Välj en [!UICONTROL Hour Type] på den nedrullningsbara menyn, om den inte är standard.
1. Klicka [!UICONTROL **Loggtid**].

   ![Logga timmar på kortet](assets/log-hours-on-card.png)

   Den tid som är inloggad på kortet sparas också på den anslutna aktiviteten eller problemet.

Loggningstiden på kortet är densamma som loggningstiden för en uppgift eller ett problem. Mer information finns i&quot;Logga tid för ett projekt, en uppgift eller ett problem&quot; i artikeln [Loggtid](/help/quicksilver/timesheets/create-and-manage-timesheets/log-time.md).

