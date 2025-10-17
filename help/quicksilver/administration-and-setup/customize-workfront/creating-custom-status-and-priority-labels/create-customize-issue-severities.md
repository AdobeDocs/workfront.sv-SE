---
title: Skapa eller anpassa allvarlighetsgrader för utgåvor
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Dina användare kan använda allvarlighetsgrader för att definiera hur allvarligt ett problem är. Du kan anpassa någon av de fem standardserierna som finns i Adobe Workfront eller skapa en ny allvarlighetsgrad för dina användare.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '641'
ht-degree: 0%

---

# Skapa eller anpassa utgåvans allvarlighetsgrad

{{highlighted-preview}}

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview Sandbox environment, and is being released in a phased rollout to Production.</span>-->

<!--
DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS.

Linked to Understanding Issue Severity.
-->

Dina användare kan använda allvarlighetsgrader för att definiera hur allvarligt ett problem är. Du kan anpassa någon av de fem standardserierna som finns i Adobe Workfront eller skapa en ny allvarlighetsgrad för dina användare.

>[!NOTE]
>
>Aktiviteter och projekt har ingen allvarlighetsgrad.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td><p>Alla</p></td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td><p>Standard</p>
       <p>Plan</p></td>
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Systemadministratör</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++ 

## Inbyggda problemallvarlighetsgrader

Workfront har fem inbyggda problemallvarlighetsgrader:

* Kosmetisk
* Orsakar förvirring
* Fel med tillfälliga lösningar
* Fel utan någon lösning
* Allvarligt fel

Du kan redigera följande för dessa allvarlighetsgrader:

* Namn
* Färg

  Färgen för en allvarlighetsgrad bevaras i en diagramrapport om du grupperar dina resultat efter allvarlighetsgrad för problem. Mer information om diagramrapporter finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Vilken allvarlighetsgrad som är standard

  Mer information om standardallvarlighetsgrader finns i [Skapa eller redigera en utgåva med allvarlighetsgrad](#create-or-edit-an-issue-severity) i den här artikeln.

* Beskrivning
* Om en allvarlighetsgrad är dold i Workfront

  Mer information om hur du döljer en allvarlighetsgrad finns i [Skapa eller redigera en allvarlighetsgrad för ett problem](#create-or-edit-an-issue-severity) i den här artikeln.

* Ta bort en allvarlighetsgrad

  När du gör detta måste du välja en ersättningsallvarlighetsgrad.

## Skapa eller redigera en allvarlighetsgrad för ett problem {#create-or-edit-an-issue-severity}

Som Workfront-administratör kan du skapa och redigera utgåvor som passar dina användares behov.

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Allvarlighetsgrader** i den vänstra panelen.

1. Om du skapar en ny allvarlighetsgrad klickar du på <span class="preview">**Ny rad** längst ned i tabellen</span> eller **Lägg till en ny allvarlighetsgrad**.
1. Konfigurera följande alternativ för den nya allvarlighetsgraden eller redigera dem för en befintlig:

   * **Allvarlighetsgrad**: Ange ett namn för allvarlighetsgraden.
   * **Viktighet**: Öka eller minska allvarlighetsgraden, som ursprungligen tilldelats av Workfront, för allvarlighetsgraden.

     Importnumret för varje allvarlighetsgrad måste vara unikt. Den högsta siffran motsvarar den högsta allvarlighetsgraden.

     Du kan inte redigera det här talet när du har sparat allvarlighetsgraden.

   * **Färg**: Välj en färg för allvarlighetsgraden.

     Färgen på allvarlighetsgraden används i diagramrapporter när du grupperar dina resultat efter allvarlighetsgrad för problem. Mer information om diagramrapporter finns i [Lägga till ett diagram i en rapport](/help/quicksilver/reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

   * **Standardallvarlighetsgrad**: Välj den allvarlighetsgrad du vill att Workfront ska tillämpa automatiskt på alla nyskapade problem.

     **Kosmetisk** är standardallvarlighetsgrad för problem i Workfront.

     Du kan inte göra en dold allvarlighetsgrad till standard.

     <div class="preview">

     Standardallvarlighetsgraden anges med ikonen ![Standardallvarlighetsgrad](assets/default-icon.png). Gör något av följande om du vill välja en ny standard:

      * Markera kryssrutan bredvid allvarlighetsgraden och välj **Gör standard** i åtgärdsfältet längst ned på skärmen.
      * Håll muspekaren över allvarlighetsgraden och klicka på menyn **Mer** som visas. Välj sedan **Använd som standard**.

        Den nya standardallvarlighetsgraden anges med ikonen .

     </div>

   * **Beskrivning**: Ange en beskrivning av allvarlighetsgraden för att förklara dess funktion.
   * <span class="preview">**Dölj alternativ**</span> eller **Dölj**: <span class="preview">Välj **Ja**</span> eller markera kryssrutan för att dölja en allvarlighetsgrad som inte längre behövs.

     En dold allvarlighetsgrad visas inte någonstans i Workfront, så användarna kan inte välja den för sina utgåvor.

     >[!IMPORTANT]
     >
     >I stället för att ta bort de allvarlighetsgrader som du inte längre vill använda föreslår vi att du döljer dem. På så sätt kan du behålla alla dina historiska data om objekt som redan har slutförts med allvarlighetsgraden, samtidigt som du förhindrar att personer använder allvarlighetsgraden i framtiden.

1. (Valfritt) Ändra listordningen för dina allvarlighetsgrader genom att dra och släppa dem i önskad ordning.

   Detta ändrar visningsordningen för problem. Det ändrar inte **Importance**-numret.

1. Klicka på **Spara**.

Mer information om hur du använder allvarlighetsgrader när du arbetar med problem finns i [Uppdatera allvarlighetsgrad](../../../manage-work/issues/issue-information/update-issue-severity.md).
