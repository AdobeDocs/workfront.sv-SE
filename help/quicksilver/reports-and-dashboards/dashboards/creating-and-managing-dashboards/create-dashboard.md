---
product-area: dashboards
navigation-topic: create-and-manage-dashboards
title: Skapa en instrumentpanel
description: Du kan skapa kontrollpaneler för att snabbt komma åt information i Adobe Workfront. Rapporter, kalendrar och externa sidor kan läggas till på kontrollpaneler som du kan dela med andra för optimalt samarbete.
author: Nolan
feature: Reports and Dashboards
exl-id: 6a284df4-f011-4b4c-b44c-2e20918f643f
source-git-commit: 51e8faf8cc91546ccc1af551f359f81c2174c19b
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Skapa en instrumentpanel

<!--Audited: 01/2024-->

Du kan skapa kontrollpaneler för att snabbt komma åt information i Adobe Workfront. Upp till 25 rapporter, kalendrar och externa sidor kan läggas till på kontrollpaneler som du kan dela med andra för optimalt samarbete.

Mer information om instrumentpaneler finns i [Kom igång med instrumentpaneler](../../../reports-and-dashboards/dashboards/understanding-dashboards/get-started-dashboards.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande:

<table style="table-layout:auto">
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td> <p><strong>Adobe Workfront</strong></p> </td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td> <p><strong>Adobe Workfront-licens*</strong></p> </td> 
   <td> <p>Aktuell: Planera </p>
   eller
   <p>Nytt: Standard </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Åtkomstnivåkonfigurationer</strong> </td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>Du får behörigheten Hantera för de instrumentpaneler du skapar</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har. Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Du måste skapa något av följande objekt innan du kan lägga till dem på en kontrollpanel:

* **Rapporter**: Mer information om hur du skapar rapporter finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

* **Kalendrar**: Mer information om hur du skapar kalendrar finns i [Översikt över kalenderrapporter](../../../reports-and-dashboards/reports/calendars/calendar-reports-overview.md).

Du kan lägga till befintliga externa sidor på en kontrollpanel eller skapa en från den nya kontrollpanelen. Mer information om hur du skapar externa sidor finns i [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

## Skapa en instrumentpanel

{{step1-to-dashboards}}

1. Klicka på **Ny instrumentpanel**.\
   Dialogrutan Ny instrumentpanel visas.

1. Ange följande:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Namn</strong></td>
      <td><p>Det här är namnet på instrumentpanelen.</p><p>Om du inte anger något namn blir namnet på den första rapporten på kontrollpanelen som standard kontrollpanelens namn.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beskrivning (valfritt)</strong></td>
      <td>Det här är en beskrivning av instrumentpanelen.</td>
     </tr>
    </tbody>
   </table>

1. Välj en layout genom att klicka på alternativknappen som motsvarar den högst upp i avsnittet **Välj layout/Lägg till rapporter/Lägg till kalendrar**. Det är den layout som rapporter, kalendrar och externa sidor visas i på kontrollpanelen.

   Layouten med en kolumn är standard.

   Mer information om rapportlayout på kontrollpaneler finns i [Förstå hur rapporter visas på en kontrollpanel](../../../reports-and-dashboards/dashboards/understanding-dashboards/understand-how-reports-display-dashboard.md).

   <!--
   Consider adding the information from this article above here, at some point, instead of linking to it.)
   -->

1. I avsnittet **Tillgängliga rapporter och kalendrar** börjar du skriva namnet på en rapport, kalender eller extern sida i sökfältet. Dra sedan rapporten, kalendern eller den externa sidan i layoutfönstret till höger.

   >[!NOTE]
   >
   >När du söker efter ett objekt returneras de 2 000 senast skapade rapporterna. Rapportnamn som innehåller Unicode-tecken returneras inte i sökresultaten. Det är en god vana att undvika att ta med Unicode-tecken när du namnger objekt i Workfront genom att skriva namn i stället för att kopiera och klistra in namn från en annan källa.

   ![Sök efter rapporter](assets/unshimmed-dashboard-ui.png)

1. (Valfritt) Klicka på **Lägg till extern sida** om du vill lägga till en ny extern sida på instrumentpanelen.

   Mer information om hur du skapar externa sidor och bäddar in dem i kontrollpaneler finns i [Bädda in en extern webbsida i en kontrollpanel](../../../reports-and-dashboards/dashboards/creating-and-managing-dashboards/embed-external-web-page-dashboard.md).

1. Klicka på **Spara + Stäng**.

   En tidsstämpel visas i det övre högra hörnet av instrumentpanelen. Tidsstämpeln innehåller datum, tid och tidszon när instrumentpanelen senast uppdaterades.
