---
content-type: api
navigation-topic: api-navigation-topic
title: Nyheter i API-version 20
description: Adobe Workfront släppte API-version 20 den 6 april 2022. API version 20 innehåller följande ändringar från version 19.
author: Becky
feature: Workfront API
role: Developer
source-git-commit: 6d2aa582a72aad098e397a5e59abdee84165a426
workflow-type: tm+mt
source-wordcount: '1792'
ht-degree: 0%

---

# Nyheter i API-version 20

Adobe Workfront släppte API-version 20 den 4 maj 2025. API version 20 innehåller följande ändringar från version 19.

## Tillagda resurser

Inga resurser har lagts till för API-version 20.

<!--

### AssignmentBillingRole (ASBLRL)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>assignmentID</b></li>
          <li><b>customerID</b></li>
          <li><b>endDate</b></li>
          <li><b>ID</b></li>
          <li><b>roleID</b></li>
          <li><b>startDate</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>assignment</b></li>
          <li><b>customer</b></li>
          <li><b>role</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlan (STAFFP)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
          <li><b>name</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>name</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COPY</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### StaffingPlanResource (STAFFR)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li><b>categoryID</b></li>
          <li><b>ID</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Reference fields</td>
      <td>
        <ul>
          <li><b>category</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li><b>objectCategories</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Core fields</td>
      <td>
        <ul>
          <li><b>ID</b></li>
          <li><b>objCode</b></li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Operations</td>
      <td>
        <ul>
          <li><b>ADD</b></li>
          <li><b>COUNT</b></li>
          <li><b>DELETE</b></li>
          <li><b>EDIT</b></li>
          <li><b>GET</b></li>
          <li><b>REPORT</b></li>
          <li><b>SEARCH</b></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

## Borttagna resurser

Inga resurser togs bort för API-version 20

## Ändrade resurser

### AccessLevelPermissions (ALVPER)

Ett AccessLevelPermissions-objekt representerar en specifik behörighet för att komma åt, skapa eller ändra ett Workfront-objekt. Dessa behörigheter kan sedan kopplas till en åtkomstnivå.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--           <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRequest (ACSREQ)

Om en användare inte har åtkomst till ett objekt i Workfront som de behöver kan de begära åtkomst till det objektet. AccessRequest-objektet representerar denna begäran.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>åtgärd</b>
            </p>
             <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AccessRule (ACSRUL)

Ett AccessRule-objekt representerar en regeluppsättning med anpassade åtkomstnivåer som avgör hur användare kan dela projekt som de skapar.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>coreAction</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>forbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>secondaryActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### AnnouncementAttachment (ANMATT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>fileExtension</b>
            </p>
             <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Godkännande (GODKÄNNANDE)

En viss arbetsuppgift, till exempel en uppgift, ett dokument eller en tidrapport, kan kräva att en ansvarig eller annan användare signerar arbetsposten. Ett Approval-objekt representerar åtgärden för signering av en arbetsuppgift.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>faktureradIntäkter</li>
              <li>budget</li>
              <li>BudgeteradKostnad</li>
              <li>BudgeteradTimme</li>
              <li>BudgeteradArbetskostnad</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>planningBenefit</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad</li>
              <li>planeradUtgiftKostnad</li>
              <li>planeradArbetskostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>planeradRiskkostnad</li>
              <li>planeradVärde</li>
              <li>remainCost</li>
              <li>remainRevenue</li>
              <li>remainRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>planeradKostnad</li>
          <li>planeradIntäkter</li>
          </ul>
          </li>
          <li><p><b>planningDuration</b></p> <p>Flaggorna <code>DYNAMIC</code>, <code>LAZY_READ</code> och <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Flaggan har lagts till <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Det möjliga värdet <code>URH</code> har lagts till (användare och roll per timme) </li>
          <li><p><b>revenueType</b></p> <p>Tillagda möjliga värden <code>URH</code> (användar- och rolltimme), <code>URC</code> (användar- och rolltimme med kap) och <code>URF</code> (användar- och rolltimme plus fast)</li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
          <p>Följande fält har lagts till:</p>
             <ul>
              <li><b>faktureringstariffer</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tilldelning (ASSGN)

Ett uppdragsobjekt representerar anslutningen mellan en arbetsuppgift och användaren, teamet eller gruppen som är tilldelad att arbeta med den.

