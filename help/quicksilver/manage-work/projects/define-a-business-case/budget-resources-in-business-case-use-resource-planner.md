---
navigation-topic: business-case-and-scorecards
title: Budgetresurser i affärsärendet med hjälp av resursplaneraren
description: Som en del av resursplaneringen kan du använda resursplaneraren på projektnivå för att budgetera de jobbroller som krävs för att slutföra arbetet i ett projekt när du skapar affärsplanen.
author: Alina
feature: Work Management
exl-id: 51ebb940-111c-442f-a8a6-287a04d2db68
source-git-commit: 8420f65e84edd42204d91aa503ff0b95153a1e67
workflow-type: tm+mt
source-wordcount: '1284'
ht-degree: 0%

---

# Budgetresurser i affärsärendet med hjälp av resursplaneraren

Som en del av resursplaneringen kan du använda resursplaneraren på projektnivå för att budgetera de jobbroller som krävs för att slutföra arbetet i ett projekt när du skapar affärsplanen.

Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Den information du anger i resursplaneraren på projektnivå visas också i resursplaneringsverktyget på systemnivå. Det motsatta är också sant. Mer information om resursplaneraren finns i [Översikt över resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

Du kan också budgetera resurser i ett affärsfall med hjälp av Adobe Workfront Scenario Planner. Mer information finns i [Budgetresurser i affärsärendet med scenarioplaneraren](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"><a href="https://www.workfront.com/plans" target="_blank">Adobe Workfront</a>*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"><a href="../../../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">Översikt över Adobe Workfront-licenser</a>*</td> 
   <td> <p>Granska eller högre</p> <p>Viktigt: Du måste ha en planlicens för att kunna ändra resursbudgeteringsinformationen. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till följande: </p> 
    <ul> 
     <li> <p>Projekt</p> </li> 
     <li> <p>Resurshantering</p> </li> 
     <li> <p>Finansiella data</p> </li> 
    </ul> <p>Mer information om åtkomsten till budgetresurserna finns även i <a href="../../../resource-mgmt/resource-planning/access-needed-to-budget-resources.md" class="MCXref xref">Tillgång till budgetresurser i Adobe Workfront</a>.</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Adobe Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter i projektet</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

## Förutsättningar

Innan du börjar måste du göra följande:

* Uppfyll alla krav för resursplanering i Adobe Workfront. Mer information finns i [Översikt över resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Associera resurspooler med projektet.

   <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:(you must have tasks assigned to job roles and users on the project - this is optional because the users and their roles come from the pools))</p>
  -->

   >[!NOTE]
   Du kan inte budgetera resurser som har tilldelats utleveranser i affärsärendet. Du kan budgetera dem i resursplaneraren på systemnivå. Mer information om resursplaneraren finns i [Översikt över resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

* Även om detta inte är en förutsättning rekommenderar vi även att du anger Planerade timmar för aktiviteterna i projektet. Detta hjälper dig att förstå hur mycket arbete en uppgift kan behöva utföra, vilket hjälper dig att avgöra hur mycket tid resurserna ska budgeteras för att slutföra uppgiften. Mer information om hur du associerar uppgifter med planerade timmar finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Använd resurspooler för ett projekt och budgetresurser i affärsärendet

>[!IMPORTANT]
Du kan budgetera dina resurser för en period på 15 år. Om du budgeterar resurser för ett projekt med en varaktighet på mer än 15 år kanske budgetinformationen inte är korrekt.

Så här använder du resurspooler och budgetprojektresurser i affärsärendet för ett projekt utan resurspool:

1. Gå till projektet som du vill budgetera resurser för.
1. Klicka **Affärsärende** i den vänstra panelen.
1. (Villkorligt) Om ditt företag inte har någon licens för Workfront Scenario Planner klickar du på **Redigera resursbudgetering** i **Resursbudgetering** fortsätter du med steg 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode,QuicksilverOrClassic.Quicksilver">(NOTE: ensure it stays right - this is 5 instead of 6 because step 2 won't print for nwe)</p>
   -->

1. (Valfritt och villkorligt) Gör något av följande om projektinformationen har publicerats från ett projekt i scenarioplaneraren:

   * Välj Resursplanering i dialogrutan **Välj vilka timmar som ska användas för att beräkna projektets budgeterade arbetskostnad** fält och klicka sedan på **Välj > Redigera resursbudgetering**.

      ![](assets/business-case-rp-selected-with-choose-button-350x120.png)

   * Om Scenarioplaneraren har valts för budgeteringsresurser för projektet klickar du på **Ändra** > **Redigera resursbudgetering**.

      ![](assets/business-case-sp-selected-change-option-to-switch-to-rp-highlighted-350x88.png)
   Detta använder projektets budgeterade timmar för att beräkna den budgeterade arbetskostnaden för projektet.

   Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenario Planner finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).

   >[!NOTE]
   Vi rekommenderar att du bestämmer dig för att använda resursplaneraren eller scenarioplaneraren när du börjar arbeta med ett projekt. Om du växlar mellan de båda delarna ofta under projektets löptid kan det leda till inkonsekvenser i budgeten för dina resurser.

1. I **Välj resurspool** fält, ange ett eller flera **Resurspooler**.

   Du får bara ange resurspooler som är ifyllda med aktiva användare.

   >[!TIP]
   Om projektet redan är associerat med resurspooler visas resursplaneraren som standard. Om du vill lägga till fler resurspooler i projektet redigerar du projektet. Mer information om hur du redigerar ett projekt finns i [Redigera projekt](../../../manage-work/projects/manage-projects/edit-projects.md).

1. Klicka **Använd**.

   Resursplaneraren visas för det valda projektet.

   Som standard listas de första 20 jobbrollerna som är associerade med det här projektet i resursbudgetavsnittet i alfabetisk ordning. 

   Mer information om resursplaneraren finns i [Översikt över resursplanering](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

   ![BC_resource_budgeting_area.png](assets/bc-resource-budgeting-area-350x276.png)

1. (Valfritt och villkorligt) Expandera jobbrollerna för att visa de användare som är associerade med dem.

   >[!NOTE]
   Aktiva användare visas endast under de jobbroller som är kopplade till dem om de uppfyller följande villkor:
   * De tillhör en av projektets resurspooler.
   * De har tilldelats budgeterade timmar.
   * De är kopplade till en av projektets jobbroller.


    

1. Klicka **Idag** för att återgå till dagens tidsram.
1. (Valfritt) Klicka på **Vecka**, **Månad** eller **Kvartal** om du vill visa information för projektet i olika tidsramar.
1. (Valfritt) Klicka på **Timmar** nedrullningsbar meny och välj **Timmar**,**FTE**, eller **Kostnad** om du vill ändra hur information visas i resursplaneraren. Timmar visas som standard.

1. (Valfritt) Klicka på **Exportera** om du vill exportera resursplaneraren till en Excel-fil.

   >[!NOTE]
   Du kan exportera data i upp till 12 tidsperioder i taget.

1. (Valfritt) Klicka på **Helskärm** icon ![full_screen_RP_in_BC.png](assets/full-screen-rp-in-bc.png) om du vill visa resursplaneraren i helskärmsläge.

1. Uppdatera **BDG** (Budgeterade timmar) med timma-, FTE- eller kostnadsvärden för användare, roller eller projektet genom att göra något av följande:

   * Uppskatta manuellt timtals-, FTE- eller kostnadsvärden för roller, användare eller projektet.

      eller

   * Klicka på **Alternativ** -ikonen för projektet eller jobbrollerna och välj ett alternativ för att automatiskt budgetera timmarna för roller, användare eller projektet.
   Mer information om budgetering i projektvyn i resursplaneraren finns i [Budgetresurser i resursplaneraren med projekt- och rollvyerna](../../../resource-mgmt/resource-planning/budget-resources-project-role-views-resource-planner.md).

   >[!NOTE]
   Du kan budgetera timmar, heltidsanställda och kostnader för dina resurser för alla tidsramar som visas i området Resursbudgetering, oberoende av tidslinjen i projektet. Om du till exempel vill ange att dina resurser kanske inte är tillgängliga under tidslinjen för projektet (där de är kopplade till Planerade timmar), men de kan vara tillgängliga under en annan tid, kan du göra det genom att budgetera dem för tidsramar där Planerade timmar är noll, om det är när de blir tillgängliga för arbete.

1. (Valfritt) Klicka på knappen **Alternativ** ikon, sedan **Justera budgetdatum**.

   Mer information om hur du justerar budgeterade datum finns i [Justera budgeteringsdatum i resursplaneraren](../../../resource-mgmt/resource-planning/adjust-budgeting-dates.md).

1. Klicka **Spara**.

   Om du har en kostnad per timme som är associerad med dina jobbroller, beräknas resurserna i området Resursbudgetering **Budgeterad arbetskostnad** av projektet. Budgeterad arbetskostnad visas i området Resursbudgetering i affärsärendet och i Översikt över affärsärenden.

   >[!TIP]
   Kostnaden visas i affärsärendet i projektets valuta.

   Den budgeteringsinformation som anges i affärsärendet visas också i resursplaneraren.

   När du kopierar ett projekt kan du även kopiera budgeterade timmar till det nya projektet. Endast timmar som har budgeterats i resursplaneraren kopieras. Mer information finns i [Kopiera ett projekt](../manage-projects/copy-project.md).
