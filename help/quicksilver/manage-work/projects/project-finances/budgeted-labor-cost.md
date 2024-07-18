---
content-type: reference
product-area: projects
navigation-topic: financials
title: Förstå budgeterad arbetskostnad och budgeterade timmar för projekt
description: Förstå budgeterad arbetskostnad och budgeterade timmar för projekt
author: Alina
feature: Work Management
exl-id: 01020bbb-7cf9-4461-b0b6-dcbbc537c616
source-git-commit: f2f825280204b56d2dc85efc7a315a4377e551c7
workflow-type: tm+mt
source-wordcount: '1128'
ht-degree: 0%

---

# Förstå budgeterad arbetskostnad och budgeterade timmar för projekt

<!--
<(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)</p>
-->

Du kan budgetera dina resurser för arbete med hjälp av Adobe Workfront Resursplanering.

När du budgeterar dina resurser för arbete med projekt beräknar Workfront den budgeterade arbetskostnaden för roller, projekt och användare baserat på kostnad per timme.

Resursplaneringens budgeterade arbetskostnad för ett projekt är en beräkning mellan kostnaden som är associerad med de jobbroller som är tilldelade för att slutföra arbetet i projektet och det timbelopp som beräknas (Resursplaneringens budgeterade timmar) som kan ta varje roll för att slutföra arbetet.

>[!IMPORTANT]
>
>Resursplaneringens budgeterade arbetskostnad för användare påverkar inte projektets arbetskostnad. Endast arbetskostnaden för jobbroller påverkar kostnaden för projektet.

## Översikt över budgeterad arbetskostnad för jobbroller och projektet

Workfront använder den budgeterade arbetskostnaden för jobbrollerna i projektet för att beräkna projektets budgeterade arbetskostnad.

>[!TIP]
>
>Budgeterad arbetskostnad för ett projekt i affärsärendet visas som Resursplanering Budgeterad arbetskostnad i rapporter och listor.

**Budgeterad arbetskostnad** (eller Budgeterad arbetskostnad för resursplanering) för ett projekt beräknas med följande formel:

`Resource Planner Budgeted Labor Cost = SUM ( Resource Planner Budgeted Hours for each job role on the project * Cost per Hour rate of each job role on the project)`

Fälten i beräkningen ovan avser följande:

* Budgeterade timmar för jobbroller i projektbudgetområdet eller resursplaneraren.

  Mer information om budgeteringsresurser i resursplaneraren finns i avsnittet Budgeteringsresurser i resursplaneraren i artikeln [Resursplaneringsöversikt](../../../resource-mgmt/resource-planning/get-started-resource-planner.md).

  Mer information om budgeteringsresurser i området Resursbudgetering i affärsärendet finns i [Budgetresurser i affärsärendet](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case.md).

* Kostnaden **Kostnad per timme för en jobbroll** i ovanstående beräkning refererar till kostnaden som är associerad med varje jobbroll i projektet.\
  Mer information om hur du skapar och hanterar jobbroller och associerar dem med kostnadstariffer finns i artikeln [Skapa och hantera jobbroller](../../../administration-and-setup/set-up-workfront/organizational-setup/create-manage-job-roles.md).

>[!NOTE]
>
>Workfront beräknar all kostnadsinformation i projektets valuta. Om du anger Budgeterade timmar för dina resurser i Resursplanering inaktiveras alternativet att ändra projektvaluta.\
>Mer information om hur du ändrar valuta för ett projekt finns i artikeln [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md).

## Översikt över budgeterad arbetskostnad för användare

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Update the following section in the Create a Business Case article, as well, when you update it here.)</p>
-->

>[!IMPORTANT]
>
>Den användarbudgeterade arbetskostnaden påverkar inte projektets budgeterade arbetskostnad. Endast arbetskostnaden för jobbrollerna i ett projekt påverkar projektets arbetskostnad i Resursplanering.
> 
>Summan av alla arbetskostnader för alla användare kan vara lika med Resursplaneringens budgeterade arbetskostnad för de jobbroller som är kopplade till användarna.
>
>Om du uppskattar budgeterade timmar för användare i resursplaneraren, är kostnaderna som är kopplade till dem för de jobbroller som är kopplade till användarna. De är inte kostnader som hänger samman med användarna eller deras priser.

Om användare är associerade med jobbrollerna i projektet och deras timmar är budgeterade i resursplaneraren, visas deras budgeterade arbetskostnad med följande namn, beroende på var du visar dem i Workfront:

* [!UICONTROL **Budgeterad arbetskostnad**]: Resursbudgeteringsområdet för affärsärendet under deras respektive roller.

  ![](assets/budgeted-labor-cost-for-users-in-business-case-highlighted-350x73.png)

