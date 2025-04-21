---
title: Översikt över delningsbehörigheter i Adobe Workfront Planning
description: Alla användare i organisationen har inte samma åtkomst och behörigheter för att använda Adobe Workfront Planning. I den här artikeln beskrivs allmän information om hur du delar eller tar bort behörigheter till en arbetsyta eller vy i Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 5a4ceb3bd7a5f121312d26775b6cf91604585775
workflow-type: tm+mt
source-wordcount: '1122'
ht-degree: 0%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Översikt över delningsbehörigheter i Adobe Workfront Planning

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>



{{planning-important-intro}}

Du kan dela eller ta bort behörigheter till en Adobe Workfront Planning-arbetsyta eller -vy.

I den här artikeln beskrivs behörighetsnivåerna för Workfront Planning-objekt.

## Objekt som du kan dela i Adobe Workfront Planning

Du kan dela följande objekt manuellt i Workfront Planning:

* Arbetsytor

   * Du kan dela arbetsytor med personer i din organisation.
   * När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna.
   * När du delar en arbetsyta delas inte vyerna. Vyer delas separat.

  Mer information finns i [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)

<!--
<div class="preview">

* Record types

    * You can share record types with people inside your organization.
    * The level of permissions granted for the workspace displays as Inherited permissions for the record type. 
    * You cannot share a record type with a higher permission level than the user has on the workspace. 

    For more information, see [Share record types](/help/quicksilver/planning/access/share-record-types.md). 

</div>
-->

* Vyer

   * Du måste ge användare, inklusive systemadministratörer, behörighet att komma åt vyer separat från deras behörigheter till att komma åt arbetsytor.
   * När du delar en vy delas alla vyelement, inklusive filter, gruppering, sortering och inställningar.
   * När du delar en vy delas inte de poster som visas i vyn. Posterna måste delas med arbetsytor som delar dem.
   * Du kan dela en vy offentligt med personer utanför organisationen när du genererar en offentlig länk för en vy.Personer som öppnar postsidan från en offentlig länk kan visa alla poster och deras fält, inklusive anslutna poster och fält.

  Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

Internt kan du dela en arbetsyta eller vy med följande Workfront-enheter:

* Användare
* Grupper
* Team
* Företag
* Jobbroller

<span class="preview"> När du delar arbetsytor och posttyper med andra ärvs behörighetsnivån från posttypen automatiskt till de poster och fält som är associerade med dem. </span>

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
>Endast standardlicensanvändare (eller plananvändare) kan ha behörighet att hantera arbetsytor och behörigheter att hantera vyer i Contribute eller Hantera.
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

I produktionsmiljön ärvs alltid posttypsbehörigheter när du ger behörighet till arbetsytan.

Följande behörighetsnivåer gäller för posttyper:


|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Redigera | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |

<div class="preview">

I förhandsgranskningsmiljön kan du ta bort posttypens ärvda behörigheter som tagits emot från arbetsytan.

Du kan ge användarna lägre behörigheter för posttypen än de har på arbetsytan.

Du kan dock inte göra följande:

* Bevilja högre behörigheter för posttypen än vad användarna har på arbetsytan.
* Ge arbetsytehanterare lägre behörigheter för en posttyp.
* Ta bort visningsbehörigheter till posttypen eller arbetsytan genom att ta bort användare från posttypsbehörigheterna.

Följande scenarier finns:

| Workspace-behörigheter | Automatiskt ärvda behörigheter för en posttyp | Möjliga behörigheter för posttyp när ärvda behörigheter är inaktiverade (beviljas manuellt) |
|--------|--------|-------------|
| Hantera | Hantera | Hantera, ta bort behörigheter* |
| Contribute | Contribute | Contribute, Visa, Ta bort behörigheter* |
| Visa | Visa | Visa, ta bort behörigheter* |

>[!NOTE]
>
>*När du tar bort behörigheter från en posttyp behåller användarna fortfarande behörigheterna Visa på arbetsytan och alla posttyper, såvida du inte tar bort deras behörigheter från arbetsytan.

</div>

### Spela in behörigheter

Postbehörigheter ärvs från <span class="preview">posttypen</span> när du beviljar behörigheter till arbetsytan och <span class="preview">posttypen</span>.

Följande behörighetsnivåer gäller för poster:


|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ | ✓ |       |
| Ta bort | ✓ | ✓ |       |
| Redigera | ✓ | ✓ |       |
| Visa | ✓ | ✓ | ✓ |

### Fältbehörigheter

Fältbehörigheter ärvs från <span class="preview">posttypen</span> när du beviljar behörigheter till arbetsytan och <span class="preview">posttypen</span>.

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