---
content-type: reference
product-area: resource-management
navigation-topic: resource-planning
title: Tillgång till budgetresurser i Workfront
description: Du kan visa och hantera information om resursplanering för de projekt som du har åtkomst till och visa när du har vissa åtkomstnivåinställningar och behörigheter för dina arbetsobjekt, användare, jobbroller och team.
author: Lisa
feature: Resource Management
exl-id: d2bfc411-188a-4f8b-8180-0e984f01b5ab
source-git-commit: a5317e3126939d4c648977635af2dbc6add02780
workflow-type: tm+mt
source-wordcount: '346'
ht-degree: 0%

---

# Tillgång till budgetresurser i Workfront

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p><b>(LINKED TO PRODUCT</b>: This is also linked to the product, in two different tooltips in the RP:</p>
<p>- the tooltip for the View-only mode of the Budgeted Hours boxes. You gave this link to Vazgen and the team for the tooltip and documented this in this sheet:https://docs.google.com/spreadsheets/d/1zKjNVw_TyfQ474jbY7JorSWTkptMNb5RFCck2IficYs/edit#gid=0</p>
<p>- Also in the tooltip from this issue: https://hub.workfront.com/issue/view?ID=5ca708d00024a39e58b5dbeaceb00939)</p>
<p>This might need to be moved to Resource Management overview and title needs to be changed to "Acces needed to manage resources" when the res manager prerequisite will drop for resource scheduling and the field goes away.</p>
<p>This should be linked from Planning in the Resource Planner - in the Budgeting Resources in the RP area)</p>
</div>
-->

När ditt företag har köpt en Adobe Workfront-licens som innehåller resursplanering kan du visa resursbudgeteringsinformation för de projekt som du har behörighet att visa. Du kan visa budgeteringsinformation i Resursplanering.

Mer information om krav för att använda budgeteringsverktygen i Workfront finns i [Kom igång med resursplanering](../../resource-mgmt/resource-planning/get-started-resource-planning.md).

För att kunna budgetera resurser, hantera resurspooler och se Kostnadsinformation i resursplaneringsverktygen måste ditt företag och du ha följande åtkomst: 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td><p>Nytt: Alla</p>
       <p>eller</p>
       <p>Aktuell: Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td><p>Nytt: Standard</p>
       <p>eller</p>
       <p>Aktuell: Planera</p></td>
  </tr>  
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> 
    <ul> 
     <li> <p>Redigera åtkomsten till resurshanteringen på din åtkomstnivå som innehåller:</p> 
      <ul> 
       <li> <p>Åtkomst att redigera projektprioriteringar och budgettimmar. </p> </li> 
       <li> <p>Åtkomst för att hantera resurspooler, om du behöver hantera resurspooler.</p> </li> 
      </ul> <p>Mer information om åtkomstnivån för resurshantering finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-resource-management.md" class="MCXref xref">Bevilja åtkomst till resurshantering</a>.</p> </li> 
     <li> <p>Redigera åtkomst till projekt och användare. </p> </li> 
     <li> <p> Redigera åtkomsten till finansiella data på din åtkomstnivå om du behöver visa eller hantera information via Kostnad.</p> <p>Mer information om åtkomstnivån för finansiella data finns i artikeln <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Bevilja åtkomst till ekonomiska data</a>.</p> </li> 
    </ul> 
   </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för projektet med behörigheterna Hantera ekonomi.</p> <p>Mer information om projektbehörigheter finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-a-project.md" class="MCXref xref">Dela ett projekt i Adobe Workfront</a>.</p> <p>Mer information om ekonomiska behörigheter för ett projekt finns i artikeln <a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md"><a href="../../workfront-basics/grant-and-request-access-to-objects/share-financial-permissions-object.md" class="MCXref xref">Dela ekonomiska behörigheter för ett objekt</a></a>.</p>

<p><b>ANMÄRKNING</b>

Om du har mindre än Hantera behörigheter för minst ett projekt i rollen kan du inte budgetera timmar, FTE eller Kostnad för rollen när du budgeterar resurser i rollvyn. Du kan bara budgetera de projekt som du har behörigheten Hantera för.</p> </td>
</tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).