Tilldelningsobjektet lade till flaggorna `ATTRIBUTE_ATTACHABLE` och `DOMAIN_EXTENDABLE`.


<!--
<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
             <p>Added the following fields:</p>
             <ul>
              <li><b>assignmentBillingRoles<b></li>
              <li><b>billingRates<b></li>
              <li><b>costRates<b></li>
            </ul>
      </td>
   <tr>
      <td role="rowheader">Default fields</td>
      <td>
        <ul>
          <li>
            <p><b>isBillable</b>
            </p>
             <p>Added</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

-->

### Avatar

Ett Avatar-objekt är ett användarfoto.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>Tillagd</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>attachedObjectCode</b>
            </p>
             <p>Tillagd</p>
           </li>
          </li>
        </ul>
      </td>
   <tr>
      <td role="rowheader">Operationer</td>
      <td>
        <ul>
          <li>
            <p><b>KOPIA</b>
            </p>
             <p>Tillagd</p>
           </li>
          </li>
        </ul>
      </td>
    </tr>
    </tr>
 </tbody>
</table>

### Baslinje (BLIN)

Baslinjer är bilder på hur ett projekts prestanda ser ut vid en viss tidpunkt. De lagrar viktig information om projektet, t.ex. nyckeldatum, förlopp, kostnad och intäktsvärden.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>budget</li>
              <li>eac</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>planeradKostnad</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Flaggan har lagts till <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Originalaktivitet (BSTSK)

Baslinjer är bilder på hur ett projekts prestanda ser ut vid en viss tidpunkt. De lagrar viktig information om projektet, t.ex. nyckeldatum, förlopp, kostnad och intäktsvärden. När du skapar en baslinje hämtas uppgiftsinformationen också till baslinjeuppgifterna för den baslinjen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>planeradKostnad</li>
          </ul>
          </li>
          <li><p><b>eac</b></p> <p>Flaggan har lagts till <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Faktureringspost (BILL)

Ett BillingRecord-objekt registrerar intäkter, timmar eller utgifter som kan faktureras. Den här informationen kan användas för att skapa fakturor i ett externt redovisningssystem.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>belopp</li>
              <li>otherAmount</li>
            </ul>
          </li>
          <li><p><b>entryDate</b></p> <p>Tillagd</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


<!--### Category (CTGY)

A Category object is a custom form.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direct fields</td>
      <td>
        <ul>
          <li>
            <p><b>catObjCode</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
          <li>
            <p><b>objTypes</b>
            </p>
             <p>Added the following possible values:</p>
             <ul>
              <li><p><code>BOOKNG</code> (Booking)</p> </li>
              <li><p><code>STAFFP</code> (Staffing Plan)</p> </li>
              <li><p><code>STAFFR</code> (Staffing plan resources)</p> </li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>-->

### CategoryParameter (CTGYPA)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>konfigurationer</b>
            </p>
             <p>Tillagd</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Företag (CMPY)

Ett företagsobjekt representerar en organisation som består av en samling personer.

Företagsobjektet lade till flaggan `SHARABLE`.

<!--

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Collection fields</td>
      <td>
        <ul>
          <li>
            <p><b>billingRates</b>
            </p>
             <p>Added</p>
          </li>
          <li>
            <p><b>costRates</b>
            </p>
             <p>Added</p>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

-->

### CustomerPreferences (CUSTPR)

Ett CustomerPreferences-objekt representerar den uppsättning inställningar som en kund har ställt in för sin instans av Workfront.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>namn</b>
            </p>
             <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li><p><code>project.mgmt:default.project.singleassignmentschedule</code> (ett tilldelningsschema)</p></li>
              <li><p><code>project.mgmt:logged.taskissue.move</code> (config.loggedtaskIssuemove)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### ExchangeRate (EXRAT)

Ett ExchangeRate-objekt representerar en valutakurs som har ställts in i Workfront. ExchangeRate-objekt är inte dynamiska.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
           <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>ränta</li>
      </td>
    </tr>
  </tbody>
</table>


