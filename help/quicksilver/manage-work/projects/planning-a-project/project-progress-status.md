---
content-type: overview
product-area: projects
navigation-topic: plan-a-project
title: Översikt över status för projektförlopp
description: Adobe Workfront fastställer ett projekts förloppsstatus genom att undersöka projektets förlopp över dess tidslinje. Du kan konfigurera Workfront för att fastställa ett projekts villkor baserat på värdet för aktiviteternas förloppsstatus. Mer information om hur du konfigurerar projektvillkoren finns i artikeln Översikt över projektvillkor och villkorstyp.
author: Alina
feature: Work Management
exl-id: 922ca4cf-c526-4704-9966-de67b0c36a2a
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '383'
ht-degree: 0%

---

# Översikt över status för projektförlopp

Adobe Workfront fastställer ett projekts förloppsstatus genom att undersöka projektets förlopp över dess tidslinje. Du kan konfigurera Workfront för att fastställa ett projekts villkor baserat på värdet för aktiviteternas förloppsstatus. Mer information om hur du konfigurerar projektvillkoren finns i artikeln [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

Följande är statusvärdena för projekt i Workfront:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>I tid</td> 
   <td> <p>Om både Planerat och Beräknat slutförandedatum är tidigare än eller lika med projektets Planerat slutförandedatum, är projektets förloppsstatus <strong>I tid</strong>.</p> <p> <img src="assets/project-on-time-progress-status-350x69.png" style="width: 350;height: 69;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Risk</td> 
   <td> <p>När både beräknade och planerade slutförandedatum infaller i framtiden men senare än projektets planerade slutförandedatum och det beräknade slutförandedatumet infaller senare än det planerade slutförandedatumet, är projektets förloppsstatus <strong>Risk</strong>. </p> <p> <img src="assets/project-at-risk-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Bakom</td> 
   <td> <p>När både beräknade och planerade slutförandedatum ligger i framtiden men senare än projektets planerade slutförandedatum, men det beräknade slutförandedatumet inte är senare än det planerade slutförandedatumet, är projektets förloppsstatus <strong>Bakom</strong>.</p> <p> <img src="assets/project-behind-progress-status-350x67.png" style="width: 350;height: 67;"> </p> </td> 
  </tr> 
  <tr> 
   <td>Sena</td> 
   <td> 
    <ul> 
     <li> <p>Om projektet är färdigt och det faktiska slutförandedatumet är senare än det planerade slutförandedatumet, är projektets förloppsstatus <strong>Sena</strong>. </p> <p> <img src="assets/project-late-progress-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
     <li> <p>Om projektet inte är färdigt och projektets planerade slutförandedatum redan har inträffat, är projektets förloppsstatus <strong>Sena</strong>. </p> <p> <img src="assets/project-late-progress-status-incomplete-status-350x66.png" style="width: 350;height: 66;"> </p> </li> 
    </ul> </td> 
  </tr> 
 </tbody> 
</table>

Tänk på följande:

* Projektets beräknade slutförandedatum styrs av aktiviteten på den kritiska vägen med det senaste planerade slutförandedatumet.
* Projektets beräknade slutförandedatum styrs av aktiviteten på den kritiska sökvägen med det senaste beräknade slutförandedatumet.

Mer information om projektets kritiska sökväg finns i [Översikt över projektets kritiska sökväg](../../../manage-work/tasks/manage-tasks/critical-path.md).

Mer information om schemalagda slutförandedatum finns i [Översikt över planerat slutförandedatum för projekt, uppgifter och ärenden](../../../manage-work/projects/planning-a-project/project-projected-completion-date.md).
