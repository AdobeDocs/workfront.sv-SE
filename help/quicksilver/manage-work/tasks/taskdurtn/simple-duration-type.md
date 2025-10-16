---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: 'Översikt över varaktighetstyp: Enkel'
description: Den enkla varaktighetstypen är en varaktighetstyp som du kan ange för en uppgift i Adobe Workfront.
author: Alina
feature: Work Management
exl-id: 9bb472db-1448-467e-93ca-611453e1c00a
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '322'
ht-degree: 0%

---

# Översikt över varaktighetstyp: Enkel

<!-- Audited: 5/2025 -->

Den enkla varaktighetstypen är en varaktighetstyp som du kan ange för en uppgift i Adobe Workfront. Mer information om varaktighetstyper i Workfront finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

## Översikt över den enkla varaktighetstypen

Din Workfront- eller gruppadministratör kan ange standardvaraktighetstypen för ditt system eller din grupp som Enkel. I det här fallet skapas alla nya uppgifter med den här varaktighetstypen.

Mer information om hur du ändrar uppgifter och utgåvor som en del av dina projektinställningar på system- eller gruppnivå finns i [Konfigurera uppgifter och ärenden för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

Följande saker händer när en uppgift har en typ av enkel varaktighet:

* Projektledare kan ändra både tidslängden och den planerade timmen för en uppgift när de ändrar hur timmarna ska fördelas mellan de tilldelade.

  Mer information finns i [Uppdatera planerade timmar och varaktighet för en aktivitet med en enkel varaktighetstyp](../../../manage-work/tasks/taskdurtn/update-planned-hours-duration-for-simple-duration-task.md).

  >[!IMPORTANT]
  >
  >När du först skapar en uppgift och tilldelar den typen Enkel varaktighet, men inte anger en varaktighet, beräknas aktivitetens varaktighet i Workfront utifrån den mängd Planerade timmar som du anger för uppgiften. Om du ändrar varaktigheten för en enkel varaktighetsåtgärd avbryter Workfront matchningen av de planerade timmarna med varaktigheten eftersom det förutsätts att du vill definiera dem manuellt.
  >
  >Workfront beräknar varaktigheten för uppgifter vars varaktighet inte har ändrats manuellt med hjälp av följande formel:
  >
  > `Task Duration = Task Planned Hours / Typical hours per work day`
  >
  >Din Workfront-administratör definierar `Typical hours per work day` i området Projektinställningar i instansens installationsprogram.

* Allokeringsprocenten är dold, men allokeringstimmar är tillgängliga för redigering.
* Alla nya kunder har varaktighetstypen på systemnivå inställd på Enkel.

## Ändra varaktighetstypen för en aktivitet till Enkel

Mer information om hur du ändrar varaktighetstypen för en aktivitet finns i [Uppdatera varaktighetstypen för en aktivitet](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: replaced with new article linked above)</p>
-->

<!--
<ol data-mc-conditions="QuicksilverOrClassic.Draft mode">
<li value="1">Go to a task for which you want to change the Duration Type.</li>
<li value="2"> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver">Click <strong>Task Details</strong> in the left panel, then in the Overview area double click <strong>Duration Type</strong>. </p> </li>
<li value="3"> <p>Select <strong>Simple</strong> from the drop-down menu.</p> </li>
<li value="4">Click <strong>Save</strong> <strong>Changes</strong><strong>.</strong></li>
</ol>
-->
