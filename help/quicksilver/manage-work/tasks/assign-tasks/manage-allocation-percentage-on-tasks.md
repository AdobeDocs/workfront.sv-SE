---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Hantera användar- eller rollallokeringsprocent för uppgifter
description: Allokeringsprocenten representerar den tid en tilldelad resurs är planerad att arbeta med en aktivitet på en dag. Det är procentandelen av en arbetsdag (enligt användaren eller projektschemat) som en resurs tilldelas under aktivitetens varaktighet.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 830ad0411084844ace1e1e543c3ebefcb558af80
workflow-type: tm+mt
source-wordcount: '431'
ht-degree: 0%

---

# Hantera användar- eller rollallokeringsprocent för uppgifter

Allokeringsprocenten representerar den tid en tilldelad resurs är planerad att arbeta med en aktivitet på en dag. Det är procentandelen av en arbetsdag (enligt användaren eller projektschemat) som en resurs tilldelas under aktivitetens varaktighet.

>[!NOTE]
>
>När du tilldelar användare arbetstid påverkar tillgängligheten enligt sina scheman de planerade och planerade datumen för uppgifter och problem. Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Nytt: Standard</p> 
   <p>Aktuell: Arbete eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Redigera åtkomst till uppgifter</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörighet till uppgiften</p> <p>Redigera behörigheter för att uppdatera allokeringsprocent i rutan Redigera uppgift</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Överväganden om att ändra procentallokeringar för uppgifter

* Användarna tilldelas som standard en lika lång procentandel av tiden till de uppgifter de tilldelas.
* Du kan ändra allokeringsprocenten för användare och jobbroller som tilldelats uppgifter manuellt endast när uppgiftens varaktighetstyp är Beräknad arbets- eller aktivitetsstyrd.

  Mer information finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Du kan inte ändra procentallokeringen för team som tilldelats aktiviteter.
* Du kan inte ändra procentallokeringen för användare och jobbroller som är tilldelade utgåvor.

## Ändra användar- eller rollprocentallokering för en uppgift

1. Gå till en aktivitet vars resurser du ändrar procentallokeringen för.
1. Klicka på **Mer**-menyn ![](assets/qs-more-icon-on-an-object.png) bredvid namnet på aktiviteten och klicka sedan på **Redigera**.

   eller

   Klicka på området **Uppdrag** i uppgiftshuvudet och klicka sedan på **Avancerat**.

1. Kontrollera att aktivitetens **varaktighetstyp** är något av följande:

   * Beräknat arbete
   * Ansträngningsstyrd

   >[!TIP]
   >
   >* Workfront använder följande formel för beräkning av tilldelningens varaktighet för varje tilldelad: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* För den enkla varaktighetstypen kan du beräkna antalet tilldelade timmar för varje resurs, inte allokeringsprocenten.

1. Klicka på **Tilldelningar** och ändra sedan **Allokeringar** för varje uppgiftstilldelad.

   Du kan bara ändra allokeringsprocenten för användar- och jobbrolltilldelningar.

   Du kan inte ändra allokeringsprocenten för ett team som tilldelats en aktivitet.

   ![Ändra allokeringsprocent](assets/advanced-assignments-allocation-percentage.png)

1. Klicka på **Spara**.
