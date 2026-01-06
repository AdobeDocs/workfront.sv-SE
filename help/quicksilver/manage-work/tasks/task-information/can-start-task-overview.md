---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '"Kan starta" Översikt över aktiviteter'
description: När en uppgift är klar att starta lägger Adobe Workfront till en Can Start-indikator i uppgiften för att enkelt identifiera att det är säkert för dig att börja arbeta med uppgiften. Du kan visa den här indikatorn i vyn för en uppgiftslista eller rapport.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: dbc4404501e20b3f1905a5eebd13734a65db27ae
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# &quot;Kan starta&quot; - översikt för uppgifter

När en uppgift är klar att starta lägger Adobe Workfront till en Can Start-indikator i uppgiften för att enkelt identifiera att det är säkert för dig att börja arbeta med uppgiften. Du kan visa den här indikatorn i vyn för en uppgiftslista eller rapport.

När aktiviteten är klar att bearbetas ställs fältet Kan starta för aktiviteten in på True.

## Så här markerar Workfront en uppgift som&quot;Kan starta&quot;

Workfront söker efter följande saker innan en uppgift markeras som True för fältet Can Start:

* Anger om värdet för Can Start för den överordnade har värdet True, om aktiviteten har en överordnad. Om värdet för det överordnade objektet är Falskt får alla underaktiviteter värdet Can Start också värdet False.
* Anger om uppgiftens föregångare och deras föräldrars föregångare är fullständiga. Om de är klara anges värdet Kan starta för uppgiften till Sant. Om någon av uppgiftens föregångare eller deras överordnade föregångare inte är slutförd, eller har statusen Fullständigt väntande godkännande, anges värdet Kan starta för uppgiften till Falskt.
* Anger om aktivitetens beroendetyp är Start-Start eller Start-Finish. Om beroendetypen är Start-Start eller Start-Finish kommer den beroende aktiviteten att ha flaggan Can start inställd på True efter att föregående aktivitet pågår (eller efter att procentandelen slutfört för föregående aktivitet är större än 1 %).

  Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Överväganden om att identifiera uppgifter som är klara att börja

* Om beroendetypen mellan en aktivitet och dess föregångare är Start-Start måste föregående aktivitet starta innan den föregående relationen anses vara löst och efterföljande aktiviteter kan starta. Mer information om beroendetyper finns i [Översikt över aktivitetsberoendetyper](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Om en aktivitet har en föregångare som sträcker sig över flera projekt aktiveras inte indikatorn Kan starta automatiskt när föregångaren slutförs. Du måste manuellt beräkna om tidslinjen för den efterföljande partens projekt eller så måste Workfront automatiskt beräkna om den, innan den efterföljande uppgiften visas som en Kan starta-uppgift. Mer information om hur du beräknar om projekttidslinjer finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

  Mer information om föregående projekt finns i [Skapa föregående projekt](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
