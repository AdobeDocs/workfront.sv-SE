---
content-type: overview
product-area: projects
navigation-topic: task-duration
title: Översikt över aktivitetsvaraktighet och varaktighetstyp
description: Aktivitetens varaktighet är skillnaden mellan det planerade slutförandedatumet och det planerade startdatumet för aktiviteten. Varaktighet anger den tidsram som är tillgänglig för uppgiften att slutföras.
author: Alina
feature: Work Management
recommendations: noDisplay, noCatalog
exl-id: c81e485a-7e8c-4907-8e6c-9991681c3541
source-git-commit: 8d5006532e93dc687beb79e817b725f18b0c65d3
workflow-type: tm+mt
source-wordcount: '1677'
ht-degree: 0%

---

# Översikt över aktivitetsvaraktighet och varaktighetstyp

<!-- Audited: 12/2023 -->

<span class="preview">Den markerade informationen på den här sidan hänvisar till funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Efter de månatliga releaserna i Production finns samma funktioner även i produktionsmiljön för kunder som aktiverat snabba releaser. </span>

<span class="preview">Mer information om snabba releaser finns i [Aktivera eller inaktivera snabba releaser för din organisation](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/enable-fast-release-process.md). </span>

Aktivitetens varaktighet är skillnaden mellan det planerade slutförandedatumet och det planerade startdatumet för aktiviteten. Varaktighet anger den tidsram som är tillgänglig för uppgiften att slutföras.

En uppgifts varaktighetstyp identifierar relationen mellan antalet resurser som tilldelats en aktivitet, den totala ansträngningen och uppgiftens totala varaktighet.

## Översikt över aktivitetsvaraktighet

Om aktivitetens faktiska start- och slutförandedatum ligger utanför schemat för projektet, den primära tilldelaren eller standardschemat, är aktivitetens varaktighet noll.

>[!BEGINSHADEBOX]

**EXEMPEL**
Om du har ett schema som börjar kl. 9.00 och slutar kl. 12.00 och en aktivitet som schemaläggs att starta kl. 2:00 och avslutas kl. 17:00, är aktivitetens varaktighet noll.


>[!ENDSHADEBOX]

Följande två scenarier gäller vid beräkning av varaktighet i Adobe Workfront:

* Om en användare tilldelas uppgiften finns följande scenarier beroende på vilken miljö du använder:

   * I produktionsmiljön använder Workfront en av följande scheman, i den här exakta ordningen för beräkning av varaktighet:

   1. Workfront tar hänsyn till användarens schema.
   1. Om användaren inte är kopplad till ett schema, tar Workfront hänsyn till projektets tidsplan.
   1. Om projektet inte är kopplat till ett schema, tar Workfront hänsyn till systemets standardschema. Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

<div class="preview">

* I förhandsvisningsmiljön:

   1. Workfront tar hänsyn till antingen schemat för projektet eller den användare som tilldelats uppgiften.

      Din Workfront- eller gruppadministratör avgör vilket schema Workfront använder när en uppgift tilldelas en användare. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Om användaren eller projektet inte har något schema använder Workfront standardschemat.

      Stegen liknar det första scenariot efter att du har förstått vilket schema Workfront använder för att beräkna varaktighet.

</div>

* Om uppgiften har tilldelats flera användare:

   1. Workfront tar hänsyn till antingen projektplanen eller den primära uppdragstagarens tidsplan.

      Din Workfront- eller gruppadministratör avgör vilket schema Workfront använder när en uppgift tilldelas flera användare. Mer information finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

   1. Om den primära tilldelaren eller projektet inte har något schema använder Workfront standardschemat.

  Stegen liknar det första scenariot efter att du har förstått vilket schema Workfront använder för att beräkna varaktighet.

>[!NOTE]
>
>När hänsyn tas till den primära tilldelades tid för ett projekt kan aktivitetens planerade datum ändras, men aktivitetens varaktighet är densamma. Mer information om hur du tar hänsyn till den primära tilldelningens tid när du planerar ett projekt finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Den ursprungliga varaktigheten för en överordnad aktivitet

Ursprunglig varaktighet för en aktivitet är den varaktighet en aktivitet hade innan den blev en överordnad aktivitet, i minuter.

När en aktivitet blir överordnad, kommer varaktigheten mellan det planerade startdatumet för den tidigaste underordnade och det planerade slutförandedatumet för den senaste underordnade aktiviteten att räknas upp till den överordnade aktiviteten och bli varaktigheten för den överordnade aktiviteten. Detta ersätter varaktigheten för den ursprungliga aktiviteten.

