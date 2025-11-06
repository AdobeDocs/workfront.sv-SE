---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Hantera användar- eller rollallokeringsprocent för aktiviteter
description: Allokeringsprocenten representerar den tid en tilldelad resurs är planerad att arbeta med en aktivitet på en dag. Det är procentandelen av en arbetsdag (enligt användaren eller projektschemat) som en resurs tilldelas under aktivitetens varaktighet.
author: Lisa
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: 798e9ee9862b34653730c07acc9c48b901b98e63
workflow-type: tm+mt
source-wordcount: '509'
ht-degree: 0%

---

# Hantera användar- eller rollallokeringsprocent för uppgifter

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->

<div class="preview">

Den markerade informationen på den här sidan avser funktioner som ännu inte är allmänt tillgängliga. Det är bara tillgängligt i förhandsvisningsmiljön för alla kunder. Samma funktioner är också tillgängliga i produktionsmiljön för alla kunder från och med en vecka från förhandsversionen.

Mer information finns i [Modernisering av gränssnitt](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).

</div>


Allokeringsprocenten representerar den tid en tilldelad resurs är planerad att arbeta med en aktivitet på en dag. Det är procentandelen av en arbetsdag (enligt användaren eller projektschemat) som en resurs tilldelas under aktivitetens varaktighet.

Du kan ändra allokeringsprocenten när du gör avancerade tilldelningar för en uppgift.

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
   <td>Adobe Workfront package</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td> <p>Standard</p>
   <p>Arbeta eller högre</p>
   </td> 
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Redigera åtkomst till uppgifter</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td>
   <td><p>Contribute eller högre behörigheter för aktiviteten</p>
   <p>Redigera behörigheter för att uppdatera allokeringsprocenten i rutan Redigera uppgift när <span class="preview"> redigerar uppgifter med den gamla funktionen. Du kan inte längre hantera allokeringsprocenten i aktivitetsrutan Redigera när du redigerar aktiviteter i den nya upplevelsen.</span></p> <p>Mer information finns i <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Redigera uppgifter</a></p>.</td>
  </tr>
 </tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--
Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation percentage in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation percentage in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.
-->

## Överväganden om att ändra procentallokeringar för uppgifter

* Användarna tilldelas som standard en lika lång procentandel av tiden till de uppgifter de tilldelas.
* Du kan ändra allokeringsprocenten för användare och jobbroller som tilldelats uppgifter manuellt endast när uppgiftens varaktighetstyp är Beräknad arbets- eller aktivitetsstyrd.

  Mer information finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Du kan inte ändra procentallokeringen för team som tilldelats aktiviteter.
* Du kan inte ändra procentallokeringen för användare och jobbroller som är tilldelade utgåvor.

## Ändra användar- eller rollprocentallokering för en uppgift

1. Gå till en aktivitet vars resurser du ändrar procentallokeringen för.
1. Klicka på området **Uppdrag** i uppgiftshuvudet och klicka sedan på **Avancerat**.

1. Kontrollera att aktivitetens **varaktighetstyp** är något av följande:

   * Beräknat arbete
   * Ansträngningsstyrd

   >[!TIP]
   >
   >* Workfront använder följande formel för beräkning av tilldelningens varaktighet för varje tilldelad: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* För den enkla varaktighetstypen kan du beräkna antalet tilldelade timmar för varje resurs, inte allokeringsprocenten.

1. Ändra fältet **Allokeringar** för varje tilldelad uppgift.

   Du kan bara ändra allokeringsprocenten för användar- och jobbrolltilldelningar.

   Du kan inte ändra allokeringsprocenten för ett team som tilldelats en aktivitet.

   ![Ändra allokeringsprocent](assets/advanced-assignments-allocation-percentage.png)

1. Klicka på **Spara**.
