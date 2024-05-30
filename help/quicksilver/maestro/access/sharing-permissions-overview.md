---
title: Översikt över delningsbehörigheter i Adobe Workfront Planning
description: Du kan dela eller ta bort behörigheter till en Adobe Workfront Planning-arbetsyta eller -vy.
hidefromtoc: true
hide: true
recommendations: noDisplay, noCatalog
el-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 5d7a7157c7ffb9634ec44de0b55b3bcf08d88786
workflow-type: tm+mt
source-wordcount: '696'
ht-degree: 0%

---

<!--update the metadata with real things when making this public; also update the description with something like this: Not all users in the organization have the same access and permissions to use Adobe Workfront Planning. This article describes the levels of access that users could have to Adobe Workfront Planning. -->

<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

# Översikt över delningsbehörigheter i Adobe Workfront Planning

{{planning-important-intro}}

Du kan dela eller ta bort behörigheter till en arbetsyta eller vy i Adobe Workfront Planning.

I den här artikeln beskrivs behörighetsnivåerna för Workfront Planning-objekt.

Mer information om hur du delar arbetsytor och vyer finns i följande artiklar:

* [Dela arbetsytor](/help/quicksilver/maestro/access/share-workspaces.md)

* [Visa](/help/quicksilver/maestro/access/share-views.md)

## Objekt som du kan dela i Adobe Workfront Planning

Du kan dela följande objekt:

* Arbetsytor

  När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna. Vyer delas inte.

* Vyer

## Att tänka på när du delar objekt i Adobe Workfront Planning

* Din Adobe Workfront-licenstyp fungerar tillsammans med dina Workfront Planning-behörigheter så att du kan visa, bidra och hantera objekt när du använder Workfront Planning.

  Information om hur licenstyper påverkar behörighetsnivåer för Workfront Planning finns i [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).
* Systemadministratörer kan hantera och dela arbetsytor som andra användare har skapat.
* Om du inte är systemadministratör kan du bidra till arbetsytor som skapats av andra om de delas med dig.
* Du kan inte dela arbetsytor eller vyer i grupp.
* Du kan dela en arbetsyta eller vy med följande enheter:
   * Användare
   * Grupper
     <!--* You can share a view publicly, with people outside your organization when you generate a public link for a view.People accessing the record page from a public link can view all records and their fields, including connected records and fields.-->
* Andra användare, inklusive systemadministratörer, kan bara komma åt vyer som de har skapat eller som har delats med dem. Systemadministratörer kan bara ges behörighet att hantera en vy.
* Du kan dela en länk till en arbetsyta eller till en vy från en posttypssida med andra. Användare som tar emot länken måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan eller posttypssidan som visas i den valda vyn.

## Delningsbehörigheter för Adobe Workfront Planning-objekt

Tabellerna i följande avsnitt visar vilken behörighetsnivå du kan välja när du delar en arbetsyta eller vy och vilka funktioner varje nivå tillåter.

>[!IMPORTANT]
>
>Alla användare kan inte ha de behörighetsnivåer som beskrivs nedan. Användarens individuella licens avgör vilken behörighetsnivå de kan få för Workfront Planning-objekt.
>
>Mer information finns i [Översikt över licenstyper vid användning av Adobe Workfront Planning](/help/quicksilver/maestro/access/license-type-overview.md).


### Behörigheter för arbetsytan

Du måste ge användarna behörighet till arbetsytor för att de ska kunna få åtkomst till följande enheter:

* Arbetsytor
* Posttyper
* Poster
* Fält
* Vyer*

  *Du kan tillåta alla användare med behörigheten Visa eller högre till en arbetsyta att även få åtkomst till vyerna på arbetsytan. Det här är en extra behörighet som du måste aktivera när du delar en vy. Mer information finns i [Visa](/help/quicksilver/maestro/access/share-views.md).

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


<!--You can share views internally or publicly. -->

Följande behörighetsnivåer gäller för vyer och visningselement:

|        | Hantera (Endast inbjudna personer kan komma åt) | Visa (Endast inbjudna personer kan komma åt) | Alla på arbetsytan kan visa* |
|--------|--------|-------|------------------------------|
| Redigera | ✓ |       |                            |
| Ta bort | ✓ |       |                            |
| Dela | ✓ |       |                           |
| Visa | ✓ | ✓ | ✓ |
| Använd | ✓ | ✓ | ✓ |

*Användarna måste ha behörigheten Visa eller högre för en arbetsyta för att få åtkomst till vyn.

<!--Replace the table above with the following when public sharing releases: 

|   Internal sharing     | Manage (Only invited people can access) | View (Only invited people can access)  |Everyone in the workspace can view*|
|--------|--------|-------|------------------------------|
| Edit   | ✓      |       |                            |
| Delete | ✓      |       |                            |
| Share  | ✓       |       |                           |
| View   | ✓      | ✓     | ✓                         |
| Apply  | ✓      | ✓     | ✓                          |

|   Public sharing      | View  |
|--------|-------|
| View   | ✓     |
| Apply  | ✓     |
-->


<!--old view permissions, before sharing View permissions to a view through a workspace:
|        | Manage | View  |
|--------|--------|-------|
| Edit   | ✓      |       |                            
| Delete | ✓      |       |                            
| Share  | ✓       |       |                           
| View   | ✓      | ✓     |                         
| Apply  | ✓      | ✓     |    
-->