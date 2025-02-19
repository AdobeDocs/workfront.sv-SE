---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över status för projektförlopp
description: Adobe Workfront fastställer ett projekts förloppsstatus genom att undersöka projektets förlopp över dess tidslinje. Du kan konfigurera Workfront för att fastställa ett projekts villkor baserat på värdet för aktiviteternas förloppsstatus. Läs mer om status för projektförlopp i den här artikeln.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: d85ccb9dbef343ecc8808412e89264b3ea6ab25e
workflow-type: tm+mt
source-wordcount: '390'
ht-degree: 0%

---

# Översikt över status för projektförlopp

<!--Audited: 12/2023-->

Adobe Workfront fastställer ett projekts förloppsstatus genom att undersöka projektets förlopp över dess tidslinje. Du kan konfigurera Workfront för att fastställa ett projekts villkor baserat på värdet för aktiviteternas förloppsstatus. Mer information om hur du konfigurerar projektvillkoren finns i artikeln [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Följande är statusvärdena för projekt i Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>I tid</td> 
   <td> Ett projekts förloppsstatus är <strong>Vid tid</strong> om:<ul><li>Om både Planerat och Beräknat slutförandedatum är tidigare än eller lika med projektets Planerat slutförandedatum</li></ul> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td> Ett projekts förloppsstatus är <strong>Vid risk</strong> om <strong>alla</strong> av följande är sanna:<ul><li>Både beräknade och planerade slutförandedatum finns i framtiden</li><li> Det beräknade slutförandedatumet är senare än både det planerade slutförandedatumet och det planerade slutförandedatumet </li></ul><p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Bakom</td> 
   <td> Ett projekts förloppsstatus är <strong>Bakom</strong> om <strong>alla</strong> av följande är sanna:<ul><li>Både beräknade och planerade slutförandedatum finns i framtiden</li><li> Både beräknade och planerade slutförandedatum är senare än projektets planerade slutförandedatum</li><li> Det beräknade slutförandedatumet är inte senare än det planerade slutförandedatumet</li></ul> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Sena</td> 
   <td> 
     Ett projekts förloppsstatus är <strong>sen</strong> om <strong>något</strong> av följande är sant:<ul><li>Projektet är färdigt och det faktiska slutförandedatumet är senare än det planerade slutförandedatumet <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Projektet är inte färdigt och projektets planerade slutförandedatum har redan inträffat <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tänk på följande:

* Projektets beräknade slutförandedatum styrs av aktiviteten på den kritiska vägen med det senaste planerade slutförandedatumet.
* Projektets beräknade slutförandedatum styrs av aktiviteten på den kritiska sökvägen med det senaste beräknade slutförandedatumet.

Mer information om projektets kritiska sökväg finns i [Översikt över projektets kritiska sökväg](../../../manage-work/tasks/manage-tasks/critical-path.md).

Mer information om schemalagda slutförandedatum finns i [Översikt över planerat slutförandedatum för projekt, uppgifter och problem](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
