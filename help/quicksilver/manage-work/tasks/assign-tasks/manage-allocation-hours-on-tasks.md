---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Hantera användar- och rolltilldelningstimmar för aktiviteter
description: När du tilldelar användare eller roller till en uppgift, tilldelas de ett visst antal timmar för att slutföra uppgiften. Du kan manuellt ändra hur många timmar varje användare eller jobbroll tilldelas när de tilldelas till en uppgift när uppgiftens varaktighetstyp är Enkel.
author: Lisa
feature: Work Management
exl-id: 2c0cd6ef-8719-4680-aa63-5e229de0f819
source-git-commit: d0be569333b0454e26f4d0de1078b0425cf81707
workflow-type: tm+mt
source-wordcount: '544'
ht-degree: 0%

---

# Hantera användar- och rollallokeringstimmar för uppgifter

Tilldelningstimmar representerar den totala tiden som en tilldelad resurs är planerad att arbeta med en aktivitet. Timmarna representerar den tid som en användare tilldelas en viss dag eller en viss veckodag, vecka eller månad under hela uppgiftens varaktighet.

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
   <p>Redigera behörigheter för att uppdatera allokeringstimmar i rutan Redigera uppgift</p></td>
  </tr>
 </tbody>
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

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
1. Klicka på **Mer**-menyn ![](assets/qs-more-icon-on-an-object.png) intill aktivitetens namn, klicka sedan på **Redigera** och sedan på **Uppdrag**.

   eller

   Klicka på området **Uppdrag** i uppgiftshuvudet och klicka sedan på **Avancerat**.

1. Kontrollera att aktivitetens **varaktighetstyp** är **enkel**.
1. Ändra **allokeringarna** för varje tilldelad uppgift. Detta är övergripande allokeringar för varje tilldelning för den här aktiviteten, under hela aktivitetens varaktighet. Detta kan även uppdatera aktivitetens totala planerade timmar.

   ![Ändra allokeringar](assets/advanced-assignments-duration-type-allocations.png)

1. Klicka på **Spara**.
