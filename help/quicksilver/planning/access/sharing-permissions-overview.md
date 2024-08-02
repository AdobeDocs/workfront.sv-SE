---
title: Översikt över delningsbehörigheter i Adobe Workfront Planning
description: Du kan dela eller ta bort behörigheter till en Adobe Workfront Planning-arbetsyta eller -vy.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 1ffd8a3dbb31154186dc37132c7e77c35de42ac3
workflow-type: tm+mt
source-wordcount: '800'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Översikt över delningsbehörigheter i Adobe Workfront Planning

{{planning-important-intro}}

Du kan dela eller ta bort behörigheter till en arbetsyta eller vy i Adobe Workfront Planning.

I den här artikeln beskrivs behörighetsnivåerna för Workfront Planning-objekt.

Mer information om hur du delar arbetsytor och vyer finns i följande artiklar:

* [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)

* [Visa](/help/quicksilver/planning/access/share-views.md)

## Objekt som du kan dela i Adobe Workfront Planning

Du kan dela följande objekt:

* Arbetsytor

   * Du kan dela arbetsytor med personer i din organisation.
   * När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna. Vyer delas inte.

* Vyer

   * Du måste ge användare, inklusive systemadministratörer, behörighet att komma åt vyer separat från deras behörigheter till att komma åt arbetsytor.
   * Du kan dela en vy offentligt med personer utanför organisationen när du genererar en offentlig länk för en vy.Personer som öppnar postsidan från en offentlig länk kan visa alla poster och deras fält, inklusive anslutna poster och fält.

  Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

Internt kan du dela en arbetsyta eller vy med följande Workfront-enheter:

* Användare
* Grupper

## Att tänka på när du delar objekt i Adobe Workfront Planning

* Din Adobe Workfront-licenstyp fungerar tillsammans med dina Workfront Planning-behörigheter så att du kan visa, bidra till eller hantera arbetsytor och deras objekt.

  Mer information om hur licenstyperna påverkar behörighetsnivåer för Workfront Planning finns i [Översikt över licenstypen när du använder Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Systemadministratörer kan hantera alla arbetsytor i systemet, inklusive de som de inte skapade.
* Andra användare, inklusive systemadministratörer, kan bara komma åt vyer som de har skapat eller som har delats med dem. Systemadministratörer kan endast ges behörighet för att hantera en vy.
* Du kan dela en länk till en arbetsyta eller till en vy med andra.

  Följande scenarier finns:
   * Användare som får länken till en arbetsyta måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan.
   * Användare som får länken till en vy kan komma åt vyn på följande sätt:

      * Måste vara aktiva användare och logga in på Workfront om länken till vyn delades internt.
      * Kan vara externa användare till Workfront och få åtkomst till vyn via en offentlig delad länk, utan att logga in på Workfront.

## Delningsbehörigheter för Adobe Workfront Planning-objekt

Tabellerna i följande avsnitt visar vilken behörighetsnivå du kan välja när du delar en arbetsyta eller vy och vilka funktioner varje nivå tillåter.

>[!IMPORTANT]
>
>Alla användare kan inte ha de behörighetsnivåer som beskrivs nedan. Användarens individuella licens avgör vilken behörighetsnivå de kan få för Workfront Planning-objekt.
>
>Endast användare med standardlicens (eller standardlicens) kan ha Contribute- eller Hantera-behörighet till arbetsytor och Hantera-behörighet till vyer.
> 
>Användare med alla andra licenstyper kan ha behörigheten Visa på arbetsytor och vyer.
>
>Mer information finns i [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Workspace-behörigheter

Du måste ge användarna behörighet till arbetsytor för att de ska kunna få åtkomst till följande enheter:

* Arbetsytor
* Posttyper
* Poster
* Fält

Följande behörighetsnivåer gäller för arbetsytor:

|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Redigera | ✓ |            |       |
| Dela | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |

### Posttypbehörigheter

Posttypsbehörigheter ärvs när du ger behörighet till arbetsytan.

Följande behörighetsnivåer gäller för posttyper:


|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Redigera | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |

### Spela in behörigheter

Postbehörigheter ärvs när du ger behörighet till arbetsytan.

Följande behörighetsnivåer gäller för poster:


|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ | ✓ |       |
| Redigera | ✓ | ✓ |       |
| Visa | ✓ | ✓ | ✓ |

### Fältbehörigheter

Fältbehörigheter ärvs när du ger behörighet till arbetsytan.
Följande behörigheter refererar till själva fälten och inte till värdena som associeras med varje fält. Om du vill redigera fältvärden måste du ha behörighet att redigera poster.

|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Redigera | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |


### Visa behörigheter

Du måste tilldela separata behörigheter för att spela in vyer. Om du ger behörighet till arbetsytan ges inte behörighet till postvyerna på arbetsytan.

Du måste ge användarna behörighet att visa vyer för att de ska ha tillgång till följande vyelement:

* Filter
* Fältsynlighet
* Sortera
* Gruppering
* Radhöjd
* Inställningar

Du kan dela vyer internt eller offentligt.

Följande behörighetsnivåer gäller för vyer och visningselement:

| Intern delning | Hantera (Endast inbjudna personer kan komma åt) | Visa (Endast inbjudna personer kan komma åt) | Alla på arbetsytan kan visa* |
|--------|--------|-------|------------------------------|
| Redigera | ✓ |       |                            |
| Ta bort | ✓ |       |                            |
| Dela | ✓ |       |                           |
| Visa | ✓ | ✓ | ✓ |
| Använd | ✓ | ✓ | ✓ |

| Offentlig delning | Visa |
|--------|-------|
| Visa | ✓ |
| Använd | ✓ |

*Användarna måste ha behörigheten Visa eller högre för en arbetsyta för att få åtkomst till vyn.



<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |  


|        | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Access the view  | ✓      | ✓     | ✓                          |
| Apply temporary filters, groupings, sort  | ✓      | ✓     | ✓                          |
-->