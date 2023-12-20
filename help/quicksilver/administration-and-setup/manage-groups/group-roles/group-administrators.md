---
title: Gruppadministratörer
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: group-roles
description: Adobe Workfront-administratörer i stora organisationer med många avdelningar kanske inte vill hantera alla avdelningar och grupper inom dessa avdelningar. I stället kan de skapa en grupp för varje avdelning och undergrupper inom den gruppen, som alla hanteras av en gruppadministratör.
author: Lisa
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 589cf9fb-f195-4b69-a240-3f73e6ca623e
source-git-commit: 850e0801511177efc5189258acd9b88234cf59c9
workflow-type: tm+mt
source-wordcount: '1047'
ht-degree: 0%

---

# Gruppadministratörer

<!-- Audited: 12/2023 -->

Adobe Workfront-administratörer i stora organisationer med många avdelningar kanske inte vill hantera alla avdelningar och grupper inom dessa avdelningar. I stället kan de skapa en grupp för varje avdelning och undergrupper inom den gruppen, som alla hanteras av en gruppadministratör.

En gruppadministratör kan hantera en grupps behov, t.ex. användarmedlemskap, layoutmallar, anpassade data, statusvärden och inställningar.

Upp till 14 nivåer av undergrupper kan finnas under en grupp.

>[!NOTE]
>
>Alla gruppadministratörer i hierarkin ovanför en undergrupp har administratörsbehörighet för att hantera den undergruppen.

Mer information om hur du skapar och hanterar grupper finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md) och [Hantera en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/manage-a-group.md). Se även [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md).

## Utse gruppadministratörer

Varje grupp på den översta nivån måste ha minst en gruppadministratör. En Workfront-administratör eller administratör för en grupp kan tilldela gruppadministratörer till gruppens undergrupper, men detta är inte nödvändigt. Mer information finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

Om du är Workfront-administratör rekommenderar vi att du gör följande innan du anger användare som gruppadministratörer:

