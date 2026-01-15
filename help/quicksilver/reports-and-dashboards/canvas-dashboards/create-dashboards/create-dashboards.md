---
product-area: Canvas Dashboards
navigation-topic: report-types
title: Skapa en arbetsytans kontrollpanel
description: Med Canvas Dashboards kan du skapa och lägga till rapporter på en anpassningsbar kontrollpanel för att snabbt visualisera dina kontodata.
author: Courtney and Jenny
feature: Reports and Dashboards
exl-id: bd31e426-7c4a-4ff8-9432-c95dc8ee3743
source-git-commit: 507cb64eb21c2798cdafe184794c0d9ed7ebc0c6
workflow-type: tm+mt
source-wordcount: '480'
ht-degree: 0%

---

# Skapa en arbetsytans kontrollpanel

>[!IMPORTANT]
>
>Funktionen Canvas Dashboards är för närvarande bara tillgänglig för användare som deltar i betatestet. Delar av funktionen kanske inte är fullständiga eller fungerar som de ska i det här skedet. Skicka feedback om din upplevelse genom att följa instruktionerna i avsnittet [Ge feedback](/help/quicksilver/product-announcements/betas/canvas-dashboards-beta/canvas-dashboards-beta-information.md#provide-feedback) i översiktsartikeln i Canvas Dashboards.<br>
>Om du har synpunkter på ett eventuellt fel eller tekniska problem ber vi dig skicka ett supportärende till Workfront Support. Mer information finns i [Kontakta kundsupport](/help/quicksilver/workfront-basics/tips-tricks-and-troubleshooting/contact-customer-support.md).<br>
>Observera att betaversionen inte är tillgänglig för följande molnleverantörer:
>
>* Använd din egen nyckel för Amazon Web Services
>* Azure
>* Google Cloud Platform

Med Canvas Dashboards kan du skapa och lägga till rapporter på en anpassningsbar kontrollpanel för att snabbt visualisera dina kontodata.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
<col> 
</col> 
<col> 
</col> 
<tbody> 
<tr> 
   <td role="rowheader"><p>Adobe Workfront package</p></td> 
   <td> 
<p>Alla </p> 
   </td> 
<tr> 
 <tr> 
   <td role="rowheader"><p>Adobe Workfront-licens</p></td> 
   <td> 
<p>Standard </p> 
<p>Plan</p> 
   </td> 
   </tr> 
  </tr> 
  <tr> 
   <td role="rowheader"><p>Konfigurationer på åtkomstnivå</p></td> 
   <td><p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p>
  </td> 
  </tr>  
</tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
+++

## Förutsättningar

Kontrollpaneler på arbetsytan måste vara aktiverade i layoutmallskonfigurationen för vänsternavigeringsobjekt på sidan Kontrollpaneler.

## Skapa en instrumentpanel

Kontrollpanelerna på arbetsytan erbjuder en mängd olika alternativ och konfigurationer som du kan använda när du skapar en kontrollpanel. I det här avsnittet går vi igenom den allmänna processen att skapa en kontrollpanel.

{{step1-to-dashboards}}

1. Klicka på **Arbetsytans kontrollpaneler** i den vänstra panelen.

1. Klicka på **Ny instrumentpanel** i det övre högra hörnet.

1. I rutan **Skapa instrumentpanel**

1. Ange följande:

   <table style="table-layout:auto">
    <col>
    <col>
    <tbody>
     <tr>
      <td role="rowheader"><strong>Namn</strong></td>
      <td><p>Ange ett namn för instrumentpanelen. Vi rekommenderar att du endast använder UTF-8-tecken för att undvika kompatibilitetsproblem.</p></td>
     </tr>
     <tr>
      <td role="rowheader"><strong>Beskrivning (valfritt)</strong></td>
      <td>Ange en beskrivning av instrumentpanelen.</td>
     </tr>
      <tr>
      <td role="rowheader"><strong>Valuta</strong></td>
      <td>Välj standardvalutatypen för instrumentpanelen. <br>
      <br> Användare kan växla mellan olika valutatyper när de filtrerar kontrollpanelen. Mer information finns i <a href="/help/quicksilver/reports-and-dashboards/canvas-dashboards/manage-canvas-dashboards/filter-canvas-dashboard.md">Filtrera en instrumentpanel efter valutatyp</a>.</td>
     </tr>
    </tbody>
   </table>

1. Klicka på **Skapa**. Rutan **Lägg till rapport** öppnas. Här kan du skapa en ny rapport eller lägga till en befintlig rapport på kontrollpanelen.

## Lägga till en rapport på en instrumentpanel

När du har skapat en kontrollpanel lägger du till rapporter i den i nästa steg. Du kan göra detta genom att antingen skapa en helt ny rapport i sektionen Kontrollpaneler på arbetsytan eller lägga till en befintlig.

Det finns tre typer av rapporter som du kan skapa i Canvas Dashboards:

* **KPI**: Den här rapporten visar nyckelprestandaindikatordata som ett tal.
Mer information finns i [Skapa en KPI-rapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-kpi-report.md).

* **Diagram**: Den här rapporten visar dina data som stapeldiagram, stapeldiagram, linjediagram eller cirkeldiagram.
Mer information finns i [Skapa en diagramrapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-chart-report.md).

* **Tabell**: Den här rapporten visar dina data i ett tabellformat.
Mer information finns i [Skapa en tabellrapport](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/build-table-report.md).

Mer information om hur du lägger till en befintlig rapport på en kontrollpanel finns i [Lägga till en befintlig rapport på en kontrollpanel](/help/quicksilver/reports-and-dashboards/canvas-dashboards/add-reports/add-existing-report.md).
