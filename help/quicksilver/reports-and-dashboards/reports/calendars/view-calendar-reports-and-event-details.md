---
product-area: calendars
navigation-topic: calendars-navigation-topic
title: Visa kalenderrapporter och händelseinformation
description: Du kan visa kalenderrapporter och händelseinformation som du har skapat eller som delats med dig i Adobe Workfront.
author: Lisa
feature: Reports and Dashboards
exl-id: db016e91-43e4-400c-ac9d-1639c7f94479
source-git-commit: e5a3024b1657942cd7abdfff76a7a6795127a4f5
workflow-type: tm+mt
source-wordcount: '676'
ht-degree: 0%

---

# Visa kalenderrapporter och händelseinformation

Du kan visa kalenderrapporter och händelseinformation som du har skapat eller som delats med dig i Adobe Workfront.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront plan*]</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>[!DNL Adobe Workfront] licens*</strong></td> 
   <td> <p>[!UICONTROL Request] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till [!UICONTROL Reports], [!UICONTROL Dashboards]och [!UICONTROL Calendars]</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>[!UICONTROL View] eller högre behörighet till kalenderrapporten</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Visa en kalenderrapport

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront]och sedan klicka **[!UICONTROL Calendars]**.

   Beroende på din åtkomstnivå kan följande kalendrar visas:

   * Din standard [!DNL Adobe Workfront] kalender\

      Workfront skapar en kalender för dig baserat på de projekt, uppgifter och utgåvor som har tilldelats dig eller som har tilldelats team, grupper eller roller som du har tilldelats.
   * Kalendrar som du har skapat\

      Mer information om hur du skapar kalendrar finns i [Översikt över kalenderrapporter](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

   * Kalendrar som andra användare har delat med dig\

      Mer information om att dela kalendrar finns i [[!UICONTROL Share a calendar] rapport](../../../reports-and-dashboards/reports/calendars/share-a-calendar-report.md).

1. (Villkorligt) Klicka på **[!UICONTROL View]** och välj sedan den kalendervaraktighet som du vill visa.\
   ![Kalenderns varaktighet](assets/view-menu-calendar-report-350x189.png)\
   Du kan välja bland följande kalenderrapportvyer:

   * **[!UICONTROL Month]**: Visar fyra veckor i kalendern
   * **[!UICONTROL Week]**: Visar en vecka i kalendern
   * **[!UICONTROL Gantt]**: Visar en kontinuerlig vy av kalendern\

      ![[!UICONTROL Gantt] kalenderrapport](assets/gantt-calendar-report.png)
Du kan se fler händelser i en [!UICONTROL Gantt] genom att rulla nedåt eller åt sidan. En inläsningssymbol visas när data fylls i för vyn.
   >[!NOTE]
   >
   >I [!UICONTROL Month] och [!UICONTROL Week] vyer, händelser som är aktuella eller framtida (inklusive händelser som sträcker sig över flera dagar, så länge de innehåller idag eller en framtida dag) har skuggning som motsvarar färgen i projekt- eller kalendergrupperingen. Tidigare händelser har ljusare skuggning för att ange att de inte längre är aktuella, men du kan ändå markera och visa dessa händelser.

1. (Valfritt) Om du visar kalendern i [!UICONTROL Month] eller [!UICONTROL Week] kan du ändra kalendervyn med följande alternativ:

   * Så här inkluderar eller exkluderar du helger:

      1. På **[!UICONTROL Calendar]** verktygsfält, klicka **[!UICONTROL Calendar Actions]** väljer du sedan i listrutan antingen **[!UICONTROL Show Weekend]** eller **[!UICONTROL Hide Weekend]**.
   * Så här ändrar du snabbt de visade datumen:

      1. På **[!UICONTROL Calendar]** klickar du på vänsterpilen i datumindikatorn för att gå tillbaka i kalendern eller högerpilen för att gå framåt.\

         ![Klicka på pilen för att ändra datumet](assets/click-arrows-to-change-dates-calendar-report.png)\
         De visade datumen justeras med ett intervall baserat på den aktuella kalendervyn. Om du till exempel visar kalendern i [!UICONTROL Week] kalendern visas antingen en vecka framåt eller en vecka bakåt, beroende på vilken pil du väljer.

      1. (Valfritt) Om du vill återgå till den aktuella dagen klickar du på **Today**.


1. (Valfritt) Om du vill visa en kalender i helskärmsläge klickar du på helskärmspilarna till höger på sidan **[!UICONTROL Calendar]** verktygsfält.
   ![Klicka på pilen för att ändra datumet](assets/click-arrows-to-change-dates-calendar-report.png)\
   Tryck på Esc för att återgå till den normala vyn av kalendern.

1. (Valfritt) Om du vill dölja händelserna för ett projekt eller en kalendergrupp som är länkad till kalendern, avmarkerar du projektet eller kalendergruppen i projektlistan.
   ![Dölj händelser](assets/hide-events-for-project-or-cal-grouping.png)\
   Du kan göra händelserna synliga igen genom att välja [!UICONTROL project] eller kalendergruppering i projektlistan.

## Visa händelseinformation för kalenderrapport

Du kan se information om en händelse i en kalender, både för aktuella och tidigare händelser.

1. Gå till händelsen som du vill veta informationen om och klicka sedan på händelsen.\
   En informationssida för händelsen öppnas.\
   ![calendar_report_EventDetails.png](assets/calendar-report-eventdetails-350x145.png)

1. (Valfritt) Om du vill visa mer information om objektet:

   1. Håll muspekaren över namnet på projektet, aktiviteten eller utgåvan.

      En informationssida öppnas för objektet.\
      ![additional_object_details_-_calendar_report.png](assets/additional-object-details---calendar-report-350x131.png)

   1. (Valfritt) Om du vill öppna det associerade projektet, aktiviteten eller utgåvan klickar du på objektets titel.
   1. (Valfritt) Om du vill stänga alla öppna informationssidor klickar du var som helst utanför sidan med händelseinformation.
