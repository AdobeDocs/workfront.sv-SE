---
content-type: overview
product-area: projects
navigation-topic: task-information
title: '`Can Start` overview for tasks'
description: När en uppgift är klar att starta lägger Adobe Workfront till en Can Start-indikator i uppgiften för att enkelt identifiera att det är säkert för dig att börja arbeta med uppgiften. Du kan visa den här indikatorn i vyn för en uppgiftslista eller rapport.
author: Alina
feature: Work Management
exl-id: 158f8370-9717-4c61-99fa-e3b76a9e61cb
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# &quot;Kan starta&quot; - översikt för uppgifter

När en uppgift är klar att starta lägger Adobe Workfront till en Can Start-indikator i uppgiften för att enkelt identifiera att det är säkert för dig att börja arbeta med uppgiften. Du kan visa den här indikatorn i vyn för en uppgiftslista eller rapport.

När aktiviteten är klar att bearbetas ställs fältet Kan starta för aktiviteten in på True.

## Så här markerar Workfront en uppgift som&quot;Kan starta&quot;

Workfront söker efter följande saker innan en uppgift markeras som True för fältet Can Start:

* Om aktiviteten har en överordnad kontrollerar den om värdet för Kan starta för den överordnade som är inställt på Sant. Om värdet för det överordnade objektet är Falskt får alla underaktiviteter värdet Can Start också värdet False. 
* Den kontrollerar också om uppgiftens föregångare och deras föräldrars föregångare är fullständiga. Om de är klara anges värdet Kan starta för uppgiften till Sant. Om någon av uppgiftens föregångare eller deras överordnade föregångare inte är slutförd, eller har statusen Fullständigt väntande godkännande, anges värdet Kan starta för uppgiften till Falskt. 

   Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Överväganden om att identifiera uppgifter som är klara att börja

* Om beroendetypen mellan en aktivitet och dess föregångare är Start-Start måste föregående aktivitet starta innan den föregående relationen anses vara löst och efterföljande aktiviteter kan starta. Mer information om beroendetyper finns i [Översikt över typer av uppgiftsberoenden](../../../manage-work/tasks/use-prdcssrs/task-dependency-types.md).
* Om en aktivitet har en föregångare som sträcker sig över flera projekt aktiveras inte indikatorn Kan starta automatiskt när föregångaren slutförs. Du måste manuellt beräkna om tidslinjen för den efterföljande partens projekt eller så måste Workfront automatiskt beräkna om den, innan den efterföljande uppgiften visas som en Kan starta-uppgift. Mer information om hur du beräknar om projekttidslinjer finns i [Beräkna om projekttidslinjer](../../../manage-work/projects/manage-projects/recalculate-project-timeline.md).

   Mer information om föregående projekt finns i [Skapa föregångare mellan projekt](../../../manage-work/tasks/use-prdcssrs/cross-project-predecessors.md).
