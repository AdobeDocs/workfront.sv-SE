---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Tillgång till objekt och områden med nya licenser
description: Tabellen nedan visar den högsta åtkomstnivån (Redigera eller Visa) som var och en av Adobe Workfront-licenserna tillåter för objekten och områdena i Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 7a9232f59e4c6f2eac2995be7d7862295b6bab2c
workflow-type: tm+mt
source-wordcount: '397'
ht-degree: 0%

---

# Tillgång till objekt och områden med nya licenser

<!-- Audited: 2/2024 -->

Tabellen nedan visar den högsta åtkomstnivån (Redigera eller Visa) som var och en av Adobe Workfront-licenserna tillåter för objekten och områdena i Workfront.

* **Visa**: Användaren kan granska och dela objekt.
* **Redigera**: Användaren kan skapa, redigera, ta bort och dela objekt.

  >[!NOTE]
  >
  >När en annan användare delar ett objekt kan användaren ange behörigheter som begränsar möjligheten att redigera det. Mer information finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

<table style="table-layout:auto">
    <tr>
        <td></td>
        <td>Standard</td>
        <td>Ljus</td>
        <td>Medarbetare</td>
        <td>Extern</td>
    </tr>
    <tr>
        <td>Projekt</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa (endast detaljsidan)</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Uppgifter</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa</td>
        <td>Visa</td>
    </tr>
    <tr>
        <td>Problem</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Portfolio</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Program</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Rapporter, kontrollpaneler och kalendrar</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa*</td>
        <td>Visa (endast för kalendrar, inga delningsbehörigheter)</td>
    </tr>
    <tr>
        <td>Filter, vyer och grupperingar</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Dokument</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Visa (inga delningsbehörigheter)</td>
    </tr>
    <tr>
        <td>Användare</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa</td>
        <td>Visa</td>
    </tr>
    <tr>
        <td>Team</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Mallar</td>
        <td>Redigera</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Finansiella uppgifter</td>
        <td>Redigera</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Resurshantering</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Scenarioplan</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Workfront-mål</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Ingen åtkomst</td>
    </tr>
</table>

&#42; Användare med en Contributor-licens kan endast visa rapporter, instrumentpaneler och kalendrar som delas med dem.

>[!NOTE]
>
>Användare med en Light-licens eller en Contributor-licens har begränsade delningsmöjligheter. Mer information finns i [Översikt över licenser](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>Externa användare kan inte söka efter objekt i Workfront. De kan visa dokument och kalendrar som delas med dem. De kan också se vilka användare som delar objekt med dem.

Du hittar detaljerad information om vilka åtkomstnivåer som tillåts för varje objekt och område i följande artiklar:

* [Bevilja åtkomst till projekt](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Bevilja åtkomst till uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Bevilja åtkomst till utleveranser](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Bevilja åtkomst till dokument](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Bevilja åtkomst till portföljer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Bevilja åtkomst till program](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Ge åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Bevilja åtkomst till filter, vyer och grupperingar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Bevilja åtkomst för användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Bevilja åtkomst för team](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Bevilja åtkomst till mallar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Bevilja åtkomst till finansiella uppgifter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Bevilja åtkomst till resurshantering](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Bevilja åtkomst till scenarioplan](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Ge åtkomst till Adobe Workfront mål](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
