---
title: Översikt över delningsbehörigheter i Adobe Workfront Planning
description: Alla användare i organisationen har inte samma åtkomst och behörigheter för att använda Adobe Workfront Planning. I den här artikeln beskrivs allmän information om hur du delar eller tar bort behörigheter till en arbetsyta eller vy i Adobe Workfront Planning.
author: Alina
feature: Workfront Planning
role: User, Admin
recommendations: noDisplay, noCatalog
exl-id: 698036a6-b3b4-44a9-91ee-63fdb6a646a1
source-git-commit: 53596271a838733b858c0b14a4e22b07a7cd20f6
workflow-type: tm+mt
source-wordcount: '1165'
ht-degree: 0%

---


<!--over time, this article should look like this one does: https://eperienceleague.adobe.com/docs/workfront/using/basics/grant-request-object-permissions/sharing-permissions-on-objects-overview.html?lang=en-->

<!--remove the Prod and Preview references when we release to Prod-->

# Översikt över delningsbehörigheter i Adobe Workfront Planning

<!--<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. After the monthly releases to Production, the same features are also available in the Production environment for customers who enabled fast releases. </span>   

<span class="preview">For information about fast releases, see [Enable or disable fast releases for your organization](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>-->



{{planning-important-intro}}

Du kan dela eller ta bort behörigheter till en Adobe Workfront Planning-arbetsyta, posttyp eller vy.

Du kan också dela planeringsförfrågningsformulär. Mer information finns i [Skapa och hantera ett begärandeformulär i Adobe Workfront Planning](/help/quicksilver/planning/requests/create-request-form.md).

I den här artikeln beskrivs behörighetsnivåerna för Workfront Planning Workspaces, posttyper, poster, fält och vyer.

## Objekt som du kan dela i Adobe Workfront Planning

Du kan dela vissa Workfront Planning-objekt manuellt, medan andra objekt ärver dessa behörigheter från andra objekt.

Du kan dela följande objekt manuellt i Workfront Planning:

* Arbetsytor

   * Du kan dela arbetsytor med personer i din organisation.
   * När du delar en arbetsyta delas även alla posttyper, poster och fält som är kopplade till arbetsytorna.
   * När du delar en arbetsyta delas inte vyerna. Vyer delas separat.

  Mer information finns i [Dela arbetsytor](/help/quicksilver/planning/access/share-workspaces.md)

* Posttyper

   * Du kan dela posttyper med personer i din organisation.
   * Nivån för behörigheter som beviljas för arbetsytan visas som ärvda behörigheter för posttypen.
   * Du kan inte dela en posttyp med en högre behörighetsnivå än användaren har på arbetsytan.

  Mer information finns i [Dela posttyper](/help/quicksilver/planning/access/share-record-types.md).


* Vyer

   * Du måste ge användare, inklusive systemadministratörer, behörighet att komma åt vyer separat från deras behörigheter till att komma åt arbetsytor.
   * När du delar en vy delas alla vyelement, inklusive filter, gruppering, sortering och inställningar.
   * När du delar en vy delas inte de poster som visas i vyn. Posterna måste delas med arbetsytor som delar dem.
   * Du kan dela en vy offentligt med personer utanför organisationen när du genererar en offentlig länk för en vy.Personer som öppnar postsidan från en offentlig länk kan visa alla poster och deras fält, inklusive anslutna poster och fält.

  Mer information finns i [Dela vyer](/help/quicksilver/planning/access/share-views.md).

## Att tänka på när du delar objekt i Adobe Workfront Planning

* Din Adobe Workfront-licenstyp fungerar tillsammans med dina Workfront Planning-behörigheter så att du kan visa, bidra till eller hantera arbetsytor och deras objekt.

  Mer information om hur licenstyperna påverkar behörighetsnivåer för Workfront Planning finns i [Översikt över licenstypen när du använder Adobe Workfront Planning](/help/quicksilver/planning/access/license-type-overview.md).
* Systemadministratörer kan hantera alla arbetsytor i systemet, inklusive de som de inte skapade.
* Andra användare, inklusive systemadministratörer, kan bara komma åt vyer som de har skapat eller som har delats med dem. Systemadministratörer kan endast ges behörighet för att hantera en vy.

* När du delar arbetsytor och posttyper med andra, ärvs behörighetsnivån från posttypen automatiskt till de poster och fält som är associerade med dem.

  >[!IMPORTANT]
  >
  >Om din organisations instans av Workfront har registrerats för Adobe Unified Experience måste de användare som du vill dela Planning-objekt med läggas till i Adobe Admin Console. Du kan inte dela Planning-objekt med Workfront-användare som inte har lagts till i Adobe Admin Console.

* Du kan dela planeringsobjekt på följande sätt:

   * Internt kan du dela en arbetsyta, en vy eller en posttyp med följande Workfront-enheter:

      * Användare
      * Grupper
      * Team
      * Företag
      * Jobbroller

     Du kan dela ett Planning-objekt med upp till 100 enheter per objekt.

   * Internt genom att dela en länk till en arbetsyta eller till en vy med andra planeringsanvändare. Följande scenarier finns:

      * Användare som får länken till en arbetsyta måste vara aktiva användare och logga in på Workfront för att få tillgång till arbetsytan.
      * Användare som får en intern delningslänk för en vy måste vara aktiva användare och logga in på Workfront för att få åtkomst till vyn.
   * Externt genom att dela en offentlig delningslänk till en vy med externa användare som inte har något Workfront-konto.

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


### Behörigheter till arbetsytor

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

### Behörigheter för posttyper

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

Posttypsbehörigheter ärvs alltid när du ger behörighet till arbetsytan.

Du kan ta bort posttypens ärvda behörigheter som har tagits emot från arbetsytan.

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
>När du tar bort behörigheter från en posttyp behåller användarna fortfarande behörigheterna Visa på arbetsytan och alla posttyper, såvida du inte tar bort deras behörigheter från arbetsytan.

### Behörigheter till poster

Postbehörigheter ärvs från posttypen när du ger behörighet till arbetsytan och posttypen.

Följande behörighetsnivåer gäller för poster:


|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ | ✓ |       |
| Ta bort | ✓ | ✓ |       |
| Redigera | ✓ | ✓ |       |
| Visa | ✓ | ✓ | ✓ |

### Behörigheter att registrera fält

Fältbehörigheter ärvs från posttypen när du ger behörighet till arbetsytan och posttypen.

Följande behörigheter refererar till själva fälten och inte till värdena som associeras med varje fält. Om du vill redigera fältvärden måste du ha behörighet att redigera poster.

|        | Hantera | Contribute | Visa |
|--------|--------|------------|-------|
| Skapa | ✓ |            |       |
| Ta bort | ✓ |            |       |
| Redigera | ✓ |            |       |
| Visa | ✓ | ✓ | ✓ |


### Behörigheter till vyer

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
