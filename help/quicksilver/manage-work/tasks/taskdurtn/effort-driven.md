---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Översikt över varaktighetstyp: ansträngningsstyrd'
description: Ansträngningsstyrd är en typ av varaktighet som du kan ange för en uppgift i Adobe Workfront. Allmän information om varaktighetstyper i Workfront finns i Översikt över Varaktighet och Varaktighetstyp.
author: Alina
feature: Work Management
exl-id: 3c8534f7-02d0-4404-a37b-0ef6360e8efc
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '862'
ht-degree: 0%

---

# Översikt över varaktighetstyp: ansträngningsstyrd

Ansträngningsstyrd är en typ av varaktighet som du kan ange för en uppgift i Adobe Workfront. Allmän information om varaktighetstyper i Workfront finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Översikt över aktivitetsstyrd varaktighetstyp

Workfront eller en gruppadministratör kan ange systemets eller gruppens standardtyp för varaktighet som aktivitetsstyrd. I det här fallet skapas alla nya uppgifter med den här varaktighetstypen. Mer information om hur du ändrar uppgifter och utgåvor som en del av dina projektinställningar på system- eller gruppnivå finns i [Konfigurera uppgifter och ärenden för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

I det här scenariot finns det en risk för godtycklig förkortning av projektplanen, såvida du inte som projektledare tar dig tid att fundera över om aktiviteten egentligen är en aktivitetsstyrd uppgift.

Använd ansträngningsalternativet för att:

* Fastställ den planerade varaktigheten baserat på antalet resurser som är tillgängliga för att arbeta med uppgiften. Varaktigheten är lika med Planerade timmar. Planerad varaktighet är lika med Planerade timmar dividerat med antalet tilldelningar.

  Den ansträngningsnivå som används för uppgiften avgör arbetsfördelningen och varaktigheten.

* Spåra det totala antalet timmar som har ägnats åt en aktivitet när flera resurser har tilldelats.

  När resurser läggs till minskar aktivitetens planerade varaktighet. (Principen om att&quot;många händer ska göra ljusverk&quot; visar vilken effekt den här varaktighetstypen har på den planerade varaktigheten för en uppgift.)

I följande avsnitt finns mer detaljerad information om hur Workfront beräknar den planerade varaktigheten för en aktivitetsstyrd uppgift och vilken effekt som tillägg av resurser har på uppgiften med den här varaktighetstypen.

## Översikt över formeln för aktivitetsstyrd varaktighetstyp

Formeln för beräkning av planerad varaktighet för en aktivitet med varaktighetstypen ansträngningsenhet beror på allokeringsprocenten för varje resurs som tilldelats aktiviteten. När det gäller en insatsstyrd uppgift beräknar Workfront planerad tid för uppgiften och är alltid densamma som varaktigheten för uppgiften:

```
Planned Hours (in hours) = Duration (in days)
```

Du kan justera aktivitetens varaktighet manuellt.

Workfront förutsätter att det finns åtta arbetstimmar per arbetsdag. Din Workfront- eller gruppadministratör definierar timmarna per arbetsdag med inställningen Normal antal timmar per arbetsdag i Projektinställningar i Inställningar. Mer information om hur du ändrar inställningar för aktiviteter och utgåvor som en del av dina projektinställningar på systemnivå finns i [Konfigurera uppgifter och utgåvor för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

>[!TIP]
>
>Workfront undersöker schemat för varje resurs som tilldelats aktiviteten för att fastställa procentandelen allokering för varje resurs för aktiviteten. Mer information om hur du skapar och tilldelar scheman till användare finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

Tänk på följande scenarier:

* [Resurser tilldelas 100 % till aktiviteten](#resources-are-allocated-100-to-the-task)
* [Resurser tilldelas för olika procentsatser av tid till uppgiften](#resources-are-allocated-for-various-percentages-of-time-to-the-task)

### Resurser tilldelas 100 % till uppgiften {#resources-are-allocated-100-to-the-task}

Den här formeln förutsätter att alla resurser tilldelas 100 % till aktiviteten.

```
Planned Duration = (Planned Hours / Number of Resources) / 8
```

Beräkningen förutsätter att antalet timmar i en normal arbetsdag är 8. Ekvationen innehåller det här värdet så att den planerade varaktigheten visas i dagar.

### Resurser tilldelas för olika procentsatser av tid till uppgiften {#resources-are-allocated-for-various-percentages-of-time-to-the-task}

Eftersom varje tilldelad resurs kan ha en unik allokeringsnivå, tar formeln hänsyn till dessa allokeringsvärden:

```
Planned Duration = (Planned Hours / SUM(Percent allocation for each resource for the task)) / 8
```

Beräkningen förutsätter att antalet timmar i en normal arbetsdag är 8. Ekvationen innehåller det här värdet så att den planerade varaktigheten visas i dagar.

## Effekten av att lägga till fler resurser i en uppgift

När du lägger till eller tar bort tilldelningar till en uppgift med aktivitetsstyrd varaktighetstyp ändras inte Varaktighet och Planerade timmar. Den planerade varaktigheten ändras dock.

I följande exempel är Normal Timme per arbetsdag inställd på 8 i projektinställningarna i systeminställningarna. Eftersom varaktigheten är 3 dagar, är antalet planerade timmar 24 (3 dagar x 8 timmar per arbetsdag = 24 planerade timmar).

>[!NOTE]
>
>När du använder uppgiftsbegränsningen Fasta datum ändras inte den planerade varaktigheten när du lägger till eller tar bort tilldelningar. I stället justeras varaktigheten och Planerade timmar. När du använder en annan aktivitetsbegränsning än Fasta datum justeras den planerade varaktigheten.

I följande tabell visas hur den planerade varaktigheten ändras genom att resurser läggs till i uppgiften:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> </th> 
   <th> <p><strong>Antal tilldelade (varje 100 % allokerat)</strong> </p> </th> 
   <th> <p><strong>Varaktighet</strong> </p> </th> 
   <th> <p><strong>Planerade timmar</strong> </p> </th> 
   <th><strong>Planerad varaktighet</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> </td> 
   <td> <p>1</p> </td> 
   <td> <p>3 dagar</p> </td> 
   <td> <p>24 timmar</p> <p>(3 dagar x 8 timmar per arbetsdag = 24 planerade timmar)</p> </td> 
   <td> <p>3 dagar</p> <p>(24 planerade timmar/1 tilldelad = 3 dagar)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>2</p> </td> 
   <td> <p>3 dagar</p> </td> 
   <td> <p>24 timmar</p> <p>(3 dagar x 8 timmar per arbetsdag = 24 planerade timmar)</p> </td> 
   <td> <p>1,5 dagar</p> <p>(24 planerade timmar/2 tilldelningar = 12 timmar, eller 1,5 dagar)</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> <p>3</p> </td> 
   <td> <p>3 dagar</p> </td> 
   <td> <p>24 timmar</p> <p>(3 dagar x 8 timmar per arbetsdag = 24 planerade timmar)</p> </td> 
   <td> <p>1 dag</p> <p>(24 planerade timmar/3 uppdragsgivare = 8 timmar eller 1 dag)</p> </td> 
  </tr> 
 </tbody> 
</table>

## Ändra varaktighetstypen för en uppgift till insatsstyrd

Mer information om hur du ändrar varaktighetstypen för en aktivitet finns i [Uppdatera varaktighetstypen för en aktivitet](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Effort Driven</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong><strong>Changes</strong>.</li>
</ol>
-->
