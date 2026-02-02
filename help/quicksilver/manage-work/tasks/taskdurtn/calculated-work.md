---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Översikt över varaktighetstyp: Beräknat arbete'
description: Beräknat arbete är en varaktighetstyp som du kan ange för en uppgift i Adobe Workfront. Allmän information om varaktighetstyper i Workfront finns i Översikt över Varaktighet och Varaktighetstyp.
author: Alina
feature: Work Management
exl-id: f521c2f5-8d58-44c0-af18-6940ad0950ea
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '568'
ht-degree: 0%

---

# Översikt över varaktighetstyp: Beräknat arbete

Beräknat arbete är en varaktighetstyp som du kan ange för en uppgift i Adobe Workfront. Allmän information om varaktighetstyper i Workfront finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Översikt över den beräknade varaktighetstypen för arbete

Beräknat arbete avgör mängden arbetsinsats (planerade timmar) som krävs för att uppgiften ska kunna slutföras. Vi rekommenderar att du använder den beräknade varaktighetstypen för arbete när resurserna som tilldelats uppgiften tilldelas för hela aktivitetens varaktighet.

Workfront eller en gruppadministratör kan ange systemets eller gruppens standardtyp för varaktighet som Beräknat arbete. I det här fallet skapas alla nya uppgifter med den här varaktighetstypen. Mer information om hur du ändrar uppgifter och utgåvor som en del av dina projektinställningar på system- eller gruppnivå finns i [Konfigurera uppgifter och ärenden för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

När resurser läggs till i en uppgift kan projektledaren förvänta sig att den planerade ansträngningen ökar. Ett timmars planeringsmöte med tre resurser representerar tre timmars arbete, och ett timmars planeringsmöte med tio resurser representerar tio timmars arbete. Detta förutsätter att varje resurs tilldelas till aktiviteten med 100 % allokering.

## Granska formeln för beräkning av arbete som krävs när du använder den beräknade varaktighetstypen för arbete

När du använder Beräknad arbetstid för en uppgift beräknas arbetsmängden för varje uppgift i Workfront med hjälp av följande två formler. Formler varierar beroende på hur stor procentandel av tiden varje resurs tilldelas till aktiviteten och hur många resurser du har tilldelat varje uppgift:

* Förenklad formel: Om du har en resurs tilldelad till aktiviteten och de tilldelas till uppgiften för 100 % av den tillgängliga tiden, beräknas värdet för arbete som krävs för varje uppgift enligt följande formel:

```
Work Required (Planned Hours) = (Duration of the task in hours) x (The number of resources assigned to the task)
```

* Komplex formel: Om du tilldelar varje resurs med olika allokeringar, tar formeln hänsyn till dessa allokeringar och tar hänsyn till dessa variationer:

```
Work Required (Planned Hours) = SUM[(Duration of the task in hours) x (Percent allocated towards tasks for each resource)]
```

## Granska effekten av att lägga till eller ta bort resurser från uppgiften

När du lägger till eller tar bort tilldelningar till en uppgift med typen Beräknad arbetstid kan du redigera varaktigheten manuellt. När tilldelningar läggs till eller tas bort från aktiviteten ändras antalet planerade timmar.

I följande exempel är Normal Timme per arbetsdag inställd på 8 i Projektinställningar i Inställningar. Varje uppgift har en varaktighet på 1 dag. När antalet tilldelningar ändras ändras, ändras antalet planerade timmar baserat på antalet tilldelningar för en given uppgift:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Antal tilldelade (varje 100 % allokerat)</strong> </p> </th> 
   <th> <p><strong>Varaktighet</strong> </p> </th> 
   <th> <p><strong>Planerade timmar</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>1</p> </td> 
   <td> <p>1 dag</p> </td> 
   <td> <p>8 timmar</p> <p>(1 dag x 8 timmar per arbetsdag x 1 tilldelad = 8 planerade timmar)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>2</p> </td> 
   <td> <p>1 dag</p> </td> 
   <td> <p>16 timmar</p> <p>(1 dag x 8 timmar per arbetsdag x 2 tilldelningar = 16 planerade timmar)</p> </td> 
  </tr> 
  <tr> 
   <td> <p>3</p> </td> 
   <td> <p>1 dag</p> </td> 
   <td> <p>24 timmar</p> <p>(1 dag x 8 timmar per arbetsdag x 3 tilldelningar = 24 planerade timmar)</p> </td> 
  </tr> 
 </tbody> 
</table>

I det här fallet tilldelas varje tilldelad 100 % till aktiviteten Beräknat arbete.

![Beräknat varaktighetstyp](assets/calcwork-350x71.png)

## Ändra varaktighetstypen för en aktivitet till Beräknat arbete

Mer information om hur du ändrar varaktighetstypen för en aktivitet finns i [Uppdatera varaktighetstypen för en aktivitet](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3">Select <strong>Calculated Work</strong> from the drop-down menu.</li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong>.</li>
</ol>
-->
