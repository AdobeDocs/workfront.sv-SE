---
user-type: administrator
product-area: system-administration;user-management
navigation-topic: work-with-a-groups-objects
title: Skapa och hantera en grupps tidrapportprofiler
description: När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med de tidrapportprofiler som administratörerna för gruppen, eller någon av dess undergrupper, har administratörsbehörighet för.
author: Caroline
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 5c895e77-bd88-435f-a903-37c2325eab45
source-git-commit: fe399743ee495334face9d4d632686d9472bc8ef
workflow-type: tm+mt
source-wordcount: '412'
ht-degree: 0%

---

# Skapa och hantera en grupps tidrapportprofiler

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">Do this to other step articles about objects and groups? Remove steps and point to main article; add group or step in that article. Already done previously for approval processes.</p>
-->

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med de tidrapportprofiler som administratörerna för gruppen, eller någon av dess undergrupper, har administratörsbehörighet för.

Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

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
   <td>Plan</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Du måste vara gruppadministratör för gruppen.</p>  <p>Du måste också ha administrativ åtkomst till tidrapporter. Mer information finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md" class="MCXref xref" data-mc-variable-override="">Ge användarna administrativ åtkomst till vissa områden</a>.</p>  <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref" data-mc-variable-override="">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Skapa och redigera tidrapportprofiler på gruppnivå

Du kan skapa och redigera tidrapportprofiler som ska användas i en grupp som du hanterar. Instruktioner finns i [Skapa, redigera och tilldela tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

## Ta bort tidrapportprofiler på gruppnivå

Du kan ta bort tidrapportprofiler som används av en grupp som du hanterar. Instruktioner finns i [Ta bort tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/delete-timesheet-profiles.md).

## Generera grupptidrapporter manuellt

Om du vill aktivera ändringar som du har gjort för att gruppera tidrapportprofiler så att de återspeglar den aktuella gruppens tidrapporter, måste du först ta bort de befintliga tidrapporterna och sedan generera nya manuellt. Instruktioner finns i [Generera tidrapporter manuellt från tidrapporter och timmar](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md#manually) in [Generera tidrapporter manuellt](../../../timesheets/create-and-manage-timesheets/manually-generate-timesheets.md).

Mer information om hur du tar bort grupptidrapporter finns i [Ta bort tidrapporter i Adobe Workfront](../../../timesheets/create-and-manage-timesheets/delete-timesheets.md).

## Exportera tidrapportprofiler på gruppnivå

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).
1. Klicka **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Klicka på namnet på gruppen med de tidrapportprofiler som du vill exportera.
1. Klicka **Tidrapportprofiler**.
1. Klicka **Exportera** om du vill exportera listan med tidrapportprofiler för gruppen.
