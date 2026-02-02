---
content-type: overview
product-area: projects
navigation-topic: task-information
title: Översikt över projektets Procent färdigt
description: Värdet för Procent färdigt för ett projekt beräknas baserat på aktiviteternas planerade varaktighet eller planerade timmar i projektet. Din Adobe Workfront-administratör eller en gruppadministratör definierar vilket värde som ska beaktas vid beräkningen av procentandelen färdig i ditt system när de konfigurerar information i området Projektinställningar. Mer information om hur du konfigurerar projektinställningar finns i Konfigurera systemomfattande projektinställningar.
author: Alina
feature: Work Management
exl-id: d2395569-9fe5-42e7-a392-cff49eb519d9
source-git-commit: ef64e5c8169fd0a12d303c17649a20400ccbeb58
workflow-type: tm+mt
source-wordcount: '819'
ht-degree: 0%

---

# Översikt över Procent färdigt i projekt

<!-- Audited 01/2024 -->

Värdet för Procent färdigt för ett projekt beräknas baserat på aktiviteternas varaktighet eller planerade timmar i projektet. Din Adobe Workfront-administratör eller en gruppadministratör definierar vilket värde som ska beaktas vid beräkningen av procentandelen färdig i ditt system när de konfigurerar information i området Projektinställningar.

Mer information om hur du konfigurerar projektinställningar finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Procent färdigt för en överordnad aktivitet baseras på varaktigheten eller planerad timme för var och en av dess underaktiviteter.

På samma sätt baseras Procent färdigt för ett projekt på varaktigheten eller planerad tid för varje huvuduppgift i projektet.

De huvudsakliga uppgifterna är de överordnade och fristående uppgifterna som inte har några underordnade.

>[!TIP]
>
>Huvudaktiviteter är inte indragna i en projektplan.

## Hur Workfront beräknar Procent färdigt

### Uppdatera Procent färdigt för en uppgift {#update-the-percent-complete-on-a-task}

Du kan ändra procentandelen färdigt för en uppgift manuellt. Detta är inte en beräkning.

Workfront använder procentandelen färdigt för en enskild uppgift för att beräkna procentandelen färdigt för den överordnade uppgiften eller procentandelen färdigt för projektet.

Mer information om hur du uppdaterar procentandelen färdigt för en aktivitet finns i [Visa och uppdatera procent färdigt för aktiviteter](../../../manage-work/projects/updating-work-in-a-project/view-update-percent-complete-for-tasks.md).

### Hur Workfront beräknar Procent färdigt för en överordnad uppgift {#how-workfront-calculates-percent-complete-on-a-parent-task}

Beroende på vad din Workfront- eller gruppadministratör har valt i projektinställningarna på system- eller gruppnivå beräknas procentandelen färdig för en överordnad aktivitet antingen utifrån aktiviteternas varaktighet eller planerade timmar.

Tänk på följande scenarier:

