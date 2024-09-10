---
title: Skapa eller anpassa allvarlighetsgrader för utgåvor
user-type: administrator
product-area: system-administration;projects
navigation-topic: create-custom-status-and-priority-labels
description: Dina användare kan använda allvarlighetsgrader för att definiera hur allvarligt ett problem är. Du kan anpassa någon av de fem standardserierna som finns i Adobe Workfront eller skapa en ny allvarlighetsgrad för dina användare.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 0331be3c-a2d8-4788-a41a-5e971fb4bbe1
source-git-commit: 0bc2817255b8879de377c3916bb36be760f28f4c
workflow-type: tm+mt
source-wordcount: '562'
ht-degree: 0%

---

# Skapa eller anpassa utgåvans allvarlighetsgrad

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

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
     <p>Nytt: Standard</p>
     <p>eller</p>
     <p>Aktuell: Planera</p>
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>[!UICONTROL System Administrator]</td>
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Inbyggda problemallvarlighetsgrader

Workfront har fem inbyggda problemallvarlighetsgrader:

* Kosmetisk
* Orsakar förvirring
* Fel med tillfälliga lösningar
* Fel utan någon lösning
* Allvarligt fel

<p>Du kan redigera följande för dessa allvarlighetsgrader:</p>

* Namn
* Färg

  Färgen för en allvarlighetsgrad bevaras i en diagramrapport om du grupperar dina resultat efter allvarlighetsgrad för problem. Mer information om diagramrapporter finns i [Lägga till ett diagram i en rapport](../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md).

* Vilken allvarlighetsgrad som är standard

  Mer information om standardallvarlighetsgrader finns i [Skapa eller redigera en utgåva med allvarlighetsgrad](#create-or-edit-an-issue-severity) i den här artikeln.
* Beskrivning
* Om en allvarlighetsgrad är dold i Workfront

  Mer information om att dölja en allvarlighetsgrad finns i [Skapa eller redigera en allvarlighetsgrad för ett problem](#create-or-edit-an-issue-severity")

* Ta bort en allvarlighetsgrad

  När du gör detta måste du välja en ersättningsallvarlighetsgrad.

## Skapa eller redigera en allvarlighetsgrad för ett problem {#create-or-edit-an-issue-severity}

Som Workfront-administratör kan du skapa och redigera utgåvor som passar dina användares behov.

{{step-1-to-setup}}

1. Klicka på **Projektinställningar** > **Allvarlighetsgrader** i den vänstra panelen.

1. Om du skapar en ny allvarlighetsgrad klickar du på **Lägg till en ny allvarlighetsgrad**.
1. Konfigurera följande alternativ för den nya allvarlighetsgraden eller redigera dem för en befintlig:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">Allvarlighetsgrad</td> 
      <td>Ange ett namn för allvarlighetsgraden</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Prioritet</td> 
      <td>Öka eller minska allvarlighetsgraden, som ursprungligen tilldelats av Workfront, efter allvarlighetsgraden.
      <p>Importnumret för varje allvarlighetsgrad måste vara unikt. Den högsta siffran motsvarar den högsta allvarlighetsgraden.</p> <p>Du kan inte redigera det här talet när du har sparat allvarlighetsgraden.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Färg</td> 
      <td> <p>Välj en färg för allvarlighetsgraden.</p> 
      <p>Färgen på allvarlighetsgraden används i diagramrapporter när du grupperar dina resultat efter allvarlighetsgrad för problem. Mer information om diagramrapporter finns i <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/add-chart-report.md" class="MCXref xref">Lägga till ett diagram i en rapport</a>.</p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">Standardallvarlighetsgrad</td> 
      <td>Välj den allvarlighetsgrad du vill att Workfront automatiskt ska välja alla nyskapade problem.</p>
      <p>Cosmetic är standardallvarlighetsgraden för problem i Workfront.</p></td> 
     </tr> 
     <tr> 
      <td role="rowheader">Beskrivning</td> 
      <td>Ange en beskrivning av allvarlighetsgraden för att förklara dess funktion.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Dölj</td> 
      <td> Dölj en allvarlighetsgrad som inte längre behövs. 
      <p>En dold allvarlighetsgrad visas inte någonstans i Workfront, så användarna kan inte välja den för sina utgåvor.</p> 
      <p><b>VIKTIGT</b>: I stället för att ta bort de allvarlighetsgrader som du inte längre vill använda föreslår vi att du döljer dem. På så sätt kan du behålla alla dina historiska data om objekt som redan har slutförts med allvarlighetsgraden, samtidigt som du förhindrar att personer använder allvarlighetsgraden i framtiden.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Ändra listordningen för dina allvarlighetsgrader genom att dra och släppa dem i önskad ordning.

   Detta ändrar visningsordningen för problem. Det ändrar inte **Importance**-numret.

1. Klicka på **Spara**.

Mer information om hur du använder allvarlighetsgrader när du arbetar med problem finns i [Uppdatera allvarlighetsgrad](../../../manage-work/issues/issue-information/update-issue-severity.md).
