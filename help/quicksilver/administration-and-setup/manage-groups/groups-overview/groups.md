---
title: Översikt över grupper
user-type: administrator
content-type: reference;overview
product-area: system-administration;user-management
navigation-topic: groups-overview
description: En Workfront-administratör kan skapa användargrupper som sammanfaller med avdelningsstrukturen. Grupper liknar, men skiljer sig från, team och företag.
author: Becky
feature: System Setup and Administration, People Teams and Groups
role: Admin
exl-id: 1353ab04-7de7-4d30-a092-27807c950777
source-git-commit: c711541f3e166f9700195420711d95ce782a44b2
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Översikt över grupper

<!-- Audited: 01/2024 -->

En Workfront-administratör kan skapa användargrupper som sammanfaller med avdelningsstrukturen. Grupper liknar, men skiljer sig från, team och företag.

Workfront-administratören ger grupper åtkomst till de områden i Workfront där de behöver arbeta och kommunicera. Varje grupp kan sedan separera sin Workfront-information, t.ex. användare, mallar, egna formulär och projekt från andra avdelningar.

Minst en gruppadministratör krävs för varje grupp. Gruppadministratörer kan använda gruppsidan för att hantera sina grupper på ett och samma ställe. Mer information finns i [Gruppadministratörer](../../../administration-and-setup/manage-groups/group-roles/group-administrators.md).

Du kan skapa upp till 14 nivåer med undergrupper under en grupp. Mer information finns i [Översikt över undergrupper](../../../administration-and-setup/manage-groups/groups-overview/subgroups.md) och [Skapa en undergrupp](../../../administration-and-setup/manage-groups/create-and-manage-subgroups/create-a-subgroup.md).

## Organisera användare med grupper

Som Workfront-administratör eller gruppadministratör kan du associera användare med grupper och undergrupper. Om du gör en grupp offentlig kan användare med en Standard- (ny) eller Plan-licens (aktuell) associera användare med den. Mer information om gruppadministratörer och offentliga grupper finns i [Skapa en grupp](../../../administration-and-setup/manage-groups/create-and-manage-groups/create-a-group.md).

När du skapar en användare rekommenderar vi att du lägger till användaren i rätt hemgrupp och andra grupper som användaren ska arbeta i. En användare kan bara ha en hemgrupp, men kan finnas i flera andra grupper.

Genom att vara en del av en grupp får användaren åtkomst till objekt som delas med gruppen och undergrupperna. Om du till exempel delar ett projekt med en grupp har användarna i gruppen och gruppens undergrupper åtkomst till det.

>[!TIP]
>
>Om avdelningarna i organisationen ofta arbetar tillsammans för att hantera projekt och resurser i dessa projekt, kanske det inte är nödvändigt att dela upp avdelningarna i många mindre grupper. Några högnivågrupper kanske fungerar bäst.

En grupp kan ha ett obegränsat antal användare.

Mer information om hur du skapar nya användare finns i [Lägg till användare](../../../administration-and-setup/add-users/add-users.md).

## Bevilja gruppåtkomst till objekt

När du delar ett objekt med en grupp har alla medlemmar i den gruppen (inklusive medlemmar i alla undergrupper) åtkomst till objektet. Mer information om delning i Workfront finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

## Associera en grupp med ett objekt

När du skapar eller redigerar något av följande Workfront-objekt kan du associera det med en grupp:

* **Projekt**: Du kan associera en enskild grupp med ett projekt för att ange ägarskap för projektet.

  Detta ger inte varje medlem i gruppen underförstådda rättigheter till projektet. För att ha rätt till projektet måste användarna ha projektet delat med sig.

  Även om användare kan vara medlemmar i flera grupper kan ett projekt ha en enda grupp kopplad till sig. Användare från andra grupper kan fortfarande arbeta med samma projekt, om projektet har delats med dem eller deras grupper. Gruppen som är associerad med projektet är vanligtvis antingen den grupp som ansvarar för att slutföra projektet eller den grupp som projektet levereras till.

  Instruktioner om hur du associerar ett projekt med en grupp finns i [Hantera information i projektöversiktsområdet](../../../manage-work/projects/manage-projects/understand-project-overview-area.md).

* **Portfolio, program eller företag**: När du skapar eller redigerar en portfölj, ett program eller ett företag kan du tilldela en enskild grupp till den för att ange att gruppen äger eller har ansvar för den. Med den här föreningen kan administratörer och användare enkelt identifiera vilka portföljer, program och företag deras grupper arbetar med.

  En gruppadministratör kan till exempel lista alla portföljer i organisationen med hjälp av en lista eller rapport och anteckningar i gruppkolumnen som portföljer tilldelas sin grupp.

  >[!NOTE]
  >
  >Att en grupp tilldelas en portfölj, ett program eller ett företag med en grupp innebär inte automatiskt att informationen i gruppen har tillgång till dess data. Du måste dela åtkomst till data manuellt med gruppen innan de kan se den.

  Instruktioner finns i [Skapa en portfölj](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md), [Skapa ett program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md) och [Skapa och redigera företag](../../../administration-and-setup/set-up-workfront/organizational-setup/create-and-edit-companies.md).

* **Godkännandeprocess**: Du kan göra en godkännandeprocess tillgänglig för projekt, aktiviteter och ärenden som tillhör en viss grupp. Mer information finns i [Skapa en godkännandeprocess för arbetsobjekt](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-approval-processes.md).
* **Milstolpesökväg**: Du kan tillåta användare i vissa grupper att använda en milstolpesökväg med sina projekt. Mer information finns i [Skapa en milstolpe-sökväg](../../../administration-and-setup/customize-workfront/configure-approval-milestone-processes/create-milestone-path.md).
* **Layoutmall**: Du kan ge en grupps administratörer behörighet att ändra en layoutmall. Instruktioner finns i [Bevilja administrativ åtkomst för en layoutmall](../../../administration-and-setup/customize-workfront/use-layout-templates/grant-admin-access-layout-template.md).

* **Tidrapportprofil**: Du kan ge en grupps administratörer behörighet att ändra en tidrapportprofil. Mer information finns i [Skapa, redigera och tilldela tidrapportprofiler](../../../timesheets/create-and-manage-timesheets/create-timesheet-profiles.md).

* **Scheman**: Du kan ge en grupps administratörer behörighet att ändra ett schema. Mer information finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).
* **Team**: Du kan associera en grupp med ett team så att gruppadministratörerna och dess undergrupper kan visa och arbeta med dessa team från gruppområdet. Mer information finns i [Skapa ett team](../../../people-teams-and-groups/create-and-manage-teams/create-a-team.md) eller [Redigera teaminställningar](../../../people-teams-and-groups/create-and-manage-teams/edit-team-settings.md).
* **Mall**: Du kan tilldela en grupp till en projektmall. Detta kan hjälpa er att effektivisera projektskapandet och hjälpa er att enklare identifiera och rapportera om vilka grupper som äger vilka projektmallar. Mer information finns i avsnittet [Översikt](../../../manage-work/projects/create-and-manage-templates/edit-templates.md#overview) i artikeln [Redigera projektmallar](../../../manage-work/projects/create-and-manage-templates/edit-templates.md).

* **Nyligen borttagna och återställda objekt**: Du kan visa och hantera grupper med nyligen borttagna objekt. Mer information finns i [Visa och hantera nyligen borttagna objekt för en grupp](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-deleted-objects.md) och [Visa och hantera nyligen återställda objekt för en grupp](../../../administration-and-setup/manage-groups/work-with-group-objects/view-manage-groups-recently-restored-objects.md).