* Om systemet beräknar procentandelen slutförd baserat på Planerade timmar beräknas procentandelen slutförd för den överordnade aktiviteten enligt följande formel:

  `Parent Task Percent Complete = (((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of Parent)*100`

  De totala planerade timmarna för den överordnade representerar summan av alla planerade timmar för var och en av de underordnade.

  ![Projekt med aktiviteter i procent slutförda och planerade timmar](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

* Om systemet beräknar procentandelen slutförd baserat på Varaktighet beräknas den överordnade aktivitetens procent slutfört med följande formel:

  `Parent Task Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/ Total Duration of Parent)*100`

  ![Projekt med aktiviteter i procent klart och tidsberäkning](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!IMPORTANT]
  >
  >Den överordnade uppgiftens totala varaktighet är den sammanlagda tiden för de underordnade aktiviteterna. En överordnad aktivitet med två underordnade objekt som har en varaktighet på 1 dag och 2 dagar har till exempel en total varaktighet på 3 dagar, även när de två underordnade kan starta samma dag.


### Hur Workfront beräknar Procent färdigt i ett projekt {#how-workfront-calculates-percent-complete-on-a-project}

Beroende på vad din Workfront- eller gruppadministratör har valt i Projektinställningar på system- eller gruppnivå beräknas procentandelen slutfört för ett projekt baserat på varaktigheten eller planerad timme för de huvudsakliga aktiviteterna i projektet.

* Om systemet beräknar procentandelen slutförd baserat på Planerade timmar beräknas projektprocenten som slutförd med följande formel:

  `Project Percent Complete =(((Task 1 Planned Hours * Task 1 Percent Complete) + (Task 2 Planned Hours * Task 2 Percent Complete))/Total Planned Hours of the Project)*100`

  Projektets totala planerade timmar är summan av de planerade timmarna för alla huvuduppgifter i projektet.

  ![Projekt med aktiviteter i procent slutförda och planerade timmar &#x200B;](assets/project-with-tasks-percent-complete-planned-hours-calculation.png)

  >[!NOTE]
  >
  >Aktivitet 1 eller Aktivitet 2 kan bara vara överordnade uppgifter eller fristående uppgifter. De underordnade uppgifterna Planerade timmar och Procent färdigt används inte i den här beräkningen.

* Om systemet beräknar procentandelen slutförd baserat på Varaktighet beräknas projektprocenten slutförd med följande formel:

  `Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

  >[!IMPORTANT]
  >
  >Projektets längd är den totala längden av alla varaktigheter för de huvudsakliga aktiviteterna som visar ett procenttal färdigt. Ett projekt med en fristående aktivitet med en varaktighet på 2 dagar och en överordnad aktivitet med en varaktighet på 5 dagar som har haft arbetet slutfört på dem får till exempel en total varaktighet på 7 dagar, även om de två aktiviteterna kan starta på samma dag.

  ![Projekt med aktiviteter i procent klart och tidsberäkning](assets/project-with-tasks-percent-complete-duration-calculation.png)

  >[!NOTE]
  >
  >Aktivitet 1 eller Aktivitet 2 kan bara vara överordnade uppgifter eller fristående uppgifter. De underordnade aktiviteterna Varaktighet och Procent färdigt används inte i den här beräkningen.

## Exempel på Procent färdigt i ett projekt med Varaktighet

När du använder varaktigheten för aktiviteterna för att beräkna procentandelen färdigt i ett projekt ska du tänka på följande exempel:

![Projekt med aktiviteter i procent klart och tidsberäkning](assets/project-with-tasks-percent-complete-duration-calculation.png)

Följande information används för att beräkna hur stor del av projektet som har slutförts

* Procent färdigt för den fristående aktiviteten (aktivitet 1 - 20 %)
* Procent färdigt för den överordnade aktiviteten (Aktivitet 2 - 25 %)
* Aktivitetens varaktighet 1 (5 dagar)
* Aktivitetens varaktighet 2 (2 dagar)
* Projektets längd (7 dagar)


Så här beräknar du procentandelen färdigt av projektet med Varaktighet:

`Project Percent Complete = (((Task 1 Duration * Task 1 Percent Complete) + (Task 2 Duration * Task 2 Percent Complete))/Duration of the Project)*100`

eller

`(((5*0.2)+(2*0.25))/7)*100= 21.43%`


<!--drafted, this was the old example:

When using the Planned Duration of the tasks to calculate the percent complete of a project, consider the following example:

percent_complete_on_project_example.png

Only the parent task (Task 1) and the standalone task (Task 8) are used to calculate the percent complete of the project.

The secondary parents of Task 1 are used to calculate the percent complete of the main parent (Task 1).

To calculate the percent complete of the main parent (Task 1), first calculate the percent complete of its secondary parents:

Task 5 Percent Complete = ((14 * 0.75 + 12 * 0.25)/(12 + 14))*100 = 51.92%

Task 2 Percent Complete = ((5 * 0.7 + 2 * 0.5)/(5 + 2))*100 = 64.29 %

Then, to calculate the percent complete of the main parent (Task 1), use the following formula:

Task 1 Percent Complete =((56 * 0.5192 + 7 * 0.6429)/63)*100 = 53.29%

To calculate the percent complete of the project, you will need to have the following numbers ready:

Task 1 Duration (63 hours) and Percent Complete (53.29%)
Task 8 Duration (100 hours) and Percent Complete (4%)
Now, to calculate the percent complete of the project, use the following formula:

Project Percent Complete =((100 * 0.04 + 63 * 0.5329))/163)*100 = 23.05%
-->