* Notera det aktuella antalet Workfront-administratörer i systemet.
* Notera hur många grupper du har i datorn.
* Ange om du kan ändra åtkomstnivån för vissa av Workfront-administratörerna och utse dem till gruppadministratörer i stället.

  Mer information om funktionerna för gruppadministratörer finns i [Uppgifter som utförs av gruppadministratörer](#tasks-done-by-group-administrators) i den här artikeln.

* Ange om du vill att gruppadministratörer ska kunna logga in som andra användare eller återställa lösenord för användare i de grupper som du administrerar. Ytterligare åtkomst krävs för att utföra dessa uppgifter, vilket förklaras nedan [Åtkomst krävs för gruppadministratörer](#access-needed-for-group-administrators).
* För bättre användarhantering bör du överväga att tilldela grupper eller undergrupper i stället för användare till följande objekt:

   * Layoutmallar
   * Scheman
   * Tidrapportprofiler

## Åtkomst krävs för gruppadministratörer {#access-needed-for-group-administrators}

Alla gruppadministratörer måste ha

* En planlicens i den aktuella prissättnings- och paketeringsmodellen
* En standardlicens i den nya prissättnings- och paketeringsmodellen

Vi rekommenderar att gruppadministratörer har behörighet att redigera för användare så att de kan utföra följande uppgifter:

* Logga in som andra användare i de grupper och undergrupper som de hanterar.
* Återställ lösenordet för en annan användare i de grupper som han/hon hanterar.

>[!IMPORTANT]
>
>Gruppadministratörer måste ha högre åtkomst än de som de hanterar, annars kan de inte visa eller ändra lägre åtkomstnivåer.
>Instruktioner om hur du beviljar åtkomst finns i [Skapa eller ändra anpassade åtkomstnivåer](../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md).

För en gruppadministratör som behöver tilldela tidrapportprofiler till användare i sina grupper och undergrupper rekommenderar vi även administratörsåtkomst till tidrapporter och timmar. Instruktioner om hur du beviljar åtkomst finns i [Ge användarna administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

## Uppgifter som utförs av gruppadministratörer {#tasks-done-by-group-administrators}

Som gruppadministratör kan du utföra de uppgifter som beskrivs nedan för att hantera de grupper som du övervakar. Vissa av dessa funktioner är desamma som för en Workfront-administratör.

>[!NOTE]
>
>I den nya prissättnings- och paketeringsmodellen måste du ha en Prime-plan eller högre för att kunna utföra följande:
>
> * Skapa grupphändelseaviseringar
> * Konfigurera inställningar för gruppprojekt
> * Konfigurera inställningar för gruppaktivitet och -problem
> * Lås upp konfiguration av undergruppsinställningar
> * Gruppera tidrapport och timinställningar
> * Lås upp tidrapport och timinställning

### Hantera gruppmedlemmar {#manage-group-members}

* Skapa, redigera och ta bort undergrupper i de grupper och undergrupper som du hanterar. Instruktioner finns i [Skapa en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).
* Lägg till användare som du har redigeringsåtkomst för till dina grupper och undergrupper. Eller lägg till användare i grupper och undergrupper genom att redigera deras profiler.

  Du kan även uppdatera fälten i en gruppmedlems profil om du har behörigheten Användaradministratör (gruppanvändare) aktiverad på åtkomstnivån.

  Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

  >[!NOTE]
  >
  >Workfront-administratörer kan åsidosätta ändringar av gruppmedlemskap som gjorts av en gruppadministratör.

* Återställ lösenord för användare som är medlemmar i de grupper som du hanterar. Mer information finns i [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).
* Logga in som användare som är medlemmar i de grupper som du hanterar. Mer information finns i [Logga in som en annan användare](../../../administration-and-setup/add-users/create-and-manage-users/log-in-as-another-user.md).
* Visa antalet tillgängliga licenser för din grupp och undergrupperna under den. Mer information finns i [Hantera tillgängliga licenser i ditt system](../../../administration-and-setup/get-started-wf-administration/manage-available-licenses-in-your-system.md).

### Hantera gruppobjekt {#manage-group-objects}

* Skapa layoutmallar på gruppnivå och koppla dem till de grupper och undergrupper som du hanterar. Mer information finns i [Skapa och hantera layoutmallar](../../../administration-and-setup/customize-workfront/use-layout-templates/create-and-manage-layout-templates.md).
* Skapa tidrapportprofiler på gruppnivå, associera dem med användare och grupper som du hanterar och generera manuellt tidrapporter. Mer information finns i [Skapa, redigera och tilldela tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).
* Utan administrativ åtkomst till godkännandeprocesser kan du skapa och redigera godkännandeprocesser för de grupper och undergrupper som du hanterar. Mer information finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).

  Mer information om administrativ åtkomst till godkännandeprocesser finns i [Ge användarna administrativ åtkomst till vissa områden](../../../administration-and-setup/add-users/configure-and-grant-access/grant-users-admin-access-certain-areas.md).

* Skapa scheman och associera dem med en grupp som du hanterar. Mer information finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* Hantera ett team som har tilldelats en grupp som du hanterar, utan att vara medlem i teamet. Skapa också en teamrapport baserad på gruppfältet för att identifiera vilken grupp ett visst team har tilldelats. Mer information finns i [Skapa ett team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md).
* Återställ ett projekt som är kopplat till en grupp som du hanterar, tillsammans med uppgifter, problem eller dokument som är kopplade till projektet. Mer information finns i [Återställ borttagna objekt](../../../administration-and-setup/manage-workfront/manage-deleted-items/restore-deleted-items.md).

### Hantera gruppinställningar och verktyg {#manage-group-preferences-and-tools}

* När en projektinställning, en uppgift eller en utgåva, eller en tidrapport och en timinställning har låsts upp för grupper i hela systemet, redigerar du den inställningen för grupper som du hanterar. Inställningarna påverkar projekt, uppgifter och problembeteende. Mer information finns i följande:

   * [Konfigurera projektinställningar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-project-preferences-group.md)
   * [Konfigurera inställningar för aktiviteter och utgåvor för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/configure-task-issue-preferences-group.md)

* Skapa och redigera gruppstatus för grupper som du hanterar. Mer information finns i [Skapa eller redigera en gruppstatus](../../../administration-and-setup/manage-groups/manage-group-statuses/create-or-edit-a-group-status.md).
* Konfigurera ett händelsemeddelande för grupper som du hanterar. Du kan bara göra detta efter att en Workfront-administratör har låst upp möjligheten att konfigurera händelsemeddelanden för grupper via systemet. Mer information finns i [Visa och konfigurera händelseaviseringar för en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/view-and-configure-event-notifications-group.md).