Mer information finns i [Översikt över aktivitetens ursprungliga varaktighet och ursprungliga planerade timmar](/help/quicksilver/manage-work/tasks/task-information/task-original-duration-and-original-planned-hours.md).

## Tidsenheter för aktivitetsvaraktighet

Du kan ange aktivitetens varaktighet både som vanlig tid och som förfluten tid mellan de planerade startdatumen och de planerade avslutsdatumen.

När du uppdaterar varaktigheten för uppgifter i en lista kan du använda följande förkortningar för att ange tidsenheter i Workfront:

| Tidsenhet | Förkortning |
|---|---|
| Minuter | M |
| Timmar | H |
| Dagar. Det här är standardinställningen. | D |
| Veckor | B |
| Månader | T, MO |
| Förflutna minuter | EM |
| Förflutna timmar | EH |
| Förflutna dagar | ED |
| Förflutna veckor | FV |
| Förflutna månader | ET |

{style="table-layout:auto"}

>[!BEGINSHADEBOX]

**EXEMPEL**

Om du vill ange att varaktigheten för en uppgift är 3 Förfluten dag skriver du&quot;3 ED&quot; i fältet Varaktighet i en uppgiftslista.  Du kan också välja önskat alternativ för Tidsenhet för varaktighet i den nedrullningsbara menyn när du redigerar en uppgift eller i delen Aktivitetsinformation. Mer information om hur du redigerar uppgifter finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).


>[!ENDSHADEBOX]

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: stays QS only forever; for the pictures below: make the first one classic at preview time and the second one stays QS always. The second one is yellow >> take out at 21.2 production!!)</p>
-->

![](assets/duration-elapsed-days-tasks-nwe-350x282.png)

Tänk på följande när du anger varaktigheten för en uppgift:

* Förfluten tid är en tidsenhet för en uppgifts varaktighet. Det är tiden mellan det planerade startdatumet och det planerade slutförandedatumet för en aktivitet som omfattar helger, helger och ledig tid. Med andra ord är förfluten tid en del av kalenderdagarna.
* Dagar representerar de arbetsdagar som är definierade i systemet och kan konfigureras under Konfigurera. I de flesta fall består en dag av 8 timmar.
* Vanlig tid (dagar eller arbetsdagar) tar hänsyn till helger, helger och ledig tid och utesluter dem från uppgiftens varaktighet.
* När du anger varaktigheten för en uppgift i veckor, beräknas varaktigheten i dagar och timmar i Workfront baserat på de inställningar för Normal arbetsdag per vecka och Normal timmar per arbetsdag som du har angett av Workfront-administratören under Projektinställningar i Konfigurera.
* Workfront använder standardlängden på fyra veckor i en månad vid beräkning av varaktighet i månader.

## Översikt över typen av aktivitetsvaraktighet

Genom att hantera varaktighetstypen för en aktivitet kan du ange konsekventa resurstilldelningar baserat på uppgiftens behov.

Varaktighetstyp hjälper dig att svara på följande frågor:

* Hur upptagen kommer vi att vara?
* Hur stort är jobbet?
* Hur lång tid kommer det att ta?

![duration_type_triangle.png](assets/duration_type_triangle.png)

