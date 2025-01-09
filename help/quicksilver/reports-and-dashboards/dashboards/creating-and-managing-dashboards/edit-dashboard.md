---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Redigera en kontrollpanel
description: Syftet med kontrollpanelen är att ge snabb åtkomst till information. Du kan fylla en kontrollpanel med rapporter, kalendrar och externa sidor.
author: Nolan
feature: Reports and Dashboards
exl-id: de15ab45-4bcd-4638-b3d7-fc70a0866d2d
source-git-commit: a9abbeaa9abd0e905c60000a218eddb85d0389b9
workflow-type: tm+mt
source-wordcount: '495'
ht-degree: 0%

---

# Redigera en kontrollpanel

<!-- Audited: 1/2025 -->

Syftet med kontrollpanelen är att ge snabb åtkomst till information. Du kan fylla en kontrollpanel med följande objekt i Adobe Workfront:

* Rapporter

  Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* Externa sidor

  Mer information om hur du skapar externa sidor finns i [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

När du har skapat de här objekten och lagt till dem på en kontrollpanel kan du redigera kontrollpanelen för att lägga till fler objekt i den, ta bort befintliga objekt från den eller redigera instrumentpanelsinformationen.

Ändringar som görs i en kontrollpanel påverkar alla användare som har tillgång till den kontrollpanelen.

När du delar en kontrollpanel med användare delas även alla rapporter och externa sidor med samma användare.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront</strong></td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Adobe Workfront-licens</strong></td> 
   <td> 
      <p>Nytt:</p>
         <ul>
         <li><p>Standard</p></li>
         </ul>
      <p>Aktuell:</p>
         <ul>
         <li><p>Plan</p></li>
         </ul>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Konfigurationer på åtkomstnivå</strong></td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader"><strong>Objektbehörigheter</strong></td> 
   <td> <p>Hantera behörigheter på kontrollpanelen</p></td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste skapa en kontrollpanel innan du kan redigera den.

Mer information om hur du skapar instrumentpaneler finns i [Skapa en instrumentpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/create-dashboard.md).

## Redigera en kontrollpanel

1. Gå till den instrumentpanel som du vill redigera.
1. Klicka på **Instrumentpanelsåtgärder** och sedan på **Redigera**.

   ![](assets/unshimmed-edit-dashboard.png)

   >[!TIP]
   >
   >Mer information om hur du tar bort en kontrollpanel finns i [Ta bort en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/delete-dashboard.md).

1. Överväg att redigera följande fält:

   * **Namn**: Redigera namnet på instrumentpanelen.
   * **Beskrivning**: Ange en beskrivning för instrumentpanelen.

1. I avsnittet **Tillgängliga rapporter och kalendrar** börjar du skriva namnet på en rapport, kalender eller extern sida i sökfältet. Dra sedan rapporten, kalendern eller den externa sidan i layoutfönstret till höger.

   >[!NOTE]
   >
   >När du söker efter ett objekt returneras de 2 000 senast skapade rapporterna. Rapportnamn som innehåller Unicode-tecken returneras inte i sökresultaten. Det är en god vana att undvika att ta med Unicode-tecken när du namnger objekt i Workfront genom att skriva namn i stället för att kopiera och klistra in namn från en annan källa.

1. (Valfritt) Välj en ny layout för kontrollpanelen genom att klicka på en alternativknapp som motsvarar den layout du vill använda.
1. (Valfritt) För muspekaren över namnet på en befintlig rapport och klicka på papperskorgsikonen för att ta bort den från kontrollpanelen.
1. (Valfritt) Ändra ordningen på rapporterna på kontrollpanelen genom att klicka på namnet på en rapport, dra den och släppa den på önskad plats i layoutfönstret.
1. (Valfritt) Klicka på **Lägg till extern sida** om du vill lägga till en extern sida på instrumentpanelen.\
   eller\
   Leta reda på en befintlig extern sida i kontrollpanelen, peka på den och klicka på ikonen **Redigera** för att redigera den externa sidan.\
   Mer information om hur du lägger till eller redigerar externa sidor i en kontrollpanel finns i [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Klicka på **Spara + Stäng**.
