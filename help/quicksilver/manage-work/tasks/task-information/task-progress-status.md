---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över status för aktivitetsstatus
description: Adobe Workfront fastställer förloppsstatusen för en aktivitet genom att undersöka förloppet för aktiviteten över dess tidslinje. Du kan konfigurera Workfront för att fastställa ett projekts villkor baserat på värdet för aktiviteternas förloppsstatus. Mer information om hur du konfigurerar projektvillkoren finns i artikeln Översikt över projektvillkor och villkorstyp.
author: Alina
feature: Work Management
exl-id: 38e5f89e-bdfa-433c-9371-3c3003ada3a3
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '777'
ht-degree: 0%

---

# Översikt över status för åtgärdsförlopp

<!-- Audited: 1/2024 -->

Adobe Workfront fastställer förloppsstatusen för en aktivitet genom att undersöka förloppet för aktiviteten över dess tidslinje. Du kan konfigurera Workfront för att fastställa ett projekts villkor baserat på värdet för aktiviteternas förloppsstatus. Mer information om hur du konfigurerar projektvillkoren finns i artikeln [Översikt över projektvillkor och villkorstyp](../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md).

## Kriterier som bestämmer aktiviteternas förloppsstatus

Mer information om ett projekts förloppsstatus finns i [Översikt över projektförloppsstatus](../../../manage-work/projects/planning-a-project/project-progress-status.md).

Mer information om hur du spårar förloppet för dina uppgifter finns i [Översikt över läget Uppföljning](../../../manage-work/tasks/task-information/task-tracking-mode.md).

Följande kriterier bestämmer förloppsstatusen för en uppgift:

<table> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Förloppsstatus</strong> </p> </th> 
   <th> <p><strong>Kontrollerar villkor</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr valign="top"> 
   <td scope="col"> <p> </p> <p><strong>I tid</strong> </p> </td> 
   <td scope="col"> <p>En aktivitet anses vara <strong>On Time</strong> när alla planerade datum matchar de planerade datumen. Den här statusen kan även innebära att projektet ligger före schemat och att de planerade datumen kan ligga före de planerade datumen.</p> <p>Mer information om beräknade datum finns i <a href="../../../manage-work/projects/planning-a-project/project-projected-completion-date.md" class="MCXref xref">Översikt över planerat slutförandedatum för projekt, uppgifter och problem</a>.</p> <p>Mer information om schemalagt slutförandedatum för aktiviteten finns i följande artiklar:</p> 
    <ul> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-start-date.md" class="MCXref xref">Översikt över aktivitetens planerade startdatum</a> </p> </li> 
     <li> <p><a href="../../../manage-work/tasks/task-information/task-planned-completion-date.md" class="MCXref xref">Översikt över aktiviteten Planerat slutförandedatum</a> </p> </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><p></p> <p><strong>Vid risk</strong> </p> </td> 
   <td><p>En aktivitet betraktas som <strong>Vid risk</strong> när det beräknade slutförandedatumet är senare än det planerade slutförandedatumet och senare än det planerade slutförandedatumet. Detta kan inträffa när en aktivitet har begränsningen <strong>Måste avslutas den</strong> eller <strong>måste starta den</strong>, men procentandelen slutförd eller föregående relationer för aktiviteten visar att den inte kan avslutas eller starta på de angivna datumen. </p><p> Om du anger aktivitetsbegränsningen till <strong>Måste avslutas den</strong> anges det planerade slutförandedatumet manuellt till ett visst datum. Det planerade slutförandedatumet matchar i det här fallet det planerade slutförandedatumet. När det gäller den här begränsningen analyserar Workfront aktiviteten för att beräkna när den ska slutföras baserat på procentandelen slutförd. Beräkningen sparas som beräknat förfallodatum. Om det beräknade förfallodatumet infaller efter det planerade slutförandedatumet riskerar aktiviteten att bli försenad. </p> <p> Om du anger aktivitetsbegränsningen till <strong>Måste starta den</strong> anges det planerade startdatumet manuellt till ett visst datum. Det planerade startdatumet matchar i det här fallet det planerade startdatumet. När det gäller den här begränsningen analyserar Workfront uppgiften för att beräkna när den ska börja baserat på dess föregångarrelationer. Den här beräkningen lagras som det beräknade startdatumet. Om det finns en framtvingad föregångare som inte tillåter att aktiviteten startar det angivna startdatumet, kan det beräknade startdatumet ligga efter det planerade slutförandedatumet. Uppgiften riskerar att bli sen. </p> <p>Obs! Oftast matchar beräknade datum beräknade datum, förutom när <strong>måste börja den</strong> eller <strong>måste avslutas den</strong> används. I dessa fall fortsätter beräknade datum att beräknas baserat på procent färdigt och andra faktorer (tidigare relationer), medan de planerade datumen måste matcha de planerade datumen som har ställts in manuellt.</p> </td> 
  </tr> 
  <tr> 
   <td> <p><strong>Bakom</strong> </p> </td> 
   <td> <p>En aktivitet anses ligga <strong>bakom</strong> när det beräknade slutförandedatumet är senare eller lika med det planerade slutförandedatumet och tidigare än det planerade slutförandedatumet.</p> <p>Det planerade slutförandedatumet är en realtidsvy över när aktiviteten ska slutföras baserat på tidigare förlopp. Även om aktiviteten startades för sent anses den inte vara försenad ännu, eftersom de planerade och planerade slutförandedatumen fortfarande ligger kvar i framtiden och aktiviteten kan fortfarande slutföras i tid.</p> <p>Obs! Statusen <strong>Bakom</strong> och <strong>Vid risk</strong> är nästan identiska. <strong>Vid risk</strong> indikerar dock att det finns vissa obligatoriska aktivitetsbegränsningar (Måste sluta på, Måste starta på, fasta datum) på ett eller båda de planerade datumen. Om det inte finns några tvingande begränsningar för aktiviteten är de beräknade datumen samma som de beräknade datumen och återspeglar systemberäkningen för slutförandedatumet baserat på aktivitetens aktuella förlopp. Aktiviteten anses inte vara sen ännu eftersom de planerade och planerade slutförandedatumen fortfarande ligger kvar i framtiden och aktiviteten kan fortfarande slutföras i tid.<br>Mer information om Planerade och beräknade datum finns i <a href="../../../manage-work/tasks/task-information/differentiate-projected-estimated-dates.md" class="MCXref xref">Översikt över beräknade och beräknade datum </a>.</p> </td> 
  </tr> 
  <tr valign="top"> 
   <td> <p><strong>Sena</strong> </p> </td> 
   <td> <p>En aktivitet är <strong>sen</strong> när det planerade slutförandedatumet infaller före dagens datum.<br></p> </td> 
  </tr> 
 </tbody> 
</table>

<!--hiding this because some users find the images confusing, as they don't really show the dates mentioned in the descriptions above. Keep the pictures though, in case some users will complain that we hid them. 

## How task Progress Status updates over time

The different date types in our projects tell us how tasks are progressing over time:

* On Time

  ![On time progress status](assets/on-time-progress-status-350x233.png)

* At Risk

  ![At risk progress status](assets/at-risk-progress-status-350x233.png)

* Behind

  ![Behind progress status](assets/behind-progress-status-350x233.png)

* Late

  ![Late progress status](assets/late-progress-status-350x233.png)

-->
