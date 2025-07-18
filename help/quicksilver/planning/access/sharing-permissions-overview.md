---
title: Översikt över delningsbehörigheter i Adobe Workfront Planning
description: Alla användare i organisationen har inte samma åtkomst och behörighet att använda Adobe Workfront Planning. I den här artikeln beskrivs allmän information om hur du delar eller tar bort behörigheter till en arbetsyta eller vy i Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 298c542afea902d9fc14ef6a4470c0bc1d9bd33c
workflow-type: tm+mt
source-wordcount: '1155'
ht-degree: 0%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Översikt över delningsbehörigheter i Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Du kan dela eller ta bort behörigheter till en arbetsyta, en posttyp eller en vy i Adobe Workfront Planning.

Du kan också dela formulär för planeringsbegäran. Mer information finns [i Skapa och hantera ett förfrågningsformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

I den här artikeln beskrivs behörighetsnivåerna för Workfront Planning-arbetsytor, posttyper, poster, fält och vyer.

## Objekt som du kan dela i Adobe Workfront Planning

Du kan dela vissa Workfront Planning-objekt manuellt, medan andra objekt ärver dessa behörigheter från andra objekt.

Du kan dela följande objekt manuellt i Workfront Planning:

* Arbetsytor

   * Du kan dela arbetsytor med personer i din organisation.
   * När du delar en arbetsyta delas även alla posttyper, poster och fält som är associerade med arbetsytorna.
   * När du delar en arbetsyta delas inte vyer. Vyer delas separat.

  Mer information finns i [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)

* Typer av poster

   * Du kan dela posttyper med personer i din organisation.
   * Den behörighetsnivå som beviljas för arbetsytan visas som Ärvda behörigheter för posttypen.
   * Du kan inte dela en posttyp med en högre behörighetsnivå än vad användaren har på arbetsytan.

  Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).


* Visningar

   * Du måste ge användare, inklusive systemadministratörer, behörighet att komma åt vyer separat från deras behörigheter till att komma åt arbetsytor.
   * När du delar en vy delas alla vyelement, inklusive filter, gruppering, sortering och inställningar.
   * När du delar en vy delas inte de poster som visas i vyn. Arkivhandlingar måste delas genom att dela arbetsytor.
   * Du kan dela en vy offentligt med personer utanför organisationen när du skapar en offentlig länk för en vy. Personer som kommer åt postsidan från en offentlig länk kan visa alla poster och deras fält, inklusive anslutna poster och fält.

  Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

Internt kan du dela en arbetsyta, en vy eller en posttyp med följande Workfront-enheter:

* Användare
* Grupper
* Team
* Företag
* Yrkesroller

När du delar arbetsytor och posttyper med andra ärvs behörighetsnivån från posttypen automatiskt till de poster och fält som är kopplade till dem.

>[!IMPORTANT]
>
>Om din organisations instans av Workfront har registrerats i Adobe Unified Experience måste de användare som du vill dela planeringsobjekt med läggas till i Adobe Admin Console. Du kan inte dela planeringsobjekt med Workfront-användare som inte har lagts till i Adobe Admin Console.


## Att tänka på när du delar objekt i Adobe Workfront Planning

