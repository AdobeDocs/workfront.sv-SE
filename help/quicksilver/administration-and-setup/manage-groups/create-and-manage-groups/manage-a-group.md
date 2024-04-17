---
user-type: administrator
product-area: system-administration;user-management
keywords: hantera,gruppera,redigera,
navigation-topic: create-and-manage-groups
title: Hantera en grupp
description: Som gruppadministratör kan du hantera en grupp som du administrerar från området Grupper i Inställningar. Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 86c120de-16b8-4ca8-a7a1-76ece70c0505
source-git-commit: 0afd578ebaa55d911c04a1d08fbcadddc1d05bbc
workflow-type: tm+mt
source-wordcount: '1319'
ht-degree: 0%

---

# Hantera en grupp

<!--
Though this might not seem that helpful because it is more of a catalog/TOC, it's the only article to link to for editing a group. Don't remove it.
-->

Som gruppadministratör kan du hantera en grupp som du administrerar från området Grupper i Inställningar. Om det finns grupper ovanför gruppen som du hanterar kan deras administratörer även göra detta för gruppen. Detsamma gäller för Workfront-administratörer (för alla grupper).

>[!NOTE]
>
>När du tilldelas som administratör för en grupp ärver du gruppadministratörsrollen för alla undergrupper som finns under den. De enda användare som kan hantera en undergrupp är gruppadministratörer för den översta gruppen ovanför och alla gruppadministratörer som har tilldelats undergruppen.

## Åtkomstkrav

Du måste ha följande för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Workfront-plan*</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> <p>Du måste vara gruppadministratör för gruppen eller Workfront-administratör. Mer information finns i <a href="../../../administration-and-setup/manage-groups/group-roles/group-administrators.md" class="MCXref xref">Gruppadministratörer</a> och <a href="../../../administration-and-setup/add-users/configure-and-grant-access/grant-a-user-full-administrative-access.md" class="MCXref xref">Bevilja användaren fullständig administrativ åtkomst</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du behöver ta reda på vilken plan eller licenstyp du har.

## Hantera medlemskap i en grupp

Du kan lägga till och ta bort användare och andra grupper från en grupp som du administrerar. Du kan också tilldela gruppmedlemmar som administratörer för gruppen och hantera användarprofilinformationen för gruppmedlemmar.

Instruktioner finns i [Visa och hantera medlemskap i en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-memberships.md).

## Hantera information om en grupp

Du kan visa och redigera sidan Gruppinformation för en grupp eller undergrupp som du hanterar. Den här sidan innehåller en beskrivning av gruppen, namnen på affärsledaren och gruppadministratörer samt ett alternativ som gör att du kan göra gruppen och alla dess undergrupper offentliga eller privata. Och om din åtkomstnivå tillåter dig att hantera anpassade formulär kan du bifoga ett anpassat formulär till en grupp.

<!--
"and an option that allows you to deactivate or reactivate the group"

Add this at end of 2nd-to-last sentence in this^ paragraph when they add the **Is active** option to the Details page!
-->

Instruktioner finns i [Visa och hantera information om en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md).

## Redigera, kopiera eller ta bort en grupp

Utan att lämna huvudsidan i en grupp som du visar kan du snabbt redigera, kopiera eller ta bort gruppen.

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Adobe Workfront övre högra hörn och klicka sedan på **Inställningar** ![](assets/gear-icon-settings.png).

1. Klicka **Grupper**.

   I listan som visas kan du se de grupper som du hanterar, tillsammans med eventuella undergrupper som de har. Adobe Workfront-administratörer kan se alla grupper.

1. Markera gruppen och klicka sedan på Redigera ![](assets/edit-icon.png), kopiera ![](assets/copy-icon.png)eller Delete ![](assets/delete.png) -ikon.

   Om du behöver information om hur du använder rutan som visas kan du läsa något av följande:

   * **Redigera**: [Visa och hantera information om en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-manage-a-groups-details.md)

   * **Kopiera**: [Skapa en grupp på den översta nivån genom att kopiera en befintlig grupp eller undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md#copying-an-existing-group-and-sub-group) i artikeln [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md)

   * **Ta bort**: [Ta bort en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/delete-a-group.md)

## Konfigurera projekt-, uppgifts- och utgivningsinställningar för en grupp

Om du är gruppadministratör och din grupp behöver andra inställningar för projekt, uppgifter och utgåvor än de som har angetts på systemnivån kan du be Workfront-administratören att låsa upp en inställning för alla grupper i hela organisationen. När den har låsts upp kan du (och gruppadministratörer för alla andra grupper) konfigurera den för de grupper som du hanterar.

Instruktioner finns i [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md) och  [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md).

## Visa, lägga till och konfigurera undergrupper

Du kan skapa, visa, redigera, kopiera, byta namn på, exportera och ta bort undergrupper under en grupp som du administrerar.

## Konfigurera händelseaviseringar för en grupp

Om en Workfront-administratör låser upp möjligheten att konfigurera händelsemeddelanden för grupperna i din organisation kan du konfigurera dem för en grupp som du administrerar. Instruktioner finns i [Visa och konfigurera händelseaviseringar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).

## Skapa och anpassa statusar för en grupp

Som gruppadministratör kan du skapa anpassade statusvärden för en grupp på den översta nivån som du hanterar. Detta ger er gruppoberoende och bidrar till att eliminera behovet av dussintals företagsövergripande anpassade statyer. (En Workfront-administratör kan även göra detta för alla grupper.)

Du kan också anpassa systemstatus för en grupp på den översta nivån om en Workfront-administratör har konfigurerat dem för att tillåta anpassning.

Instruktioner finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).

