---
content-type: reference
product-area: projects
navigation-topic: financials
title: Beräkna budgeterad kostnad
description: Beräkna förlopp för budgeterat kostnadsspårningsprojekt med en användningsrapport""
author: Lisa
feature: Work Management
exl-id: e96fe38f-58c2-4938-9d2d-81d1109123fa
source-git-commit: 6afa65f921864403c10541d283ef717dce81aed7
workflow-type: tm+mt
source-wordcount: '394'
ht-degree: 0%

---

# Beräkna budgeterad kostnad

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: This article is linked from "Tracking Project Progress with a Utilization Report"</p>
<p>Keep the structure of this article similar to Calculating Budgeted Labor Cost)</p>
</div>
-->

Den budgeterade kostnaden för ett projekt är den totala kostnaden som är associerad med projektet enligt den uppskattning du gjorde när du planerar projektet.

## Översikt över budgeterad kostnad i ett projekt

Du kan inte ändra den budgeterade kostnaden för ett projekt manuellt. Adobe Workfront beräknar den budgeterade kostnaden med följande formel:

`Budgeted Cost = Resource Planner Budgeted Labor Cost + Budgeted Expenses Cost + Fixed Cost of the project`

* Den budgeterade arbetskostnaden för **resursplanering** i beräkningen ovan är kostnaden som är associerad med jobbrollerna i projektet.

  Du kan spåra den budgeterade arbetskostnaden för ett projekt i området Resursbudgetering i affärsärendet eller Resursplaneringen.

  >[!TIP]
  >
  >  Budgeterad arbetskostnad för ett projekt i affärsärendet visas som Resursplanering Budgeterad arbetskostnad i rapporter och listor.

  Mer information om budgeterade arbetskostnader finns i artikeln [Förstå budgeterad arbetskostnad och budgeterade timmar för projekt](../../../manage-work/projects/project-finances/budgeted-labor-cost.md).

* Den **budgeterade utgiftskostnaden** i beräkningen ovan är den planerade kostnad som är associerad med utgifterna i projektet, så som de beräknas i området Utgifter i affärsärendet eller på fliken Utgifter i projektet.\
  Mer information om utgifter för ett projekt finns i artikeln [Hantera projektutgifter](../../../manage-work/projects/project-finances/manage-project-expenses.md).

* **Fast kostnad** i beräkningen ovan är det fasta belopp som är associerat med kostnaden för projektet, enligt definitionen i området Ekonomi i projektavsnittet.\
  Mer information om underfliken Ekonomi i ett projekt finns i artikeln [Hantera information i projektfinansieringsdelen](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

>[!NOTE]
>
>Workfront beräknar all kostnadsinformation i projektets valuta. Om du anger Budgeterade timmar för dina resurser i Resursplanering inaktiveras alternativet att ändra projektvaluta.
>
>Mer information om hur du ändrar valuta för ett projekt finns i artikeln [Ändra projektvalutan](../../../manage-work/projects/project-finances/change-project-currency.md).

## Hitta den budgeterade kostnaden för ett projekt

Budgeterad kostnad som återspeglas i resursbudgeteringsområdet i affärsärendet eller resursplaneraren visas i följande områden i Workfront under följande namn:

<table style="table-layout:auto"> 
   <col> 
   <col> 
   <tbody> 
    <tr> 
     <td><strong>Visningsnamn för budgeterad kostnad</strong></td> 
     <td><strong>Område i Workfront</strong></td> 
    </tr> 
    <tr> 
     <td>Budgeterad kostnad</td> 
     <td> <p>Översikt över affärsärenden</p> <p> <img src="assets/business-case-summary-qs-350x453.png" style="width: 350;height: 453;"> </p> </td> 
    </tr> 
    <tr> 
     <td>Kostnad</td> 
     <td> <p>Portfolio Optimizer</p> <p>Tips! Summan av alla projektbudgeterade kostnadsvärden är portföljens budgeterade kostnad.</p> </td> 
    </tr> 
    <tr> 
     <td>Projektbudgeterad kostnad</td> 
     <td> <!--
       <p data-mc-conditions="QuicksilverOrClassic.Draft mode">Resource Estimates report (NOTE: this was removed with flash)</p>
      --> <p>Projektrapport</p> <p>Projektrapport (ekonomiska data)</p> <p>Uppgiftsrapport</p> <p>Problemrapport</p> <p>Budgeterad timrapport</p> <p>Mer information om hur du skapar en rapport finns i artikeln <a href="../../../reports-and-dashboards/reports/creating-and-managing-reports/create-custom-report.md" class="MCXref xref">Skapa en anpassad rapport</a>.</p> </td> 
    </tr> 
   </tbody> 
  </table>
