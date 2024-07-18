---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Åtkomst till objekt och områden per licenstyp
description: Tabellen nedan visar den högsta åtkomstnivån (Redigera eller Visa) som var och en av Adobe Workfront-licenserna tillåter för objekten och områdena i Workfront.
author: Courtney
feature: System Setup and Administration
role: Admin
exl-id: d8f2a295-c053-4763-bf6e-6e836087a839
source-git-commit: 880e82546ac0ca80be60f03db31b99ad1778c35a
workflow-type: tm+mt
source-wordcount: '425'
ht-degree: 0%

---

# Åtkomst till objekt och områden per licenstyp

Tabellen nedan visar den högsta åtkomstnivån (Redigera eller Visa) som var och en av Adobe Workfront-licenserna tillåter för objekten och områdena i Workfront.

* **Visa**: Användaren kan granska och dela objekt.
* **Redigera**: Användaren kan skapa, redigera, ta bort och dela objekt.

  >[!NOTE]
  >
  >När en annan användare delar ett objekt kan användaren ange behörigheter som begränsar möjligheten att redigera det. Mer information finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

|   | Plan | Arbete | Granska | Begäran | Extern |
|---|---|---|---|---|---|
| Projekt | Redigera | Redigera (utan behörighet att skapa) | Visa | Visa (endast detaljsidan) | Ingen åtkomst |
| Uppgifter | Redigera | Redigera | Visa | Visa | Visa |
| Problem | Redigera | Redigera | Redigera | Redigera | Ingen åtkomst |
| Portfolio | Redigera | Visa | Visa | Ingen åtkomst | Ingen åtkomst |
| Program | Redigera | Visa | Visa | Ingen åtkomst | Ingen åtkomst |
| Rapporter, kontrollpaneler och kalendrar | Redigera | Visa | Visa | Visa&#42; | Visa (endast för kalendrar, inga delningsbehörigheter) |
| Filter, vyer och grupperingar | Redigera | Redigera | Redigera | Redigera | Ingen åtkomst |
| Dokument | Redigera | Redigera | Redigera | Redigera | Visa (inga delningsbehörigheter) |
| Användare | Redigera | Visa | Visa | Visa | Visa |
| Team | Redigera | Redigera | Visa | Visa | Ingen åtkomst |
| Mallar | Redigera | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst | Ingen åtkomst |
| Finansiella uppgifter | Redigera | Visa (endast området Ekonomi i Projektinformation) | Visa | Ingen åtkomst | Ingen åtkomst |
| Resurshantering | Redigera | Visa | Visa | Ingen åtkomst | Ingen åtkomst |
| Scenarioplan | Redigera | Redigera | Redigera | Ingen åtkomst | Ingen åtkomst |
| Workfront-mål | Redigera | Redigera | Redigera | Redigera | Ingen åtkomst |

&#42; Användare med en begärandelicens kan endast visa rapporter, instrumentpaneler och kalendrar som delas med dem.

>[!NOTE]
>
>Användare med en Review-licens eller en Request-licens har begränsade delningsmöjligheter. Mer information finns i [Översikt över Adobe Workfront-licenser](../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md).
>
>Externa användare kan inte söka efter objekt i Workfront. De kan visa dokument och kalendrar som delas med dem. De kan också se vilka användare som delar objekt med dem.

Du hittar detaljerad information om vilka åtkomstnivåer som tillåts för varje objekt och område i följande artiklar:

* [Bevilja åtkomst till projekt](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-projects.md)
* [Bevilja åtkomst till aktiviteter](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-tasks.md)
* [Bevilja åtkomst till utgåvor](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-issues.md)
* [Bevilja åtkomst till dokument](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-documents.md)
* [Bevilja åtkomst till portföljer](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-portfolios.md)
* [Bevilja åtkomst till program](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-programs.md)
* [Bevilja åtkomst till rapporter, instrumentpaneler och kalendrar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-reports-dashboards-calendars.md)
* [Bevilja åtkomst till filter, vyer och grupperingar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-fvg.md)
* [Bevilja åtkomst till användare](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-other-users.md)
* [Bevilja åtkomst för team](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-teams.md)
* [Bevilja åtkomst till mallar](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-templates.md)
* [Bevilja åtkomst till ekonomiska data](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md)
* [Bevilja åtkomst till resurshantering](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md)
* [Bevilja åtkomst till scenarioplan](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md)
* [Ge åtkomst till Adobe Workfront mål](../../../administration-and-setup/add-users/configure-and-grant-access/grant-access-goals.md)
