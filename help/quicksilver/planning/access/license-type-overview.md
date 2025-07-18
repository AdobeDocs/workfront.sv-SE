---
title: Översikt över licenstyp vid användning av Adobe Workfront Planning
description: Din åtkomst till Adobe Workfront Planning beror på licenstypen, förutom dina behörigheter till objekt. Alla användare i organisationen har inte samma åtkomst och behörigheter för att använda Adobe Workfront Planning. I den här artikeln beskrivs de åtkomstnivåer som användare kan ha till Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '647'
ht-degree: 0%

---


# Översikt över licenstyper vid användning av Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->

{{planning-important-intro}}

Din Adobe Workfront-licenstyp fungerar tillsammans med dina Adobe Workfront Planning-behörigheter för att ge följande åtkomst:

* Visa, bidra till eller hantera arbetsytor eller posttyper
* Visa eller hantera vyer.

Mer information om behörigheter för objekt i Workfront Planning finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

Mer information om åtkomst till Workfront Planning finns i [Åtkomstöversikt för Adobe Planning](/help/quicksilver/planning/access/access-overview.md).

## Förhållandet mellan Workfront licenstyper och Workfront Planning permissions

Tabellen nedan beskriver förhållandet mellan licenstypen för en användare i Adobe Workfront och den behörighetsnivå som du kan ge dem till Adobe Workfront Planning-objekt baserat på den licensen.

Om du ger en användare behörighet till en arbetsyta får den även behörighet att spela in typer, poster och fält.

Du måste ge användarna separata behörigheter för vyer, utöver de som de har för arbetsytor, för att kunna komma åt och hantera vyer.

Tänk på följande när du arbetar med behörigheter för posttyper:

* Användare ärver automatiskt behörigheter för posttyp från arbetsytor.
* När en användare har behörigheten Hantera på en arbetsyta kan de inte ha en lägre åtkomst till en posttyp.
* Användare kan inte ha större behörighet för en posttyp än de har för arbetsytan som posttypen tillhör.
* Om du tar bort användarnas behörigheter till en posttyp tas inte deras visningsåtkomst bort till alla posttyper på arbetsytan, eftersom deras behörigheter inte tas bort från arbetsytan.

| Adobe Workfront licenstyp* | Högsta tillåtna behörighet i Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Standard | <p>Användare kan hantera arbetsytor, posttyper och vyer. De kan skapa, redigera och ta bort arbetsytor, posttyper, poster, fält och vyer.</p> <br> <p>Systemadministratörer har behörigheten Hantera för alla arbetsytor, inklusive de som de inte skapade.</p> |
| Ljus eller Medarbetare | <p>Användarna kan visa de arbetsytor som delas med dem samt posttyper, poster och fält för dessa arbetsytor.</p> <br> <p>Användarna kan visa de vyer som delas med dem, men de kan inte skapa egna. </p><br> <p>Användare kan inte skapa, redigera eller ta bort arbetsytor, posttyper, poster eller fält.</p> |

*Workfront Planning finns inte för tidigare Workfront-licenser.
Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).


### Licenstyper och behörigheter till arbetsytor och posttyper

Endast användare med en standardlicens kan ha Contribute- eller Hantera-behörigheter för arbetsytor och posttyper. Behörigheterna Contribute och Hantera för arbetsytor och posttyper överförs också till poster och fält.

Användare med alla andra licenstyper kan ha behörigheten Visa på arbetsytor och posttyper som delas med dem, samt till poster och fält.

Systemadministratörer kan visa alla arbetsytor i systemet, inklusive de som de inte skapade.

>[!INFO]
>
>**EXEMPEL:**
>
>Medarbetare eller användare med ljuslicens kan inte bidra till eller hantera arbetsytor och deras objekt.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att bidra till eller hantera en arbetsyta när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
>![Behörigheter är nedtonade för medverkande användare på arbetsytan](assets/permissions-grayed-out-for-contributor-user-on-workspace.png)


### Licenstyper och behörigheter till vyer

Endast användare med en standardlicens kan ha behörigheten Hantera för att visa. Användare med alla andra licenstyper kan ha behörigheten Visa för vyer som delas med dem.

>[!INFO]
>
>**EXEMPEL:**
>
>Medarbetare eller användare med ljuslicens kan inte hantera vyer. De kan använda temporära filter, sorteringar eller grupperingar för vyer som de har åtkomst till.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att hantera en vy när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
>![Behörigheterna är nedtonade för ljusa användare på visningsresursen](assets/permissions-grayed-out-for-light-user.png)