## Definiera varaktighetstyper

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="row"><p><strong>Varaktighetstyp</strong></p></th> 
   <th scope="col"> <p><strong>Funktion</strong> </p> </th> 
   <th scope="col"> <p><strong>Hur resurser påverkar det</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <th scope="col"> <p><strong>Beräknad tilldelning</strong> </p> </th> 
   <td scope="col"> <p>Beräknar allokeringsprocenten för varje tilldelad för en uppgift. </p> <p>När du väljer den här varaktighetstypen kan du ange individuell Varaktighet och Planerade timmar för uppgiften. Workfront dividerar de planerade timmarna med antalet timmar i aktivitetens varaktighet och med antalet resurser som tilldelats aktiviteten för att beräkna allokeringen för varje tilldelad.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/calculated-assignment.md" class="MCXref xref">Översikt över varaktighetstyp: Beräknat uppdrag</a>.</p> </td> 
   <td scope="col">Varaktighet och Planerade timmar ändras inte när du lägger till eller tar bort tilldelningar för aktiviteten. </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Beräknat arbete</strong> </p> </th> 
   <td scope="col"> <p>Anger de planerade timmarna (mängden arbetsinsats) som krävs för att aktiviteten ska slutföras.</p> <p>Används normalt när resurserna som tilldelats aktiviteten tilldelas för aktivitetens hela varaktighet.</p> <p>När du väljer den här varaktighetstypen kan du ange en enskild Varaktighet för uppgiften. Workfront beräknar de planerade timmarna för aktiviteten genom att multiplicera antalet dagar i tidsperioden med antalet arbetstimmar i tidsplanen och antalet tilldelningar av aktiviteten. </p> <p>Du kan ändra allokeringsprocenten för varje tilldelad till uppgiften manuellt, vilket minskar antalet planerade timmar.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/calculated-work.md" class="MCXref xref">Översikt över varaktighetstyp: Beräknat arbete</a>.</p> </td> 
   <td scope="col"> <p>Planerade timmar ökar när tilldelningar läggs till i uppgiften. </p> <p>Planerade timmar minskar när tilldelningar tas bort från aktiviteten.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Ansträngningsstyrd</strong></p> </th> 
   <td scope="col"> <p>Bestämmer antalet planerade timmar baserat på antalet resurser.</p> <p>När du väljer den här varaktighetstypen kan du ange en enskild Varaktighet för uppgiften. Workfront beräknar de planerade timmarna för aktiviteten genom att multiplicera antalet dagar i tidsperioden med antalet arbetstimmar i tidsplanen och dividera antalet med antalet tilldelningar för aktiviteten. </p> <p>Du kan ändra allokeringsprocenten för varje tilldelad till uppgiften manuellt, men antalet planerade timmar är detsamma.</p> <p>Mer detaljerad information finns i <a href="../../../manage-work/tasks/taskdurtn/effort-driven.md" class="MCXref xref">Översikt över varaktighetstyp: Ansträngningsstyrd</a>.</p> </td> 
   <td scope="col"> <p>Planerade timmar ökar när tilldelningar tas bort från aktiviteten.</p> <p>Planerade timmar minskar när tilldelningar läggs till i aktiviteten. </p> <p>Varaktigheten ändras inte, oavsett antalet tilldelningar eller deras schema. </p> <p>Varaktigheten är lika med Planerade timmar. Planerad varaktighet är lika med Planerade timmar dividerat med antalet tilldelningar.</p> </td> 
  </tr> 
  <tr> 
   <th scope="col"> <p><strong>Enkel</strong> </p> </th> 
   <td scope="col"> <p>Bestämmer antalet planerade timmar och varaktigheten (som är densamma för den här varaktighetstypen) baserat på det antal timmar som varje tilldelad tilldelas. </p> <p>Workfront beräknar de planerade timmarna genom att addera de tilldelade timmarna för varje tilldelad. </p> <p>Du kan ändra antalet timmar som varje tilldelad har tilldelats manuellt, och antalet planerade timmar och mängden varaktighet ändras i enlighet med detta. Om du väljer ett totalt antal tilldelade timmar för alla tilldelningar, delas det antalet jämnt mellan varje tilldelad.</p> <p>Mer information finns i <a href="../../../manage-work/tasks/taskdurtn/simple-duration-type.md" class="MCXref xref">Översikt över varaktighetstypen: Enkel</a>.</p> </td> 
   <td scope="col"> <p>Timmar fördelas jämnt mellan tilldelningar om du väljer ett totalt antal tilldelade timmar. Som projektledare kan du dock justera timmarna manuellt för varje tilldelad. </p> <p>Du kan antingen redigera Planerade timmar och Varaktighet för en aktivitet med en enkel varaktighetstyp infogad eller på aktivitetsnivå. </p> <p>Om ett smidigt team tilldelas till en uppgift anges varaktighetstypen automatiskt till Enkel och kan inte ändras. Uppgiftens varaktighet för ett team måste vara längre än 0 minuter.</p> </td> 
  </tr> 
 </tbody> 
</table>

## De nya aktiviteternas varaktighetstyp

Den nya aktivitetens varaktighetstyp matchar den varaktighetstyp som är inställd i systemet. Standardtypen för varaktighet är Beräknad tilldelning. Workfront-administratören eller en gruppadministratör kan uppdatera standardvaraktighetstypen för ditt system eller för gruppen som är kopplad till projektet. Mer information finns i [Konfigurera uppgifter och utgåvinställningar för hela systemet](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-task-issue-preferences.md).

## Ändra varaktighetstypen för en aktivitet

Mer information om hur du ändrar varaktighetstypen för en aktivitet finns i [Uppdatera varaktighetstypen för en aktivitet](../../../manage-work/tasks/taskdurtn/update-duration-type-of-task.md).
