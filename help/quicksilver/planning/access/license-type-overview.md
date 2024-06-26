---
title: Översikt över licenstyper vid användning av Adobe Workfront Planning
description: Din åtkomst till Adobe Workfront Planning beror på licenstypen, förutom dina behörigheter till objekt.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 99b8d6371a718b7268edfda81959ae3170d1962b
workflow-type: tm+mt
source-wordcount: '353'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Översikt över licenstyper vid användning av Adobe Workfront Planning

{{planning-important-intro}}

Din Adobe Workfront-licenstyp fungerar tillsammans med dina Adobe Workfront Planning-behörigheter så att du kan visa, bidra och hantera arbetsytor. <!--add more objects here when we can grant other object-specific permissions-->

Workfront Planning-behörigheter för att spela in vyer är oberoende av Workfront licenstyper.

Användare med alla licenstyper kan visa, skapa, redigera och hantera Workfront Planning-vyer.

I den här artikeln beskrivs vilka typer av licenser som behövs i Workfront och vilka behörigheter som ges till arbetsytor i Workfront Planning baserat på respektive licenstyp.

En användare med en lägre licenstyp har begränsade behörigheter till arbetsytor när de använder Workfront Planning-funktioner.

>[!INFO]
>
>**EXEMPEL:**
>
>Beställare (eller medarbetare, enligt den nya licensmodellen) kan inte bidra till eller hantera arbetsytor och deras objekt.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att bidra till eller hantera en arbetsyta när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)


Information om behörigheter för objekt i Workfront Planning finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Förhållandet mellan Workfront licenstyper och Workfront Planning permissions

Tabellen nedan beskriver förhållandet mellan licenstypen för en användare i Adobe Workfront och den behörighetsnivå som du kan ge dem till Adobe Workfront Planning-objekt baserat på den licensen.

Om du ger en användare behörighet till en arbetsyta får den även behörighet att spela in typer, poster och fält.


| Adobe Workfront licenstyp* | Högsta tillåtna behörighet i Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nytt: Standard <br> eller <br>Aktuell: Planera | Användare kan hantera arbetsytor. De kan skapa, redigera och ta bort arbetsytor, posttyper, poster och fält. <br> Systemadministratörer har behörigheten Hantera för alla arbetsytor, inklusive de som de inte skapade. |
| Nytt: Ljus, Medarbetare <br> eller <br>Aktuell: Arbete, begärande, granskare | Användarna kan visa de arbetsytor som delas med dem samt posttyper, poster och fält för dessa arbetsytor. <br> Användare kan inte skapa, redigera eller ta bort arbetsytor, posttyper, poster eller fält. |

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).