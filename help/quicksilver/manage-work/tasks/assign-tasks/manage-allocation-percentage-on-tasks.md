---
product-area: projects;user-management
navigation-topic: assign-tasks
title: Hantera användar- eller rollallokeringsprocent för uppgifter
description: Allokeringsprocenten representerar den tid en tilldelad resurs är planerad att arbeta med en aktivitet på en dag. Det är procentandelen av en arbetsdag (enligt användaren eller projektschemat) som en resurs tilldelas under aktivitetens varaktighet.
author: Alina
feature: Work Management
exl-id: 82238dff-b95e-42e4-8e72-6247934b504d
source-git-commit: ad5d6bfda24119076df8336ed291c0ba63e2c88a
workflow-type: tm+mt
source-wordcount: '499'
ht-degree: 0%

---

# Hantera användar- eller rollallokeringsprocent för uppgifter

{{highlighted-preview}}

Allokeringsprocenten representerar den tid en tilldelad resurs är planerad att arbeta med en aktivitet på en dag. Det är procentandelen av en arbetsdag (enligt användaren eller projektschemat) som en resurs tilldelas under aktivitetens varaktighet.

>[!NOTE]
>
>När du tilldelar användare arbetstid påverkar tillgängligheten enligt sina scheman de planerade och planerade datumen för uppgifter och problem. Mer information om scheman finns i [Skapa ett schema](../../../administration-and-setup/set-up-workfront/configure-timesheets-schedules/create-schedules.md).

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Arbeta eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till uppgifter</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Contribute eller högre behörigheter för aktiviteten</p> <p>Redigera behörigheter för att uppdatera allokeringsprocent i rutan Redigera uppgift</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Överväganden om att ändra procentallokeringar för uppgifter

* Användarna tilldelas som standard en lika lång procentandel av tiden till de uppgifter de tilldelas.
* Du kan ändra allokeringsprocenten för användare och jobbroller som tilldelats uppgifter manuellt endast när uppgiftens varaktighetstyp är Beräknad arbets- eller aktivitetsstyrd.

  Mer information finns i [Översikt över aktivitetsvaraktighet och varaktighetstyp](../../../manage-work/tasks/taskdurtn/task-duration-and-duration-type.md).

* Du kan inte ändra procentallokeringen för team som tilldelats aktiviteter.
* Du kan inte ändra procentallokeringen för användare och jobbroller som är tilldelade utgåvor.

## Ändra användar- eller rollprocentallokering för en uppgift

1. Gå till en aktivitet vars resurser du ändrar procentallokeringen för.
1. Klicka på **Mer** meny ![](assets/qs-more-icon-on-an-object.png) bredvid namnet på uppgiften och klicka sedan på **Redigera**.

   eller

   Klicka på **Uppdrag** i uppgiftshuvudet och klicka sedan **Avancerat**.

1. Se till att **Varaktighetstyp** en av följande uppgifter:

   * Beräknat arbete
   * Ansträngningsstyrd

   >[!TIP]
   >
   >* I Workfront används följande formel för beräkning av tilldelningens varaktighet: `Allocation Percentage = (Work Required / Number of days in the Duration) / Number of hours per work day / Number of assignees`.
   >* För den enkla varaktighetstypen kan du beräkna antalet tilldelade timmar för varje resurs, inte allokeringsprocenten.

1. Klicka **Uppdrag** och sedan ändra **Allokeringar** för varje tilldelad uppgift.

   Du kan bara ändra allokeringsprocenten för användar- och jobbrolltilldelningar.

   Du kan inte ändra allokeringsprocenten för ett team som tilldelats en aktivitet.

   Exempelbild i produktionsmiljön:
   ![](assets/qs-advanced-assignments-box-with-duration-type-and-duration-350x251.png)

   <span class="preview">Exempelbild i förhandsvisningsmiljön:</span>
   ![Ändra allokeringsprocent](assets/advanced-assignments-allocation-percentage.png)

1. Klicka **Spara**.
