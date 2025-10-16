---
product-area: reporting
navigation-topic: create-and-manage-reports
title: Redigera rapportinställningar
description: Du kan redigera inställningarna för en rapport för att definiera hur den ska visas för andra användare, eller vilken typ av information som användare kan fråga innan de kör rapporten.
author: Nolan
feature: Reports and Dashboards
exl-id: 6fbbc557-65da-4ffe-968a-9c8db6a45811
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '612'
ht-degree: 0%

---

# Redigera rapportinställningar

<!-- Audited: 11/2024 -->

Du kan redigera inställningarna för en rapport för att definiera hur den ska visas för andra användare, eller vilken typ av information som användare kan fråga innan de kör rapporten.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td> 
      <p>Standard</p>
      <p>Plan</p>
   </td>
  </tr> 
  <tr> 
   <td role="rowheader">Åtkomstnivåkonfiguration</td> 
   <td> <p>Redigera åtkomst till rapporter, instrumentpaneler och kalendrar</p> <p>Redigera åtkomst till filter, vyer, grupperingar</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
 <td> <p>Hantera behörigheter i en rapport</p></td>  
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Instruktioner

1. Börja skapa en rapport genom att gå till **huvudmenyn** > **Rapporter** och sedan markera objektet för rapporten.

   eller

   Öppna en befintlig rapport och klicka sedan på **Rapportåtgärder** > **Redigera**.

1. Klicka på **Rapportinställningar** i det övre högra hörnet i Report Builder.
1. Konfigurera följande rapportinställningar:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Rapporttitel</td> 
      <td>Ange en rubrik för rapporten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en programsats som beskriver rapportens syfte och användningsområden.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Kör den här rapporten med åtkomsträttigheter för</td> 
      <td>Välj den användare vars åtkomsträttigheter du vill att den här rapporten ska användas när den visas för andra användare. Mer information om hur du kör en rapport med åtkomsträttigheter för en annan användare finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/run-deliver-report-access-rights-another-user.md" class="MCXref xref">Kör och leverera en rapport med åtkomsträttigheter för en annan användare</a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa</td> 
      <td>Välj standardfliken som visas för alla användare när rapporten läses in.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa ... objekt när rapporten läses in på en kontrollpanel</td> 
      <td>Ange antalet objekt som ska visas för alla användare när rapporten läses in på en kontrollpanel. Standardvärdet är 15 objekt och det maximala antalet objekt är 200.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa vyn Resursstödraster på fliken Information</td> 
      <td> <p>(Endast användarrapport) Välj det här alternativet om du vill visa resursstödrastret på fliken Information i rapporten.</p> <p>Obs! När du använder vyn Resursstödraster på en användarrapport visas endast projekt som har statusen Aktuell. Om du vill se projekt med någon annan status kan du använda fliken Användare i området Personer i det globala navigeringsfältet och använda vyn Resursstödraster där. <!--
         <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
          For more information about using the Resource Grid, see the article Overview of the Resource Grid . (drafted because this article is drafted also: Article is in draft Feb 1, 2021)
         </MadCap:conditionalText>
        --></p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa en särskild vy på fliken Detaljer</td> 
      <td>(Endast projektrapport) Ange vilken typ av vy som användare ska se när de öppnar informationen på fliken Information. Du kan till exempel välja en milstolpe- eller Gantt-vy.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Visa den här rapporten i en Gantt-vy som standard</td> 
      <td>(Endast projektrapport och Aktivitetsrapport) Välj det här alternativet om du vill att Gantt-vyn ska aktiveras automatiskt när användare visar fliken Information i den här rapporten.<br>Mer information om hur du visar Gantt-schemat i projektrapporter och aktivitetsrapporter finns i avsnittet Visa aktivitetsinformation i projektlistan Gantt-schema i artikeln <a href="../../../manage-work/gantt-chart/use-the-gantt-chart/view-info-in-gantt.md" class="MCXref xref">Visa information i Gantt-schemat </a>.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt att vy ändras i rapporten</td> 
      <td>Välj det här alternativet om du vill tillåta användare att ändra vyn när de kör rapporten.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt att gruppen ändras i rapporten</td> 
      <td>Välj det här alternativet om du vill tillåta användare att ändra gruppen när rapporten körs.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Tillåt att filter ändras i rapporten</td> 
      <td>Välj det här alternativet om du vill tillåta användare att ändra filtret när rapporten körs.</td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **Rapportera uppmaningar** om du vill konfigurera eventuella uppmaningar för rapporten.\
   Mer information om hur du lägger till uppmaningar i en rapport finns i artikeln [Lägg till en uppmaning i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-prompt-report.md).

1. Klicka på **Klar,** och sedan på **Spara + stäng**.

## Ytterligare information

Se även:

<!--outdated: * [Basic Report Creation Program for the new Workfront experience](https://one.workfront.com/s/basic-report-creation-program) -->
* [Kom igång med rapporter](../../../reports-and-dashboards/reports/reporting/get-started-reports-workfront.md)
* [Använd inbyggda Adobe Workfront-rapporter](../../../reports-and-dashboards/reports/using-built-in-reports/use-workfront-built-in-reports.md)
* [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md)