* Din Adobe Workfront-licenstyp fungerar tillsammans med dina Workfront Planning-behörigheter för att ge dig tillgång till att visa, bidra eller hantera arbetsytor och deras objekt.

  Mer information om hur licenstyper påverkar behörighetsnivåer för Workfront Planning finns i [Översikt över licenstyper när du använder Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Systemadministratörer kan hantera alla arbetsytor i systemet, även de som de inte har skapat.
* Andra användare, inklusive systemadministratörer, kan bara komma åt vyer som de har skapat eller som har delats med dem. Systemadministratörer kan endast ges behörighet att hantera en vy.
* Du kan dela en länk till en arbetsyta eller till en vy med andra.

  Följande scenarier finns:
   * Användare som får länken till en arbetsyta måste vara aktiva användare och logga in på Workfront för att kunna komma åt arbetsytan.
   * Användare som får länken till en vy kan komma åt vyn på följande sätt:

      * Måste vara aktiva användare och logga in på Workfront, om länken till vyn har delats internt.
      * Kan vara externa användare till Workfront och komma åt vyn från en offentligt delad länk, utan att logga in på Workfront.

## Dela behörigheter för Adobe Workfront Planning-objekt

Tabellerna i följande avsnitt illustrerar den behörighetsnivå som du kan välja när du delar en arbetsyta eller en vy och vilka funktioner varje nivå tillåter.

>[!IMPORTANT]
>
>Alla användare kan inte ha de behörighetsnivåer som beskrivs nedan. Användarnas individuella licens avgör vilken behörighetsnivå de kan få för Workfront Planning-objekt.
>
>Endast användare med standardlicens (eller plan) kan ha behörigheten Delta eller Hantera till arbetsytor och Hantera behörigheter till vyer.
> 
>Användare med alla andra licenstyper kan ha visningsbehörighet till arbetsytor och vyer.
>
>Mer information finns i [Översikt över licenstyper när du använder Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).


### Behörigheter till arbetsytor

Du måste ge användare behörighet till arbetsytor för att de ska få åtkomst till följande entiteter:

* Arbetsytor
* Typer av poster
* Arkiv
* Fält

Följande är behörighetsnivåer för arbetsytor:

|        | Förvalta | Bidra | Utsikt |
|--------|--------|------------|-------|
| Redigera | ✓ |            |       |
| Aktie | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Utsikt | ✓ | ✓ | ✓ |

### Behörigheter till posttyper

<!-- old access:
In the Production environment, Record Type permissions are always inherited when you grant permissions to the workspace.

The following are the levels of permissions for record types: 


|        | Manage | Contribute | View  |
|--------|--------|------------|-------|
| Create | ✓      |            |       |
| Delete | ✓      |            |       |
| Edit   | ✓      |            |       |
| View   | ✓      | ✓          | ✓     |

-->

Behörigheter för posttyp ärvs alltid när du beviljar behörigheter till arbetsytan.

Du kan ta bort posttypens ärvda behörigheter som du har fått från arbetsytan.

Du kan ge användare lägre behörigheter för posttypen än de har på arbetsytan.

Du kan dock inte göra följande:

* Bevilja högre behörigheter för posttypen än vad användarna har på arbetsytan.
* Ge arbetsrumsansvariga lägre behörigheter för en posttyp.
* Ta bort visningsbehörigheter till posttypen eller arbetsytan genom att ta bort användare från posttypsbehörigheterna.

Följande scenarier finns:

| Behörigheter för arbetsyta | Automatiskt ärvda behörigheter för en posttyp | Möjliga behörigheter för posttyp när ärvda behörigheter är avstängda (beviljas manuellt) |
|--------|--------|-------------|
| Förvalta | Förvalta | Hantera, ta bort behörigheter* |
| Contribute | Contribute | Behålla, visa, ta bort behörigheter* |
| Utsikt | Utsikt | Visa, ta bort behörigheter* |

>[!NOTE]
>
>*När du tar bort behörigheter från en posttyp behåller användarna fortfarande behörigheterna Visa på arbetsytan och alla posttyper, såvida du inte tar bort deras behörigheter från arbetsytan.

### Behörigheter till poster

Postbehörigheter ärvs från posttypen när du ger behörighet till arbetsytan och posttypen.

Följande behörighetsnivåer gäller för poster:


|        | Förvalta | Bidra | Utsikt |
|--------|--------|------------|-------|
| Skapa | ✓ | ✓ |       |
| Ta bort | ✓ | ✓ |       |
| Redigera | ✓ | ✓ |       |
| Utsikt | ✓ | ✓ | ✓ |

### Behörigheter att registrera fält

Fältbehörigheter ärvs från posttypen när du ger behörighet till arbetsytan och posttypen.

Följande behörigheter refererar till själva fälten och inte till värdena som associeras med varje fält. Om du vill redigera fältvärden måste du ha behörighet att redigera poster.

|        | Förvalta | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Redigera | ✓ |            |       |
| Utsikt | ✓ | ✓ | ✓ |


### Behörigheter till vyer

Du måste ge separata behörigheter för att spela in vyer. Att bevilja behörigheter till arbetsytan ger inte behörighet till postvyerna på arbetsytan.

Du måste ge användarna behörighet till vyer för att de ska få åtkomst till följande vyelement:

* Filter
* Synlighet i fält
* Sortera
* Gruppering
* Radhöjd
* Inställningar

Du kan dela åsikter internt eller offentligt.

Följande är behörighetsnivåerna för vyer och vyelement:

| Intern delning | Hantera (endast inbjudna personer har åtkomst) | Visa (endast inbjudna personer har åtkomst) | Alla på arbetsytan kan visa* |
|--------|--------|-------|------------------------------|
| Redigera | ✓ |       |                            |
| Ta bort | ✓ |       |                            |
| Aktie | ✓ |       |                           |
| Utsikt | ✓ | ✓ | ✓ |
| Använda | ✓ | ✓ | ✓ |

| Offentlig delning | Utsikt |
|--------|-------|
| Utsikt | ✓ |
| Använda | ✓ |

*Användare måste ha visningsbehörighet eller högre behörighet till en arbetsyta för att få åtkomst till den här vyn.

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
