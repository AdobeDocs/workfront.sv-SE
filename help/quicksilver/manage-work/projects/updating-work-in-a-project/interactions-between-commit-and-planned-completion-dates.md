---
product-area: projects
navigation-topic: update-work-in-a-project
title: Interaktion mellan implementeringsdatumet och det planerade slutförandedatumet
description: Både planerat slutförande och implementeringsdatum anger när uppgiften ska slutföras. Men de skiljer sig åt på grund av vem som ställer in varje datum.
author: Alina
feature: Work Management
exl-id: 1709c60c-ac75-48eb-9226-ec2cf556ebf0
source-git-commit: 1eb1e919bede7e366956d8c0bd969329a641123f
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Interaktion mellan implementeringsdatumet och det planerade slutförandedatumet

<!--
this article has mostly information that is repeated from the articles linked from here. I left it in here for searchability's sake.
-->

Både planerat slutförande och implementeringsdatum anger när uppgiften ska slutföras. Men de skiljer sig åt på grund av vem som ställer in varje datum.

## Översikt över implementeringsdatum och planerat slutförandedatum

Planerade datum för slutförande och implementering finns för både uppgifter och problem.

Följande tabell innehåller information om skillnaden mellan datum för implementering och planerad slutförande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Bekräftelsedatum</td> 
   <td> <p>Bekräftelsedatum är det datum då den person som tilldelats en uppgift eller en utgåva manuellt beräknar att de har slutfört uppgiften eller utgåvan.</p> <p>Mer information om implementeringsdatum finns i <a href="../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md" class="MCXref xref">Genomför datumöversikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Planerat slutförandedatum</td> 
   <td> <p>Det planerade slutförandedatumet visas när projektägaren förväntar sig att aktiviteten eller utgåvan ska slutföras. Den kan antingen anges manuellt av projektägaren eller av vem som helst med behörigheten Hantera för uppgiften eller problemet, eller så kan den beräknas automatiskt av Adobe Workfront.</p> <p>Mer information om planerade slutförandedatum finns i <a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Översikt över den planerade slutförandedagen</a></p> </td> 
  </tr> 
 </tbody> 
</table>

## Interaktion mellan implementeringsdatumet och det planerade slutförandedatumet

När projektägaren skapar och tilldelar en uppgift eller ett problem får uppgiften eller problemet följande:

* Planerat slutförandedatum
* Inget implementeringsdatum

Den tilldelande som arbetar med uppgiften eller utgåvan kan uppdatera implementeringsdatumet manuellt eller automatiskt uppdatera det genom att acceptera att arbeta med det. Detta är ett visuellt sätt att visa projektägaren när det skulle vara realistiskt för dem att slutföra uppgiften eller problemet.

>[!TIP]
>
>Endast den som tilldelats kan uppdatera implementeringsdatumet för en uppgift eller utgåva.

Tilldelningsmottagaren som ändrar implementeringsdatumet ändrar inte automatiskt det planerade slutförandedatumet. Det motsatta är också sant: om du ändrar det planerade slutförandedatumet ändras inte implementeringsdatumet.

När implementeringsdatumet ändras meddelas projektägaren via ett Workfront-meddelande i appen om att ändringen har inträffat.

Om det datum för implementering som den tilldelade personen erbjuder kan accepteras av projektägaren, måste de manuellt uppdatera det planerade slutförandedatumet för aktiviteten för att visa vilken effekt den kan ha på tidslinjen i projektet. Ändringar av det planerade slutförandedatumet påverkar inte projekttidslinjen.

Mer information finns i följande artiklar:

* [Genomför datumöversikt](../../../manage-work/projects/updating-work-in-a-project/overview-of-commit-dates.md)
* [Uppdatera implementeringsdatum för aktiviteter och ärenden](../../../manage-work/projects/updating-work-in-a-project/update-commit-date-on-tasks-and-issues.md)
