---
title: Översikt över licenstyper vid användning av Adobe Workfront Planning
description: Din åtkomst till Adobe Workfront Planning beror på licenstypen, förutom dina behörigheter till objekt.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
exl-id: 10dee6f9-06ff-435a-81a4-2125642fab59
source-git-commit: 402fb9d279fec258390535100e8f3d2c3c1b913b
workflow-type: tm+mt
source-wordcount: '428'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront plannint. This article describes the levels of access that users could have to Adobe Workfront Planning. -->
<!--update the title and the metadata title if Workfront Planning is NOT its own product - because the title is too generic for it being a Workfront capability-->

# Översikt över licenstyper vid användning av Adobe Workfront Planning

{{planning-important-intro}}

Din Adobe Workfront-licenstyp fungerar tillsammans med dina Adobe Workfront Planning-behörigheter för att ge följande åtkomst:

* Visa, bidra till eller hantera arbetsytor
* Visa eller hantera vyer.

Information om behörigheter för objekt i Workfront Planning finns i [Översikt över delningsbehörigheter i Adobe Workfront Planning](/help/quicksilver/planning/access/sharing-permissions-overview.md).

## Förhållandet mellan Workfront licenstyper och Workfront Planning permissions

Tabellen nedan beskriver förhållandet mellan licenstypen för en användare i Adobe Workfront och den behörighetsnivå som du kan ge dem till Adobe Workfront Planning-objekt baserat på den licensen.

Om du ger en användare behörighet till en arbetsyta får den även behörighet att spela in typer, poster och fält.


| Adobe Workfront licenstyp* | Högsta tillåtna behörighet i Adobe Workfront Planning |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
| Nytt: Standard <br> eller <br>Aktuell: Planera | Användare kan hantera arbetsytor. De kan skapa, redigera och ta bort arbetsytor, posttyper, poster och fält. <br> Systemadministratörer har behörigheten Hantera för alla arbetsytor, inklusive de som de inte skapade. |
| Nytt: Ljus, Medarbetare <br> eller <br>Aktuell: Arbete, begärande, granskare | Användarna kan visa de arbetsytor som delas med dem samt posttyper, poster och fält för dessa arbetsytor. <br> Användare kan inte skapa, redigera eller ta bort arbetsytor, posttyper, poster eller fält. |

*Mer information finns på [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

### Licenstyper och behörigheter för arbetsytan

Endast användare med en standardlicens (eller en planlicens) kan ha Contribute- eller Hantera-behörigheter för arbetsytor. Användare med alla andra licenstyper kan ha behörigheten Visa på arbetsytor som delas med dem.

Systemadministratörer kan visa alla arbetsytor i systemet, även de som de inte skapade.

>[!INFO]
>
>**EXEMPEL:**
>
>Beställare (eller medarbetare, enligt den nya licensmodellen) kan inte bidra till eller hantera arbetsytor och deras objekt.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att bidra till eller hantera en arbetsyta när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
>![](assets/permissions-grayed-out-for-requestor-user.png)

### Licenstyper och visningsbehörigheter

Endast användare med en standardlicens (eller en planlicens) kan ha behörigheten Hantera för att visa. Användare med alla andra licenstyper kan ha behörigheten Visa för vyer som delas med dem.

>[!INFO]
>
>**EXEMPEL:**
>
>Medarbetare (eller beställare och granskare) kan inte hantera vyer. De kan använda temporära filter, sorteringar eller grupperingar för vyer som de har åtkomst till.
>
>Det finns en indikation i delningsrutan om att användare inte kan beviljas behörighet att hantera en vy när de har en licens på lägre nivå, eftersom dessa behörighetsnivåer är nedtonade.
>
>![](assets/permissions-grayed-out-for-reviewer-user-on-a-view.png)


<!--Replace all of the above with this:

The table below describes the relationship between the license type of a user in Adobe Workfront and the level of permissions you can grant to them to Adobe Workfront Planning objects based on that license. 

Granting a user permissions to a workspace also grants them permissions to record types, records, and fields. 

You must grant view permissions separately from workspace permissions. 


| Adobe Workfront license type*                                   | Highest permissions allowed in Adobe Workfront Planning                                                                                                                                             |
|------------------------------------------------|-------------------------------------------------------------------------------------------------------------------------------------------------------------------------------|
|New: Standard <br> or <br>Current: Plan                    | <ul><li>Users can contribute to or manage workspaces and they can manage views. They can create, edit, or delete workspaces, record types, records, fields, and views.</li> <li> System administrators have Manage permissions to all workspaces, including the ones they did not create.</li> <li> System administrators can only access views they created.</li></ul>                                                                                                                     |
|New: Light, Contributor <br> or <br>Current: Work, Requestor, Reviewer                      | <ul><li>Users can view the workspaces shared with them, as well as the record types, records, and fields of those workspaces.</li> <li>Users can access views shared with them and apply temporary filters, sorts, or groupings, but they cannot modify the views. </li><li> Users cannot create, edit, or delete workspaces, record types, records, fields, or views.</li></ul>|

*For more information, see [Access requirements in Workfront documentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md). 

-->