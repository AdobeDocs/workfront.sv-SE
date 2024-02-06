---
title: Översikt över delningsbehörigheter i Adobe Maestro
description: Du kan dela eller ta bort behörigheter till en Adobe Maestro-arbetsyta eller -vy.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 08a7fa1f3871494c4c6b0c385a98a64735b7f7e4
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Maestro. This article describes the levels of access that users could have to Adobe Maestro. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Översikt över delningsbehörigheter i Adobe Maestro

{{maestro-important-intro}}

Du kan dela eller ta bort behörigheter till en Adobe Maestro-arbetsyta eller -vy.

I den här artikeln beskrivs behörighetsnivåerna för Maestro-objekt.

Mer information om hur du delar arbetsytor och vyer finns i följande artiklar:

* [Dela arbetsytor](/help/quicksilver/maestro/access/share-workspaces.md)

* [Visa](/help/quicksilver/maestro/access/share-views.md)

## Objekt som du kan dela i Adobe Maestro

Du kan dela följande objekt i Maestro:

* Arbetsytor

  När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna. Vyer delas inte.

* Vyer

## Att tänka på när du delar objekt i Maestro

* Din Adobe Workfront-licenstyp fungerar tillsammans med dina Maestro-behörigheter så att du kan visa, bidra och hantera Maestro-objekt.

  Mer information om hur licenstyper påverkar behörighetsnivåer för Maestro-objekt finns i [Översikt över licenstypen i Adobe Maestro](/help/quicksilver/maestro/access/license-type-overview.md).
* Systemadministratörer kan hantera och dela arbetsytor som andra användare har skapat.
* Om du inte är systemadministratör kan du bidra till arbetsytor som skapats av andra om de delas med dig.
* Du kan inte dela flera arbetsytor samtidigt.
* Du kan dela en arbetsyta med följande enheter:
   * Användare
   * Grupper
* Andra användare, inklusive systemadministratörer, kan bara komma åt vyer som de har skapat eller som har delats med dem.
* Du kan dela en länk till en arbetsyta eller till en vy från en posttypssida med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan eller posttypssidan som visas i den valda vyn.

## Delningsbehörigheter för Maestro-objekt

Tabellerna i följande avsnitt visar vilken behörighetsnivå du kan välja när du delar en maestro-arbetsyta eller -vy och vilka funktioner varje nivå tillåter.

>[!IMPORTANT]
>
>Alla användare kan inte ha de behörighetsnivåer som beskrivs nedan. Användarens individuella licens avgör vilken behörighetsnivå de kan få för Maestro-objekt.
>
>Mer information finns i [Översikt över licenstypen i Adobe Maestro](/help/quicksilver/maestro/access/license-type-overview.md).


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