### FinancialData (FINDAT)

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualExpenseCost</li>
              <li>actualFixedRevenue</li>
              <li>actualLaborCost</li>
              <li>actualLaborCostHours</li>
              <li>actualLaborRevenue</li>
              <li>actualNonBillableExpenseCost</li>
              <li>fixedCost</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradUtgiftKostnad</li>
              <li>planeradFastIntäkter</li>
              <li>planeradArbetskostnad</li>
              <li>planeradArbetstidKostnadstid</li>
              <li>planeradArbetsplatsIntäkter</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>totalActualCost</li>
              <li>totalActualRevenue</li>
              <li>totalPlanerad kostnad</li>
              <li>totalPlanerad intäkt</li>
              <li>totalVarianceCost</li>
              <li>totalVarianceRevenue</li>
              <li>variansUtgiftKostnad</li>
              <li>varianceLaborCost</li>
              <li>varianceLaborCostHours</li>
              <li>varianceLaborRevenue</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Grupp (GRUPP)

Ett Group-objekt representerar en uppsättning användare och team. Grupper representerar ofta avdelningsstruktur.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>valuta</b>
            </p>
             <p>Tillagd</p>
          </li>
         </ul>
      </td>
    </tr>
  </tbody>
</table>

### Timme (TIMME)

Ett Timobjekt representerar en timme som loggas av en användare på en tidrapport.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
              <li>resourceRevenue</li>
          </ul>
          </li>
          <li><p><b>ratesOrigin</b></p> <p>Tillagd</p></li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>



### OpTask (OPTASK)

Ett OpTask-objekt kallas vanligtvis för ett problem. Ett problem är en arbetsuppgift som vanligtvis anger att det finns ett problem som förhindrar att en uppgift eller ett projekt slutförs. Ett problem kan också vara en Help Desk-begäran. Ändringsorder, begäranden och buggar är också problem.

OpTask-objektet lade till flaggan DOMAIN_EXTENDABLE

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualCost</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
              <li>actualCost</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Parameter (PARAM)

Ett Parameter-objekt är ett anpassat fält.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>INTRNL</code> (Intern sökning)</p>
              </li>
              <li>
                <p><code>MULTINTRNL</code> (Flerval intern sökning)</p>
              </li>
              <li>
                <p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p>
              </li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>



### Portfolio (PORT)

Ett Portfolio-objekt är en samling projekt som konkurrerar om samma resurser, vanligtvis pengar eller personer som ska slutföra dem.

Portfolio-objektet lade till flaggan `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>justerad</li>
              <li>budget</li>
              <li>valuta</li>
              <li>netValue</li>
              <li>onBudget</li>
              <li>onTime</li>
              <li>portfolioNetValue</li>
              <li>portfolioRoi</li>
              <li>roi</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
   </tbody>
</table>

### Program (PRGM)

Ett Program-objekt är en delmängd av projekt i en portfölj, där liknande projekt kan grupperas tillsammans.

Programobjektet lade till flaggan `DOMAIN_EXTENDABLE`.

### Projekt (PROJ)

Projekt är arbetsuppgifter inom Workfront och är en viktig byggsten i det sätt på vilket Workfront hjälper människor att arbeta. Ett Project-objekt representerar en grupp med uppgifter med ett gemensamt, specifikt mål.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBenefit</li>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>actualRiskCost</li>
              <li>actualValue</li>
              <li>bcwp</li>
              <li>bcws</li>
              <li>faktureradIntäkter</li>
              <li>budget</li>
              <li>BudgeteradKostnad</li>
              <li>BudgeteradTimme</li>
              <li>BudgeteradArbetskostnad</li>
              <li>eac</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>planningBenefit</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad</li>
              <li>planeradUtgiftKostnad</li>
              <li>planeradArbetskostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>planeradIntäkter</li>
              <li>planeradRiskkostnad</li>
              <li>planeradVärde</li>
              <li>remainCost</li>
              <li>remainRevenue</li>
              <li>remainRiskCost</li>
              <li>resourcePlannerBudgetedHours</li>
              <li>resourcePlannerBudgetedLaborCost</li>
              <li>riskPerformanceIndex</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>planeradKostnad</li>
          <li>planeradIntäkter</li>
          </ul>
          </li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Flaggan har lagts till <code>CURRENCY</code></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### QueueDef (QUED)

Ett QueueDef-objekt representerar en kö, vilket är ett projekt som har publicerats i Help Desk-området där användarna kan skicka utgåvor till den.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>requestedCoreAction</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
          <li>
            <p><b>requestedForbiddenActions</b>
            </p>
            <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>REMOVE_CUSTOMFORM</code> (Ta bort från anpassade data)</p>
              </li>
              <li>
                <p><code>ADD_SUB_PROJECTS</code> (Lägg till delprojekt)</p>
              </li>
<!--              <li>
                <p><code>ASSIGN_STAFFING_PLAN_RESOURCES</code> (Assign resources)</p>
              </li>-->
            </ul>
<!--            <p>Modified the following possible values:</p>
             <ul>
              <li>
                <p><code>ADD_BOOKINGS</code> (Add Bookings) changed to <code>MANAGE_BOOKINGS</code> (Manage Bookings)</p>
              </li>
            </ul>-->
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>


### Hastighet (RATE)

Ett Rate-objekt representerar en faktureringsfrekvens i Workfront.

Rate-objektet lade till flaggan `ATTRIBUTE_ATTACHABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>costPerHour</li>
              <li>localBillingPerHour</li>
              <li>localCostPerHour</li>
              <li>localCurrency</li>
              <li>rateValue</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>costPerHour</li>
          <li>localBillingPerHour</li>
          <li>localCostPerHour</li>
          <li>rateValue</li>
          </ul>
          </li>
         <li>
          <p>Följande fält har lagts till:
          <ul>
          <li>valuta</li>
          <li>låst</li>
          <li>type</li>
          <li>value</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Roll (ROLE)

