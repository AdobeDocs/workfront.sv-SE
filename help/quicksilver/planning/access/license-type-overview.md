---
title: Översikt över licenstyp vid användning av Adobe Workfront Planning
description: Din åtkomst till Adobe Workfront Planning beror på licenstypen, förutom dina behörigheter till objekt. Alla användare i organisationen har inte samma åtkomst och behörigheter för att använda Adobe Workfront Planning. I den här artikeln beskrivs de åtkomstnivåer som användare kan ha till Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: cf3b5d3f8e3a8a1922da757a41b4c5e0ee84e6fd
workflow-type: tm+mt
source-wordcount: '564'
ht-degree: 0%

---


# Översikt över licenstyper vid användning av Adobe Workfront Planning

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

{{planning-important-intro}}

Din Adobe Workfront-licenstyp fungerar tillsammans med dina Adobe Workfront Planning-behörigheter för att ge följande åtkomst:

* Visa, bidra till eller hantera arbetsytor
* Visa eller hantera vyer.

Mer information om behörigheter för objekt i Workfront Planning finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Mer information om åtkomst till Workfront Planning finns i [Åtkomstöversikt för Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Förhållandet mellan Workfront licenstyper och Workfront Planning permissions

Tabellen nedan beskriver förhållandet mellan licenstypen för en användare i Adobe Workfront och den behörighetsnivå som du kan ge dem till Adobe Workfront Planning-objekt baserat på den licensen.

Om du ger en användare behörighet till en arbetsyta får den även behörighet att spela in typer, poster och fält.

Du måste ge användarna separata behörigheter för vyer, utöver de som de har för arbetsytor, för att kunna komma åt och hantera vyer.

| Adobe Workfront licenstyp* | Högsta tillåtna behörighet i Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Användare kan hantera arbetsytor och vyer. De kan skapa, redigera och ta bort arbetsytor, posttyper, poster, fält och vyer.</p> <br> <p>Systemadministratörer har behörigheten Hantera för alla arbetsytor, inklusive de som de inte skapade.</p> |
| Ljus eller Medarbetare | <p>Användarna kan visa de arbetsytor som delas med dem samt posttyper, poster och fält för dessa arbetsytor.</p> <br> <p>Användarna kan visa de vyer som delas med dem, men de kan inte skapa egna. </p><br> <p>Användare kan inte skapa, redigera eller ta bort arbetsytor, posttyper, poster eller fält.</p> |

*Workfront Planning finns inte för tidigare Workfront-licenser.
Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


<!--OLD 

| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | Users can manage workspaces. They can create, edit, or delete workspaces, record types, records, and fields. <br> System administrators have Manage permissions to all workspaces, including the ones they did not create.                                                                                                                     |
| New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces. <br> Users cannot create, edit, or delete workspaces, record types, records, or fields.|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
-->

### Licenstyper och behörigheter för arbetsytan

Endast användare med en standardlicens kan ha Contribute- eller Manage-behörighet till arbetsytor. Användare med alla andra licenstyper kan ha behörigheten Visa på arbetsytor som delas med dem.

Systemadministratörer kan visa alla arbetsytor i systemet, även de som de inte skapade.

>[!INFO]
>
>**EXEMPEL:**
>
>Medarbetare eller användare med ljuslicens kan inte bidra till eller hantera arbetsytor och deras objekt.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att bidra till eller hantera en arbetsyta när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
><span class="preview">![](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)</span>


### Licenstyper och visningsbehörigheter

Endast användare med en standardlicens kan ha behörigheten Hantera för att visa. Användare med alla andra licenstyper kan ha behörigheten Visa för vyer som delas med dem.

>[!INFO]
>
>**EXEMPEL:**
>
>Medarbetare eller användare med ljuslicens kan inte hantera vyer. De kan använda temporära filter, sorteringar eller grupperingar för vyer som de har åtkomst till.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att hantera en vy när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
><span class="preview">![](assets/permissions-grayed-out-for-light-user.png)</span>
