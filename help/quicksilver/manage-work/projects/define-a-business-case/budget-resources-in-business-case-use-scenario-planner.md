---
navigation-topic: business-case-and-scorecards
title: Budgetresurser i affärsärendet med scenarioplaneraren
description: Som en del av resursplaneringen kan du använda Adobe Workfront Scenario Planner för att budgetera de jobbroller som krävs för att slutföra arbetet i ett projekt när du bygger affärsplanen.
author: Alina
feature: Work Management
exl-id: d5f3e348-dc7d-4265-a5ce-8eef152db410
source-git-commit: 5433008d93e99d69f8116e222bfce02411b77825
workflow-type: tm+mt
source-wordcount: '927'
ht-degree: 0%

---

# Budgetresurser i affärsärendet med scenarioplaneraren

<!--drafted for the Budgeted Hours story: 

<span class="preview">The highlighted information on this page refers to functionality not yet generally available. It is available only in the Preview environment.</span> -->

Som en del av resursplaneringen kan du använda Adobe Workfront Scenario Planner för att budgetera de jobbroller som krävs för att slutföra arbetet i ett projekt när du bygger affärsplanen.

Mer information om hur du skapar ett affärsärende finns i [Skapa ett affärsärende för ett projekt](../../../manage-work/projects/define-a-business-case/create-business-case.md).

>[!TIP]
>
>Jobbrollsinformationen för det projekt som är kopplat till projektet som du anger i scenarioplanen på systemnivå visas i området Resursbudgetering för projektets affärsplan när du publicerar initiativet. Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenario Planner finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md).

Du kan också budgetera resurser i affärsärendet med hjälp av Resursplanering. Mer information finns i följande:

* [Budgetresurser i affärsärendet](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md)

<!--* [Budget resources by project in the Resource Planner](../../../resource-mgmt/resource-planning/budget-by-project-resource-planner-d.md)-->

>[!NOTE]
>
>Vi rekommenderar att du bestämmer dig för att använda resursplaneraren eller scenarioplaneraren när du börjar arbeta med ett projekt. Om du växlar mellan de båda delarna ofta under projektets löptid kan det leda till inkonsekvenser i budgeten för dina resurser.

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 </col> 
 <col> 
 </col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Företag eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Granska eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för Adobe Workfront Scenario Planner för att få tillgång till de funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du skaffar Workfront Scenario Planner finns i <a href="../../../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda scenarioplaneraren</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Redigera åtkomst till följande: </p> 
    <ul> 
     <li> <p>Projekt</p> </li> 
     <li> <p>Finansiella data</p> </li> 
     <li> <p>Scenarioplan </p> </li> 
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

* Skapa en plan med hjälp av scenarioplanen.

   Mer information finns i [Skapa och redigera planer i scenarioplaneraren](../../../scenario-planner/create-and-edit-plans.md).

* Skapa ett initiativ för planen och länka det till ett projekt.

   Se till att du anger nödvändig information om befattningsroller för initiativet och uppdatera det länkade projektet med den här informationen.

   Mer information finns i följande artiklar:

   * [Skapa och redigera initiativ i Scenarioplaneraren](../../../scenario-planner/create-and-edit-initiatives.md)
   * [Importera projekt till planer i scenarioplaneraren](../../../scenario-planner/import-projects-to-plans.md)
   * [Uppdatera eller skapa projekt genom att publicera initiativ i Scenarioplanen](../../../scenario-planner/publish-scenarios-update-projects.md).

* Även om detta inte är några krav rekommenderar vi även följande:

   * Tilldela uppgifter i projektet till de jobbroller som är budgeterade i scenarioplaneraren.
   * Ange antalet planerade timmar för aktiviteterna i projektet.

      Detta hjälper dig att förstå hur mycket arbete en uppgift kan behöva utföra, vilket hjälper dig att bestämma hur mycket tid resurserna ska budgeteras för att slutföra uppgiften.

      Mer information om hur du associerar uppgifter med planerade timmar finns i [Redigera uppgifter](../../../manage-work/tasks/manage-tasks/edit-tasks.md).

## Budgetresurser i affärsärendet med hjälp av scenarioplaneraren för projekt som är kopplade till initiativ

>[!IMPORTANT]
Du kan budgetera dina resurser för en period på 15 år. Om du budgeterar resurser för ett projekt med en varaktighet på mer än 15 år kanske budgetinformationen inte är korrekt.
<!--
><MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">>
>(is this still accurate for the Scenario Planner?)>
></MadCap:conditionalText>>
>-->


1. Gå till projektet som du vill budgetera resurser för.

   >[!TIP]
   Detta är ett projekt som är kopplat till ett initiativ i Scenarioplanen, vars länkade initiativ har publicerats minst en gång.

1. Klicka **Affärsärende** i den vänstra panelen.
1. (Villkorligt) I **Resursbudgetering** gör du något av följande:

   * Om du precis har publicerat information från Scenarioplaneraren väljer du Scenarioplanering i **Välj vilka timmar som ska användas för att beräkna projektets budgeterade arbetskostnad** i området Resursbudgetering och klicka sedan **Välj**.

      ![](assets/business-case-sp-selected-with-choose-button-350x121.png)

   * Om resursplaneraren tidigare har valts för budgeteringsresurser för projektet klickar du på **Ändra** > **Scenarioplan** > **Välj**.

      ![](assets/business-case-rp-selected-change-option-to-switch-to-sp-highlighted-350x37.png)

      Workfront använder de obligatoriska jobbrolltimmarna från det länkade initiativet för att beräkna projektets budgeterade arbetskostnad och budgeterade timmar. Detta är det rekommenderade alternativet. Kostnaden visas i affärsärendet i projektets valuta.

      <!--drafted for Budgeted Hours:
   <span class="preview">När du kopierar ett projekt och väljer att kopiera de budgeterade timmarna till det nya projektet, kopieras inte de timmar som har budgeterats med scenarioplanen till det nya projektet. Endast timmar som har budgeterats i resursplaneraren kopieras. Mer information finns i [Kopiera ett projekt](../manage-projects/copy-project.md)</span>
-->

   >[!IMPORTANT]
   > 
   >När du använder Scenarioplanering för att budgetera resurser för projektet visas Budgeterad arbetskostnad i följande områden i Workfront:
   > 
   >* Resursbudgeteringsområde för affärsärendet
   >* Scenarioplanering på systemnivå som personkostnad för det projekt som är kopplat till projektet. Mer information finns i [Skapa och redigera initiativ i Scenarioplaneraren](../../../scenario-planner/create-and-edit-initiatives.md).


1. (Valfritt) Klicka på **Visa i scenarioplan** att öppna den plan som innehåller det projekt som är kopplat till projektet. Då öppnas Scenarioplanen på en ny flik i webbläsaren.
1. (Valfritt) Uppdatera information om initiativet. Mer information finns i [Skapa och redigera initiativ i Scenarioplaneraren](../../../scenario-planner/create-and-edit-initiatives.md).

   >[!NOTE]
   > 
   >Du måste publicera initiativet efter varje ändring för området Resursbudgetering i projektet som ska uppdateras.
