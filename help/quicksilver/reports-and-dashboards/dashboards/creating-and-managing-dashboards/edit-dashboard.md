---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Redigera en kontrollpanel
description: Syftet med kontrollpanelen är att ge snabb åtkomst till information. Du kan fylla en kontrollpanel med rapporter, kalendrar och externa sidor.
author: Nolan
feature: Reports and Dashboards
exl-id: de15ab45-4bcd-4638-b3d7-fc70a0866d2d
source-git-commit: 811eb1453c140808b0d6c5d9a3b4a0729cb16b2d
workflow-type: tm+mt
source-wordcount: '552'
ht-degree: 0%

---

# Redigera en kontrollpanel

Syftet med kontrollpanelen är att ge snabb åtkomst till information. Du kan fylla en kontrollpanel med följande objekt i Adobe Workfront:

* Rapporter

  Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Kalendrar

  Mer information om hur du skapar kalendrar finns i [Kalendrar: artikelindex](../../../reports-and-dashboards/reports/calendars/calendars.md).

* Externa sidor

  Mer information om hur du skapar externa sidor finns i [Bädda in en extern webbsida i en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

När du har skapat de här objekten och lagt till dem på en kontrollpanel kan du redigera kontrollpanelen för att lägga till fler objekt i den, ta bort befintliga objekt från den eller redigera instrumentpanelsinformationen.

Ändringar som görs i en kontrollpanel påverkar alla användare som har tillgång till den kontrollpanelen.

När du delar en kontrollpanel med användare delas även alla rapporter, kalendrar och externa sidor med samma användare.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-plan*</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens*</strong></td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå*</strong></td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter på kontrollpanelen</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste skapa en kontrollpanel innan du kan redigera den.

Mer information om hur du skapar kontrollpaneler finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Redigera en kontrollpanel

1. Gå till den instrumentpanel som du vill redigera.
1. Klicka **Instrumentpanelsåtgärder** och sedan klicka **Redigera**.

   ![](assets/qs-dashboard-actions-menu-350x318.png)

   >[!TIP]
   >
   >Mer information om hur du tar bort en kontrollpanel finns i [Ta bort en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/delete-dashboard.md).

1. Överväg att redigera följande fält:

   * **Namn**: Redigera namnet på kontrollpanelen.
   * **Beskrivning**: Ange en beskrivning för instrumentpanelen.

1. I **Tillgängliga rapporter och kalendrar** börjar du skriva namnet på en rapport, kalender eller extern sida i **Sök efter namn eller typ..** och sedan dra och släppa rapporten eller kalendern i layoutfönstret till höger.

   >[!NOTE]
   >
   >När du söker efter ett objekt returneras de 2 000 senast skapade rapporterna. Rapportnamn som innehåller Unicode-tecken returneras inte i sökresultaten. Det är en god vana att undvika att ta med Unicode-tecken när du namnger objekt i Workfront genom att skriva namn i stället för att kopiera och klistra in namn från en annan källa.

1. (Valfritt) Välj en ny layout för kontrollpanelen genom att klicka på en alternativknapp som motsvarar den layout du vill använda.
1. (Valfritt) För muspekaren över namnet på en befintlig rapport och klicka på papperskorgsikonen för att ta bort den från kontrollpanelen.
1. (Valfritt) Ändra ordningen på rapporterna på kontrollpanelen genom att klicka på namnet på en rapport, dra den och släppa den på önskad plats i layoutfönstret.
1. (Valfritt) Klicka på **Lägg till extern sida** om du vill lägga till en extern sida på kontrollpanelen.\
   eller\
   Leta reda på en befintlig extern sida på kontrollpanelen, för muspekaren över den och klicka på **Redigera** om du vill redigera den externa sidan.\
   Mer information om hur du lägger till eller redigerar externa sidor på en kontrollpanel finns i [Bädda in en extern webbsida i en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Klicka **Spara + Stäng**.