* [!UICONTROL **BDG**]: Resursplaneraren visar information i projekt- och rollvyn utifrån kostnad.

  ![](assets/budgeted-labor-cost-for-users-in-rp-project-view-cost--highlighted-350x115.png)

Användarna visas i området Resursbudgetering i affärsärendet under sina respektive roller eller i Resursplaneraren om de uppfyller följande krav:

* De är kopplade till en av jobbrollerna i projektet.
* De har angivna budgettimmar i resursplaneraren.
* De har en kostnad per timme som är associerad med deras profil.

  Mer information om hur du lägger till kostnad per timme för användare finns i artikeln [Redigera en användares profil](../../../administration-and-setup/add-users/create-and-manage-users/edit-a-users-profile.md).

* Användaren ingår i en av de resurspooler som är associerade med projektet.

En användares budgeterade arbetskostnad beräknas med följande formel:

`User Budgeted Labor Cost = Budgeted hours for the user on the project * Cost per Hour rate of the user`

## Hitta den budgeterade arbetskostnaden för ett projekt

Budgeterad arbetskostnad som återspeglas i resursbudgeteringsområdet för affärsärendet eller resursplaneraren visas i följande områden i Workfront under följande namn:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Visningsnamn för budgeterad arbetskostnad</strong></td> 
     <td><strong>Område i Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Budgeterad arbetskostnad</td> 
     <td>Resursbudgeteringsområde för affärsärendet</td> 
    </tr> 
    <tr> 
     <td>Budgeterad kostnad</td> 
     <td><p>Kostnadsvy för användningsrapport</p><p>Mer information finns i <a href="../../../resource-mgmt/resource-utilization/view-utilization-information.md">Visa användningsinformation</a> .</p></td> 
    </tr> 
    <tr> 
     <td>BDG </td> 
     <td>Resursplaneringsprojekt eller rollvyer, per kostnad</td> 
    </tr> 
    <tr> 
     <td>Resursplaneringsprojekt budgeterad arbetskostnad</td> 
     <td> <p>Projektrapport</p> <p>Projektrapport (ekonomiska data)</p> <p>Uppgiftsrapport</p> <p>Problemrapport</p> <p>Budgeterad timrapport</p> <p>Mer information om hur du skapar en rapport finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>

>[!NOTE]
>
>Om du använder Adobe Workfront Scenario Planner för att budgetera projektresurser är Budgeterad arbetskostnad i området Resursbudgetering i affärsärendet densamma som personkostnaderna för det projekt som är kopplat till projektet. Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenarioplan finns i [Översikt över scenarioplanen](../../../scenario-planner/scenario-planner-overview.md). Mer information om budgeteringsresurser med hjälp av scenarioplaneraren finns i [Budgetresurser i affärsärendet med hjälp av scenarioplaneraren](../../../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

## Hitta budgeterade timmar för ett projekt

<!--
(NOTE: Keep the structure of this article similar to Calculating Budgeted Cost)
-->

Budgeterade timmar påverkar värdet för projektets budgeterade arbetskostnad (eller budgeterade resursplaneringskostnad).

Budgeterad arbetskostnad för ett projekt är den kostnad som är associerad med de jobbroller som är tilldelade för att slutföra arbetet i projektet och det timbelopp som beräknas (Budgeterade timmar) som kan ta varje roll för att slutföra arbetet.

Du kan visa budgeterade timmar i Workfront i fälten som listas i tabellen nedan.

>[!NOTE]
>
>Alla andra omnämnanden av&quot;Budgeterade timmar&quot; i Workfront avser timmar som budgeterats med inaktuella funktioner som tagits bort från Workfront. Dessa är skrivskyddade fält och uppdateras inte med aktuell information när du använder aktuella resursbudgeteringsverktyg.

De budgeterade timmarna i området Resursbudgetering i affärsärendet eller resursplaneringen visas i följande områden i Workfront och under följande namn:

* **Timmar**: Resursbudgeteringsområdet för affärsärendet
* **BDG**:Resursplanering visas i timmar
* **Budgeterade timmar**: Översikt över utnyttjanderapporter
Mer information finns i [Visa information om resursutnyttjande](../../../resource-mgmt/resource-utilization/view-utilization-information.md).
* **Bud. Timmar**: Budgeterad timrapport

  Objektet Budgeterad timme i rapporten Budgeterad timme refererar till information som relaterar till ett ersatt resurshanteringsverktyg. Bara &quot;Bud&quot;. Timmar&quot; i den här rapporten refererar till de timmar som budgeterats i resursplaneraren eller i området Resursbudgetering för projektets affärsärende.

  Mer information om hur du skapar en rapport finns i artikeln **Skapa en anpassad rapport**.
* **Budgeterade timmar för resursplanering**: i följande rapporter:

   * Projektrapport
   * Projektrapport (ekonomiska data)
   * Uppgiftsrapport
   * Problemrapport
   * Budgeterad timrapport