Ett rollobjekt (jobbroll) representerar en funktionskapacitet eller en kompetensuppsättning som en användare kan fylla, till exempel Designer eller Product Manager.

Rollobjektet lade till flaggan `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>faktureringPerTimme</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
        <ul>
          <li>
          <p>Följande fält har lagts till:
          <ul>
          <li>faktureringstariffer</li>
          <li>costRates</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScheduledReport (SCHREP)

Ett ScheduledReport-objekt representerar en rapport som har konfigurerats att schemaläggas för leverans.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>format</b>
            </p>
             <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>tiff</code> (enum.fileextension.tiff)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### ScoreCardQuestion (SCOREQ)

Ett ScoreCardQuestion-objekt representerar en fråga som har lagts till i ett styrkort. Dessa frågor avgörs vanligtvis av Portfolio-chefen och deras svar gör det möjligt för den som ansvarar för ledningen att förstå hur väl ett projekt passar in i portfolions mål.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>displayType</b>
            </p>
             <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li><p><code>INTRNL</code> (Intern sökning)</p></li>
              <li><p><code>MULTINTRNL</code> (Flerval intern sökning)</p></li>
              <li><p><code>UIEXTNSION</code> (enum.parameterdisplaytypeenum.uiextension)</p></li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Aktivitet (AKTIVITET)

Ett Task-objekt representerar en arbetsuppgift som måste utföras som ett steg mot att uppnå ett slutligt mål (slutföra ett projekt).

Aktivitetsobjektet lade till flaggan `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad/li&gt;
              <li>planeradUtgiftKostnad</li>
              <li>planeradArbetskostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>planeradIntäkter</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>planeradKostnad</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Följande möjliga värden har lagts till:<ul><li><code>URH</code> (Användare och roll varje timme)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Följande möjliga värden har lagts till:<ul><li><code>URH</code> (Användare och roll varje timme)</li><li><code>URC</code> (Användare och roll per timme med versaler)</li><li><code>URF</code> (Användare och roll, timvis plus fast)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Mall (TMPL)

Ett Template-objekt representerar ett mönster för ett projekt. Projekt kan skapas från mallar för att spara tid. En mall innehåller ett team och uppgifter som kopieras till alla projekt som skapas från mallen.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>budget</li>
              <li>fixedCost</li>
              <li>fixedRevenue</li>
              <li>planningBenefit</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad</li>
              <li>planeradUtgiftKostnad</li>
              <li>planeradArbetskostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>planeradIntäkter</li>
              <li>planeradRiskkostnad</li>
              <li>workRequired</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>planeradKostnad</li>
          <li>planeradIntäkter</li>
          </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
          <p>Följande fält har lagts till:</p>
             <ul>
              <li><b>faktureringstariffer</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### TemplateTask (TTSK)

