---
content-type: overview;reference
product-area: projects
navigation-topic: use-predecessors
title: Översikt över aktivitetsberoendetyper
description: Beroendetyper refererar till föregående relationer mellan uppgifter. De definierar när den beroende aktiviteten kan starta eller slutföras baserat på början eller slutet av dess föregångare.
author: Alina
feature: Work Management
exl-id: 30d1c60d-0632-4a32-b7e7-a9f8e81bf727
source-git-commit: 7427706f6ce6cad3370b91269c1b4e7a10ed09f9
workflow-type: tm+mt
source-wordcount: '315'
ht-degree: 0%

---

# Översikt över typer av uppgiftsberoenden

<!-- Audited: 12/2023 -->

Beroendetyper refererar till föregående relationer mellan uppgifter. De definierar när den beroende aktiviteten kan starta eller slutföras baserat på början eller slutet av dess föregångare.

>[!IMPORTANT]
>
>Adobe Workfront begränsar inte de beroende aktiviteterna från att starta eller slutföra baserat på beroendetyper om inte de föregående relationerna upprätthålls. Mer information om hur du framtvingar föregångare finns i [Tvinga föregångare](../../../manage-work/tasks/use-prdcssrs/enforced-predecessors.md).

Du måste ange beroendetypen för en föregående relation när du upprättar relationen mellan dina uppgifter.

Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

Följande är Workfront beroendetyper:

* **Slutför-Start (fs)**: Föregående-aktiviteten måste avslutas innan den beroende aktiviteten kan startas. Det här är standardberoendetypen som används när ingen annan beroendetyp har angetts.
* **Slutför (ff)**: Föregående-aktiviteten måste avslutas innan den beroende aktiviteten kan slutföras.
* **Start-Start (ss)**: Föregående aktivitet måste startas innan den beroende aktiviteten kan startas. Du kan inte starta den beroende aktiviteten om inte föregående aktivitet har startats.
* **Start-Finish (sf)**: Föregående aktivitet måste startas innan den beroende aktiviteten kan slutföras. Du kan starta den beroende aktiviteten innan föregångaren startas, men du kan inte slutföra den om inte föregående aktivitet har startats.
* **Schemalagd-Start (sd)**: Detta schemalägger en aktivitet som Slutför-Start, men den faktiska tvingande typen är Slutför. När du använder det här schemaläggs den beroende aktiviteten att starta efter att föregående aktivitet har slutförts. Tvingande åtgärder gör det dock så att den beroende aktiviteten kan starta när som helst, men den kan inte slutföras förrän föregående aktivitet är klar.

>[!NOTE]
>
>Förkortningarna för Beroendetyper används i uppgiftslistor för att definiera föregående relationer. Mer information finns i [Exempel på föregående värden i en uppgiftslista](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md#examples-of-predecessor-values-in-a-task-list) i [Översikt över föregående aktiviteter](/help/quicksilver/manage-work/tasks/use-prdcssrs/predecessors-overview.md).

