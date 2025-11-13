---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Hantera användar- och rolltilldelningstimmar för aktiviteter
description: När du tilldelar användare eller roller till en uppgift, tilldelas de ett visst antal timmar för att slutföra uppgiften. Du kan manuellt ändra hur många timmar varje användare eller jobbroll tilldelas när de tilldelas till en uppgift när uppgiftens varaktighetstyp är Enkel.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: 1f9a0e6064f83c6f0947e3c7ef596e96c934a687
workflow-type: tm+mt
source-wordcount: '573'
ht-degree: 0%

---

# Hantera användar- och rollallokeringstimmar för uppgifter

<!--Audited: 10/2025-->

<!--remove new/old experience references when they remove the New/ Old experience toggle from the Edit Tasks box-->


<!--<div class="preview"> 

The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment for all customers. The same features will also be available in the Production environment for all customers starting with  a week from the Preview release.      

For more information, see [Interface modernization](/help/quicksilver/product-announcements/product-releases/interface-modernization/interface-modernization.md).  

</div> -->

Tilldelningstimmar representerar den totala tiden som en tilldelad resurs är planerad att arbeta med en aktivitet. Timmarna representerar den tid som en användare tilldelas en viss dag eller en viss veckodag, vecka eller månad under hela uppgiftens varaktighet.

Du kan ändra allokeringstimmar när du gör avancerade tilldelningar för en uppgift.

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
   <p>Redigera behörigheter för att uppdatera allokeringstimmar i rutan Redigera uppgift när du redigerar uppgifter med den gamla funktionen. Du kan inte längre hantera tilldelningstimmar i åtgärdsrutan Redigera när du redigerar uppgifter i den nya upplevelsen.</p> <p>Mer information finns i <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Redigera uppgifter</a>.</p></td>
  </tr>
 </tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Take this piece out of the table above when we remove the new experience/ after production release in the task box: 

<p>Edit permissions to update allocation hours in the Edit Task box when editing tasks using the old experience. <span class="preview">You can no longer manage allocation hours in the Edit task box when editing tasks in the new experience.</span></p> <p>For information, see <a href="/help/quicksilver/manage-work/tasks/manage-tasks/edit-tasks.md">Edit tasks</a></p>.-->


## Överväganden för att ändra allokeringstimmar för en aktivitet

>[!IMPORTANT]
>
>När du har ändrat allokeringarna för varje tilldelning för uppgifter manuellt kan aktiviteternas planerade timmar uppdateras i enlighet med detta. Mer information finns i avsnittet [Uppdatera planerade timmar för aktiviteter när användartilldelningar hanteras](../../../manage-work/tasks/task-information/planned-hours.md#update) i artikeln [Översikt över planerade timmar](../../../manage-work/tasks/task-information/planned-hours.md).

* Det totala antalet timmar som tilldelas enskilda resurser som tilldelats till aktiviteten representerar aktivitetens planerade timmar.
* Om det finns en användar- eller rolltilldelning för en aktivitet, matchar antalet timmar som tilldelats användaren eller rollen aktivitetens planerade timmar.
* När det gäller flera tilldelningar tilldelas varje användare eller jobbroll som standard ett lika stort antal timmar att arbeta med uppgiften, om uppgiftens varaktighetstyp är Enkel. Mer information finns i följande artiklar:

   * [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md)
   * [Översikt över varaktighetstyp: Enkel](../../../manage-work/tasks/taskdurtn/simple-duration-type.md)

* När aktiviteten har en enkel varaktighetstyp kan du manuellt ändra antalet allokerade timmar för varje användare eller jobbroll för att ange att en del av uppgiftstilldelningarna kan ha mer tid att arbeta med en uppgift än andra.
* Du kan inte ändra antalet timmar som tilldelats team som tilldelats aktiviteter.
* Du kan inte ändra användar- eller jobbrollallokeringen manuellt för utgåvor.
* Du kan också hantera dagliga, veckovisa eller månadsvisa tilldelningar av användare till uppgifter eller ärenden med hjälp av Utjämning av arbetsbelastning. Mer information finns i [Hantera användartilldelningar i Utjämning av arbetsbelastning](../../../resource-mgmt/workload-balancer/manage-user-allocations-workload-balancer.md).

## Ändra användar- eller rollallokeringstimmar för en uppgift

1. Gå till en uppgift vars tilldelningar du vill ändra allokeringstimmar för.
1. Klicka på området **Uppdrag** i uppgiftshuvudet och klicka sedan på **Avancerat**.
1. Kontrollera att aktivitetens **varaktighetstyp** är **enkel**.
1. Ändra fältet **Allokeringar** för varje tilldelad uppgift. Detta är övergripande allokeringar för varje tilldelning för den här aktiviteten, under hela aktivitetens varaktighet. Detta kan även uppdatera aktivitetens övergripande **Planerade timmar**.

   ![Ändra allokeringar](assets/advanced-assignments-duration-type-allocations.png)

1. Klicka på **Spara**.