Ett TemplateTask-objekt representerar en aktivitet som är en del av en Template. Malluppgifter blir uppgifter i det projekt där mallen används.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>faktureringsbelopp</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad/li&gt;
              <li>planeradUtgiftKostnad</li>
              <li>planeradArbetskostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>planeradIntäkter</li>
              <li>revenueType</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>planeradKostnad</li>
          <li>planeradIntäkter</li>
          </ul>
          </li>
          <li><p><b>costType</b></p> <p>Följande möjliga värden har lagts till:<ul><li><code>URH</code> (Användare och roll varje timme)</li></ul></li>
          <li><p><b>revenueType</b></p> <p>Följande möjliga värden har lagts till:<ul><li><code>URH</code> (Användare och roll varje timme)</li><li><code>URC</code> (Användare och roll per timme med versaler)</li><li><code>URF</code> (Användare och roll, timvis plus fast)</li></ul></li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Tidrapport (TSPEN)

Ett Timesheet-objekt representerar ett virtuellt tidkort som gör att användare kan ange faktiskt antal arbetstimmar för uppgifter, projekt och obemannade timtyper.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Kärnfält</td>
      <td>
        <ul>
          <li>
            <p><b>objCode</b>
            </p>
             <p>Borttagen</p>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Uppdatera (UPPDATERA)

Arbetsobjekt i Workfront kan uppdateras för att hålla användarna informerade om den aktuella statusen. Ett Update-objekt representerar en av dessa uppdateringar. Uppdateringar kan anges av användare eller skapas av Workfront-systemet.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p><b>updateType</b>
            </p>
             <p>Följande möjliga värden har lagts till:</p>
             <ul>
              <li>
                <p><code>externalFolderMetadataError</code> (enum.updatetypeenum.externalFolderMetadataError)</p>
              </li>
            </ul>
          </li>
          </li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>

### Användare (ANVÄNDARE)

Ett User-objekt representerar en person med ett konto i Workfront som kan logga in och interagera med systemet.

Användarobjektet lade till fälten `ATTRIBUTE_ATTACHABLE` och `DOMAIN_EXTENDABLE`.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>faktureringPerTimme</li>
              <li>costPerHour</li>
            </ul>
          </li>
        </ul>
      </td>
    </tr>
    <tr>
      <td role="rowheader">Samlingsfält</td>
      <td>
          <p>Följande fält har lagts till:</p>
             <ul>
              <li><b>faktureringstariffer</b></li>
              <li><b>costRates</b></li>
            </ul>
      </td>
    </tr>
  </tbody>
</table>

### Arbete (ARBETE)

Ett Work-objekt är ett vanligt gränssnitt som både Task och OpTask ärver och delar gemensam kod mellan de två.

<table>
  <col/>
  <col/>
  <tbody>
    <tr>
      <td role="rowheader">Direktfält</td>
      <td>
        <ul>
          <li>
            <p>Följande fält har lagt till flaggan <code>RESTRICTABLE</code>:
            </p>
             <ul>
              <li>actualBillableExpenseCost</li>
              <li>actualCost</li>
              <li>actualExpenseCost</li>
              <li>actualLaborCost</li>
              <li>actualNonBillableExpenseCost</li>
              <li>actualRevenue</li>
              <li>costAmount</li>
              <li>costType</li>
              <li>planeradFakturerbarUtgiftKostnad</li>
              <li>planeradKostnad</li>
              <li>planeradUtgiftKostnad</li>
              <li>planeradArbetskostnad</li>
              <li>planeradEjFakturerbarUtgiftKostnad</li>
              <li>planeradIntäkter</li>
            </ul>
          </li>
          <li>
          <p>Följande fält har ändrat typ från <code>double</code> till <code>class java.math.BigDecimal</code>:
          <ul>
          <li>actualCost</li>
          <li>actualRevenue</li>
          <li>planeradKostnad</li>
          <li>planeradIntäkter</li>
          </ul>
          </li>
          <li><p><b>planningDuration</b></p> <p>Flaggorna <code>DYNAMIC</code>, <code>LAZY_READ</code> och <code>READ_ONLY</code></li>
          <li><p><b>resourcePlannerBudgetedHours</b></p> <p>Flaggan har lagts till <code>CURRENCY</code></li>
          <li><p><b>costType</b></p> <p>Det möjliga värdet <code>URH</code> har lagts till (användare och roll per timme) </li>
          <li><p><b>revenueType</b></p> <p>Tillagda möjliga värden <code>URH</code> (användar- och rolltimme), <code>URC</code> (användar- och rolltimme med kap) och <code>URF</code> (användar- och rolltimme plus fast)</li>
        </ul>
      </td>
    </tr>
  </tbody>
</table>



