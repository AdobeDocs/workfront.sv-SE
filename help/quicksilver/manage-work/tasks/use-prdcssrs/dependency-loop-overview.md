---
content-type: overview
product-area: projects
navigation-topic: use-predecessors
title: Översikt över uppgiftsberoendeloop
description: När du lägger till föregående relationer till uppgifter kan du stöta på beroendeloopar. Mer information om föregående aktiviteter finns i Översikt över föregående aktiviteter.
author: Alina
feature: Work Management
exl-id: 142e9637-841c-43d1-b297-e42c28a9e010
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '244'
ht-degree: 0%

---

# Översikt över uppgiftsberoendeloop

När du lägger till föregående relationer till uppgifter kan du stöta på beroendeloopar. Mer information om föregående aktiviteter finns i [Översikt över föregående aktiviteter](../../../manage-work/tasks/use-prdcssrs/predecessors-overview.md).

## Översikt över beroendeloop

Beroendeslingor inträffar när du har två eller flera uppgifter som är beroende av varandra och som ska slutföras. Adobe Workfront tillåter inte att du skapar en föregående relation mellan uppgifter om den skapar en beroendeloop.

**Exempel:** Uppgift 2 är en föregångare till Uppgift 1, vilket innebär att du måste slutföra Uppgift 2 innan du kan börja arbeta med Uppgift 1.

Om du försöker göra Task 1 till en föregångare till Task 2 får du ett fel med en beroendeloop eftersom du inte kan starta Task 1 förrän Task 2 har slutförts, men uppgift 2 kan inte startas förrän Task 1 har slutförts.

![](assets/dependency-loop-error-message-350x209.png)

![](assets/dependency-loop-in-task-list-nwe-350x97.png)

## Överväganden om beroendeloopar

* Beroendeslingor kan omfatta mer än två åtgärder. Ibland skapas en beroendeslinga av det antal överordnade aktiviteter som du ansluter till en föregående relation.
* En beroendeloop kan också inträffa om du försöker göra en överordnad till en underordnad.
* Om det är en beroendeloop kan du inte spara uppgifterna eller projektet. För att kunna åtgärda beroendeloopen måste du omvärdera den föregående relationen mellan de uppgifter som anges i felmeddelandet och ta bort konflikterna innan du kan spara uppgifterna eller projektet.

 
