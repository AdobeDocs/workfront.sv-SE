---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Varaktighetstyper i Adobe Workfront och Microsoft Project
description: De varaktighetstyper som är tillgängliga i Adobe Workfront skiljer sig från deras motsvarigheter i Microsoft Project, som kallas uppgiftstyper. Detta kan vara förvirrande ibland vid export eller import av projekt mellan Workfront och Microsoft Project.
author: Alina
feature: Work Management
exl-id: 986ecf91-693d-4ee1-bc56-355a2819ae41
source-git-commit: c1b8af0d8a95714bb597db7a429794773358cf05
workflow-type: tm+mt
source-wordcount: '256'
ht-degree: 0%

---

# Varaktighetstyper i Adobe Workfront och Microsoft Project

De varaktighetstyper som är tillgängliga i Adobe Workfront skiljer sig från deras motsvarigheter i Microsoft Project, som kallas uppgiftstyper. Detta kan vara förvirrande ibland vid export eller import av projekt mellan Workfront och Microsoft Project.

Mer information om hur du importerar och exporterar projekt mellan Workfront och Microsoft Project finns i följande artiklar:

* [Exportera ett projekt till Microsoft Project](../../../manage-work/projects/manage-projects/export-project-to-ms-project.md)
* [Importera ett projekt från Microsoft Project](../../../manage-work/projects/create-projects/import-project-from-ms-project.md)

## Varaktighetstyper i Workfront och Microsoft Project

Workfront har fyra olika varaktighetstyper:

* Enkel
* Ansträngningsstyrd
* Beräknat arbete
* Beräknad tilldelning

Mer information finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

Dessa varaktighetstyper känns inte igen av Microsoft Project. För närvarande har Microsoft Project tre aktivitetstyper som liknar varaktighetstyper i Workfront:

* Fasta enheter
* Fast arbete
* Fast varaktighet

## Varaktighetstypen ändras vid export från Workfront till MS Project

När du exporterar projekt från Workfront till Microsoft Project blir uppgifter som styrs av satsningar fasta. Enkelt, Beräknat arbete och Beräknad tilldelning blir fasta enheter.

## Varaktighetstypen ändras vid import från MS Project till Workfront

När du importerar projekt från Microsoft Project till Workfront blir Fasta enheter&quot;Ansträngningsstyrda&quot;. Fast arbete och Fast varaktighet får den standardvaraktighetstyp som din Workfront-administratör har valt för ditt system. Mer information finns i [Konfigurera uppgifter och utgåvinställningar för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

<!--
<note type="warning">
When a task has Calculated Work as the Duration Type and the default Duration Type in Setup is set as Calculated Assignment, then MS Project assignment allocations will be lost during the import.
<MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
(drafting this because it is misleading)
</MadCap:conditionalText>
</note>
-->