## Arbeta med en grupps projekt

När du visar huvudsidan för en grupp som du administrerar i området Grupper i Konfigurera kan du göra följande med projekt:

* Visa och arbeta med (redigera, kopiera, ta bort och exportera) projekt som är kopplade till gruppen och dess undergrupper och som har delats med dig
* Skapa ett nytt projekt för gruppen

Instruktioner finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-projects.md).

## Visa och hantera en grupps godkännandeprocesser

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med de godkännandeprocesser som administratörerna för gruppen, eller någon av dess undergrupper, har administratörsbehörighet för.

Instruktioner finns i [Godkännandeprocesser på gruppnivå](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-groups-approval-processes.md).

## Visa och hantera en grupps layoutmallar

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med den layoutmall som administratörerna för gruppen, eller en av dess undergrupper, har administratörsbehörighet för.

Instruktioner finns i [Skapa och ändra en grupps layoutmallar](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-layout-templates.md).

## Visa och hantera gruppmedlemmars scheman

En gruppadministratör som skapar ett schema för en grupp måste ange den grupp vars administratörer ska hantera schemat. Vanligtvis är detta den grupp som schemat skapas för, men det kan vara en annan grupp om gruppadministratören hanterar flera grupper och anger en av de andra i stället.

När du visar huvudsidan för en grupp som du hanterar kan du visa och hantera schemat från gruppens sida, om gruppen är utsedd till den vars administratörer kan redigera ett schema.

Instruktioner finns i [Skapa och ändra en grupps scheman](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-schedules.md).

## Visa och hantera gruppmedlemmarnas tidrapportprofiler

När du visar huvudsidan för en grupp som du administrerar kan du hantera de tidrapportprofiler som du och andra administratörer i gruppen - eller någon av dess undergrupper - har behörighet att redigera. Instruktioner finns i [Skapa och hantera en grupps tidrapportprofiler](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-timesheet-profiles.md).

## Visa och hantera undergruppsmedlemmar

När du visar huvudsidan för en grupp som du administrerar kan du visa och hantera alla användare i gruppens undergrupper. Instruktioner finns i [Visa och hantera undergruppsmedlemmar](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/view-and-manage-subgroup-members.md).

## Visa och hantera en grupps team

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med team som är kopplade till gruppen eller någon av dess undergrupper.

Instruktioner finns i [Skapa och ändra en grupps team](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-teams.md).

## Visa och hantera en grupps företag

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med företag som är kopplade till gruppen eller någon av dess undergrupper. Instruktioner finns i [Skapa och ändra en grupps företag](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-companies.md).

## Visa och hantera en grupps portföljer och program

När du visar en grupp som du hanterar i området Grupper kan du visa och arbeta med portföljer och program när båda följande gäller:

* De är kopplade till gruppen som du visar eller någon av dess undergrupper
* Du har behörighet att visa dem eftersom du skapade dem eller så delades de med dig

Instruktioner finns i [Skapa och ändra en grupps projekt](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-portfolios.md) och [Skapa, ändra och visa en grupps program](../../../administration-and-setup/manage-groups/work-with-group-objects/create-and-modify-a-groups-programs.md).

## Inaktivera eller återaktivera en grupp

<!--
DRAFTED IN FLARE:
Delete this section when they add the </span>
<b>Is active</b>
 option to the Details page!</span>

-->

Du kan behålla en grupps standardläge som aktiv eller inaktivera den.

Det kan vara praktiskt att inaktivera en grupp när den inte används just nu eftersom användare inte längre ser den i textbaserade fält när de söker efter en grupp som de vill associera med ett annat objekt.

Instruktioner om hur du gör en grupp inaktiv eller aktiv finns i [Inaktivera eller återaktivera en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/deactivate-or-reactivate-a-group.md).
