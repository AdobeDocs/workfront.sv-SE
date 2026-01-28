---
user-type: administrator
content-type: reference
product-area: system-administration
navigation-topic: access-levels
title: Åtkomst till objekt och områden via licenser
description: Tabellen nedan visar den högsta åtkomstnivån (Redigera eller Visa) som var och en av Adobe Workfront-licenserna tillåter för objekten och områdena i Workfront.
author: Becky
feature: System Setup and Administration
role: Admin
exl-id: 87fb5673-6e36-4182-958a-d69a56fe7b68
source-git-commit: 0ccf02a333b41705a582bcb10ab9a90198123997
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Tillgång till objekt och områden med hjälp av licenser

<!-- Audited: 2/2024 -->

>[!NOTE]
>
>Informationen i den här artikeln hänvisar till de aktuella åtkomstnivåerna. Mer information om de äldre åtkomstnivåerna finns i [Översikt över åtkomstnivåer](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).

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
        <td>Redigera**</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Uppgifter</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Problem</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Redigera</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Portföljer</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa</td>
        <td>Ingen åtkomst</td>
    </tr>
    <tr>
        <td>Program</td>
        <td>Redigera</td>
        <td>Visa</td>
        <td>Visa</td>
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

&#42;-användare med en Contributor-licens kan bara visa rapporter, instrumentpaneler och kalendrar som delas med dem.

&#42;&#42; Användare med en Light-licens kan bara logga tid på projektnivå när Redigera-åtkomst är aktiverat. De kan inte skapa, redigera, ta bort eller dela projekt. Standardåtkomstnivån för projekt för ljusa användare är Visa.

>[!NOTE]
>
>* Användare med en Light-licens eller en Contributor-licens har begränsade delningsmöjligheter. Mer information finns i [Licensöversikt](/help/quicksilver/administration-and-setup/add-users/how-access-levels-work/licenses-overview.md).
>
>* Externa användare kan inte söka efter objekt i Workfront. De kan visa dokument och kalendrar som delas med dem. De kan också se vilka användare som delar objekt med dem.
>
>* Contributor-användare och externa användare kan inte se innehåll som är delat i hela systemet.  Den måste delas med dem uttryckligen.

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
