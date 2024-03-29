---
title: Översikt över delningsbehörigheter i Adobe Workfront-planeringen
description: Du kan dela eller ta bort behörigheter till en planeringsarbetsyta eller vy i Adobe Workfront.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 130365bfa220337aa25f27ba03742ea3471972cb
workflow-type: tm+mt
source-wordcount: '531'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront planning. This article describes the levels of access that users could have to Adobe Workfront planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Översikt över delningsbehörigheter i Adobe Workfront-planeringen

{{maestro-important-intro}}

Du kan dela eller ta bort behörigheter till en arbetsyta eller vy i Adobe Workfront-planeringen.

I den här artikeln beskrivs behörighetsnivåerna för Workfront planeringsobjekt.

Mer information om hur du delar arbetsytor och vyer finns i följande artiklar:

* [Dela arbetsytor](/help/quicksilver/maestro/access/share-workspaces.md)

* [Visa](/help/quicksilver/maestro/access/share-views.md)

## Objekt som du kan dela i Adobe Workfront-planeringen

Du kan dela följande objekt:

* Arbetsytor

  När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna. Vyer delas inte.

* Vyer

## Att tänka på vid delning av objekt i Adobe Workfront-planering

* Din Adobe Workfront-licenstyp fungerar tillsammans med dina planeringsbehörigheter i Workfront så att du kan visa, bidra till eller hantera objekt när du använder Workfront-planering.

  Mer information om hur licenstyper påverkar behörighetsnivåer för Workfront-planering finns i [Översikt över licenstyp vid användning av Adobe Workfront-planering](/help/quicksilver/maestro/access/license-type-overview.md).
* Systemadministratörer kan hantera och dela arbetsytor som andra användare har skapat.
* Om du inte är systemadministratör kan du bidra till arbetsytor som skapats av andra om de delas med dig.
* Du kan inte dela flera arbetsytor samtidigt.
* Du kan dela en arbetsyta eller vy med följande enheter:
   * Användare
   * Grupper
* Andra användare, inklusive systemadministratörer, kan bara komma åt vyer som de har skapat eller som har delats med dem. Systemadministratörer kan bara ges behörighet att hantera en vy.
* Du kan dela en länk till en arbetsyta eller till en vy från en posttypssida med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan eller posttypssidan som visas i den valda vyn.

## Delningsbehörigheter för Adobe Workfront planeringsobjekt

Tabellerna i följande avsnitt visar vilken behörighetsnivå du kan välja när du delar en arbetsyta eller vy och vilka funktioner varje nivå tillåter.

>[!IMPORTANT]
>
>Alla användare kan inte ha de behörighetsnivåer som beskrivs nedan. Användarens individuella licens avgör vilken behörighetsnivå de kan få för Workfront planeringsobjekt.
>
>Mer information finns i [Översikt över licenstyp vid användning av Adobe Workfront-planering](/help/quicksilver/maestro/access/license-type-overview.md).


### Behörigheter för arbetsytan

|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Redigera | ✓ |            |       |
| Dela | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |

### Posttypbehörigheter

Posttypsbehörigheter ärvs när du ger behörighet till arbetsytan.

|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Redigera | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |

### Spela in behörigheter

Postbehörigheter ärvs när du ger behörighet till arbetsytan.

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

|        | Hantera | Visa |
|--------|--------|-------|
| Redigera | ✓ |       |
| Ta bort | ✓ |       |
| Visa | ✓ | ✓ |
| Använd | ✓ | ✓ |
