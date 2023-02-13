---
product-area: projects
navigation-topic: plan-a-project
title: Visa projektplanerade timmar på panelen Rollallokering
description: Du kan visa rollallokering för alla jobbroller som har tilldelats arbetsobjekt i ett projekt på panelen Rollallokering i projektet.
author: Alina
feature: Work Management
exl-id: 76f70cb6-f707-4a73-bc81-e755e2d0a33d
source-git-commit: bbd64e9deed1b89d720272508b3562c354578704
workflow-type: tm+mt
source-wordcount: '468'
ht-degree: 0%

---

# Visa projektplanerade timmar på panelen Rollallokering

Du kan visa rollallokering för alla jobbroller som har tilldelats arbetsobjekt i ett projekt på panelen Rollallokering i projektet.

>[!NOTE]
>
>Den här artikeln hänvisar till att visa de jobbroller som är associerade med uppgifter och utgåvor i ett projekt och deras tilldelade planerade timmar på panelen Rolltilldelning i ett projekt. Mer information om hur du avstämde Planerade timmar med initieringstimmar med hjälp av rollallokeringspanelen när du använder Adobe Workfront scenarioplan finns i följande:
>
>* [Visa rolltilldelning för projekt och initiativ i uppgiftslistan](../../../scenario-planner/show-role-allocation-task-list-nwe.md)
>* [Visa rolltilldelning för projekt och initiativ i Utjämning av arbetsbelastning](../../../scenario-planner/show-role-allocation-workload-balancer.md)
>
>  Du måste ha en licens för Scenarioplanering för att kunna se initieringstimmar på panelen Rollallokering. Mer information om scenarioplanen finns i [Kom igång med scenarioplanen](../../../scenario-planner/get-started-with-scenario-planning.md) .

## Åtkomstkrav

<!--drafted for P&P:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront plan*</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront license*</td> 
   <td> <p>Current license: Light or higher</p> 
   Or
   <p>Legacy license: Review or higher</p> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>View or higher access to Projects</p> <p>If you still don't have access, ask your Workfront administrator if they set additional restrictions in your access level. For information on how a Workfront administrator can modify your access level, see <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Create or modify custom access levels</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>View or higher permissions on the project</p> <p>For information on requesting additional access, see <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Request access to objects </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

-->

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller ge högre åtkomst till projekt</p> <p>Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa eller högre behörigheter i projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Du måste ha följande:

* Uppgifter eller ärenden som tilldelats jobbroller eller användare som är kopplade till en jobbroll.

   >[!TIP]
   Om aktiviteterna eller problemen inte har tilldelats, tilldelats till team eller har tilldelats användare utan jobbroll är projektets planerade timmar noll på panelen Rolltilldelning.

* Aktiviteter och problem med en varaktighet som är högre än noll.

## Visa projektplanerade timmar på panelen Rollallokering

1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront och klicka sedan på **Projekt**.
1. Klicka på namnet på ett projekt för att komma åt det. Sidan Projekt öppnas.
1. Klicka på något av följande i den vänstra panelen:

   * **Uppgifter**
   * **Utjämning av arbetsbelastning**

1. Klicka på **Visa rollallokering** icon ![](assets/show-role-allocation-icon.png).

   Panelen Rolltilldelning visas.

   ![](assets/role-allocation-panel-planned-hours-only-350x316.png)

1. Granska följande information i **Rollallokering** panel: |Fält | Beskrivning| |—|—| | **Jobbroll** |Jobbroller som tilldelats aktiviteter och ärenden i projektet. Dessa kan vara jobbroller som tilldelas direkt till uppgifter och ärenden eller jobbroller som är kopplade till användare som har tilldelats aktiviteter och ärenden i projektet.  | | **Planerade timmar** |Totalt antal planerade timmar från uppgifter och ärenden som tilldelats jobbroller eller användare som är associerade med en jobbroll i projektet. |



