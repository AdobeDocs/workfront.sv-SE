---
product-area: reporting
keywords: användare,delegering,rapport,delegat,godkännande
navigation-topic: create-and-manage-reports
title: Skapa en delegeringsrapport för användare
description: Skapa en delegeringsrapport för användare
author: Nolan
feature: Reports and Dashboards
exl-id: c860574b-0488-499e-8d36-d0f3f85aac2d
source-git-commit: aa8275f252dd51f5a14d7aa931423aa4afb4ba8f
workflow-type: tm+mt
source-wordcount: '325'
ht-degree: 0%

---

# Skapa en delegeringsrapport för användare

<!--Audited: 10/2024-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: consider moving this to the Custom&nbsp;View, Filter, Grouping Samples section as an example of a report)</p>
-->

I Adobe Workfront kan användare delegera projekt, uppgifter och utfärda godkännanden till andra användare för att se till att deras godkännanden hanteras när de inte är på kontoret. Användare med en planlicens kan skapa en delegeringsrapport för användare för att se:

* Vem har delegerat sina uppgifter, utgåvor och projektgodkännanden till en annan användare
* Vilka användare som har delegerat uppgifter, utgåvor och projektgodkännanden som tilldelats dem

* Datum då delegationerna börjar och slutar

Mer information om hur du delegerar godkännanden finns i [Delegera godkännandebegäran](../../../review-and-approve-work/manage-approvals/delegate-approval-requests.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn more about delegating work, see <a href="../../../workfront-basics/manage-your-account-and-profile/manage-time-off/personal-time-off.md" class="MCXref xref">Log personal time off and delegate your work</a>.</p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">DRAFTED: To learn how to manage delegated work in Home, see [future link here].</p>
-->

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
 <td> <p>Visa behörigheter för de objekt vars godkännanden har delegerats och för de användare som deltar i delegeringen</p></td>  
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa en delegeringsrapport för användare

1. Klicka på ikonen **Huvudmeny** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Rapporter**.

1. Klicka på **Ny rapport** och välj sedan **Användardelegering**.

   ![Ny delegering av rapportanvändare](assets/classic-new-report-user-delegation-350x644.png)

   Följande fält visas som standard i den här rapporten:

   | Fält | Beskrivning |
   |---|---|
   | **Från användare** | Det här är användaren som delegerar uppgifter, utgåvor och projektgodkännanden till en annan användare. |
   | **Till användare** | Det här är den användare som har delegerat uppgifter, utgåvor och projektgodkännanden till sig. |
   | **Startdatum** | Detta är början på frånvarotiden för användaren som har gjort delegeringarna. |
   | **Slutdatum** | Detta är slutet på frånvarotiden för användaren som har gjort delegeringarna. |

   {style="table-layout:auto"}

1. (Valfritt) Ändra följande i Report Builder:

   * Kolumner (vy)
   * Grupperingar
   * Filter
   * Diagram

   Mer information om de här funktionerna finns i [Skapa en anpassad rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md).

1. När du är klar med att skapa rapporten klickar du på **Spara + stäng**.

   Rapporten visas.
