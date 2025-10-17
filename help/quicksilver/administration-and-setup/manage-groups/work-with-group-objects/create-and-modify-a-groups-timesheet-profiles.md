---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Skapa och hantera en grupps tidrapportprofiler
description: När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med de tidrapportprofiler som administratörerna för gruppen, eller någon av dess undergrupper, har administratörsbehörighet för.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '344'
ht-degree: 0%

---

# Skapa och hantera en grupps tidrapportprofiler

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med de tidrapportprofiler som administratörerna för gruppen, eller någon av dess undergrupper, har administratörsbehörighet för.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

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
   <td><p>Du måste vara gruppadministratör för gruppen eller systemadministratör.</p>
   <p>Du måste också ha administrativ åtkomst till tidrapporter.</p></td>
  </tr>
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Skapa och redigera tidrapportprofiler på gruppnivå

Du kan skapa och redigera tidrapportprofiler som ska användas i en grupp som du hanterar. Instruktioner finns i [Skapa, redigera och tilldela tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Ta bort tidrapportprofiler på gruppnivå

Du kan ta bort tidrapportprofiler som används av en grupp som du hanterar. Instruktioner finns i [Ta bort tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Generera grupptidrapporter manuellt

Om du vill aktivera ändringar som du har gjort för att gruppera tidrapportprofiler så att de återspeglar den aktuella gruppens tidrapporter, måste du först ta bort de befintliga tidrapporterna och sedan generera nya manuellt. Instruktioner finns i [Generera tidrapporter manuellt från tidrapporter och timmar](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) i [Generera tidrapporter manuellt](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Mer information om hur du tar bort grupptidrapporter finns i [Ta bort tidrapporter i Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exportera tidrapportprofiler på gruppnivå

{{step-1-to-setup}}

1. Klicka på **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen med de tidrapportprofiler som du vill exportera.
1. Klicka på **Tidrapportprofiler**.
1. Klicka på **Exportera** om du vill exportera listan med tidrapportprofiler för gruppen.
