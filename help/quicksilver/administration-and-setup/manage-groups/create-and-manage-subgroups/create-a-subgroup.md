---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: create-and-manage-subgroups
title: Skapa en undergrupp
description: Du kan skapa en undergrupp under en grupp som du hanterar för att ordna användare och projekt och för att tilldela behörigheter i Adobe Workfront. Vanligtvis hanterar gruppadministratörer grupper och undergrupper. De kan använda gruppsidan för att hantera sina grupper och undergrupper på ett och samma ställe.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: b59b1491-9a78-49c0-89c9-ab1ce0099e0b
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '636'
ht-degree: 0%

---

# Skapa en undergrupp

Du kan skapa en undergrupp under en grupp som du hanterar för att ordna användare och projekt och för att tilldela behörigheter i Adobe Workfront.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

Vanligtvis hanterar gruppadministratörer grupper och undergrupper. De kan använda gruppsidan för att hantera sina grupper och undergrupper på ett och samma ställe. Mer information om hur grupper och undergrupper fungerar i Workfront finns i [Översikt över grupper](../../../administration-and-setup/manage-groups/groups-overview/groups.md) och [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

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
   <td>Du måste vara gruppadministratör för gruppen eller systemadministratör.</td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Lägg till en undergrupp

{{step-1-to-setup}}

1. Klicka på **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Markera den befintliga gruppen eller undergruppen där du vill lägga till en ny undergrupp.
1. Klicka på **Ny undergrupp**.
1. Skriv ett **gruppnamn** för undergruppen i rutan **Ny undergrupp** som visas.
1. (Valfritt) Ange någon av följande uppgifter:

   * **Beskrivning**: Ange en beskrivning för undergruppen. Du kan skriva upp till 512 tecken.
   * **Är aktiv**: Det här alternativet är aktiverat som standard och gör gruppen aktiv i din Workfront-instans.

     När vanliga användare söker efter en grupp för att bifoga den till ett objekt eller för att dela ett objekt i typsnittsfält som det som visas nedan, visas endast aktiva grupper i listan.

     ![Typhuvudfält för en grupp](assets/typeahead-for-group.png)

     Om du vill effektivisera detta för dina användare kan du inaktivera alternativet **Är aktiv** för grupper som inte används för närvarande.

     Du kan enkelt visa, filtrera och gruppera grupplistan baserat på aktiv eller inaktiv status i det här fältet. Mer information om hur du använder vyer, filter och grupperingar i listor finns i [Rapportera element: filter, vyer och grupperingar](/help/quicksilver/reports-and-dashboards/reports/reporting-elements/reporting-elements-filters-views-groupings.md).

   * **Affärsledare**: Du kan tilldela en användare som affärsledare för en undergrupp som du hanterar. En företagsledare är någon som fattar affärsbeslut för undergruppen. Mer information finns i [Översikt över företagsledare](/help/quicksilver/administration-and-setup/manage-groups/group-roles/business-leader-overview.md).

     Om personen inte redan är medlem i undergruppen läggs även personens namn till i gruppen om du lägger till personen i det här fältet.

     >[!NOTE]
     >
     >* Innan du kan ta bort affärsledaren från en undergrupp måste du ta bort deras namn från fältet Affärsledare.
     >* Om du tar bort namnet från fältet Affärsledare förblir användaren medlem i undergruppen såvida du inte tar bort dem från den. Instruktioner om hur du tar bort någon från en grupp finns i [Visa och hantera en grupps medlemskap](/help/quicksilver/administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

   * **Gruppmedlemmar och gruppadministratörer**: Om du vill lägga till användare och grupper som medlemmar i undergruppen börjar du att skriva namnet på en befintlig användare eller grupp som du vill lägga till och markerar sedan namnet när det visas.

     De användare och grupper som du lägger till har åtkomst till alla objekt som delas med gruppen.

     En undergrupp ärver gruppadministratörerna för gruppen ovanför, så det är valfritt att ange en användare som gruppadministratör för en undergrupp. Du kan tilldela en gruppmedlem som administratör för gruppen med den nedrullningsbara menyn till höger om användarens namn.

   * **Sök efter personer och grupper i listan**: Om du behöver hitta en användare eller grupp som redan har tilldelats den här undergruppen kan du skriva deras namn här och markera den när den visas.

1. Klicka på **Spara.**
