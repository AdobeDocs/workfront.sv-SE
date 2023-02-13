---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Beräkningsexempel - beräkna EAC på projektnivå
description: PIM = timbaserad
author: Alina
feature: Work Management
exl-id: ff88b7e3-2a5b-464f-bed1-6848067840b8
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '1768'
ht-degree: 6%

---

# Beräkningsexempel - beräkna EAC på projektnivå

## EAC-metod: Beräkna på projektnivå

* [PIM = timbaserad](#pim-hour-based)
* [PIM= Kostnadsbaserad](#pim-cost-based)

### PIM = timbaserad {#pim-hour-based}

* [Enkelt exempel: projektet saknar underordnade uppgifter](#simple-example-project-has-no-children-tasks)
* [Komplicerat exempel: projektet har underordnade uppgifter](#complicated-example-project-has-children-tasks)

#### Enkelt exempel: projektet saknar underordnade uppgifter {#simple-example-project-has-no-children-tasks}

PIM = timbaserad

EAC-metod = Beräkna på projektnivå ***

1. Skapa projekt A med tre uppgifter (inga underordnade uppgifter) som alla är tilldelade till Användare 1 vars kostnad/timme är 100,00 USD.
1. Lägg till planerade och faktiska timmar för varje uppgift och % slutfört enligt tabellen nedan:

   <table style="table-layout:auto">
    <col>
    <col>
    <col>
    <col>
    <thead>
     <tr>
      <th><br><p><strong>Uppgift</strong></p></th>
      <th><br><p><strong>Antal timmar</strong></p></th>
      <th><br><p><strong>Agera timmar</strong></p></th>
      <th><p><strong>% klart</strong></p></th>
     </tr>
    </thead>
    <tbody>
     <tr>
      <td><p>Aktivitet 1</p></td>
      <td><p>5 timmar</p></td>
      <td><p>25 tim</p></td>
      <td><p>20%</p></td>
     </tr>
     <tr>
      <td><p>Aktivitet 2</p></td>
      <td><p>10 tim</p></td>
      <td><p>25 tim</p></td>
      <td><p>30%</p></td>
     </tr>
     <tr>
      <td><p>Aktivitet 3</p></td>
      <td><p>15 tim</p></td>
      <td><p>25 tim</p></td>
      <td><p>40%</p></td>
     </tr>
    </tbody>
   </table>

1. Beräkna om finansiering av projektet.
1. **CPI för aktivitet 1** = 0,04 beräknat enligt följande:\
   **CPI för aktivitet 1** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
      *ELSE* CPI = 1\
   **CPI för aktivitet 1** = 1 / 25\
   **CPI för aktivitet 1** = .04

1. **EAC för uppgift 1** = 125 tim beräknat enligt följande:\
   **EAC för uppgift 1** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för uppgift 1** = 5 / .04\
   **EAC för uppgift 1** = 125 tim****

1. CPI/EAC för uppgifter 2 och 3 är:\
   Aktivitet 2 = 0,12 / 83,33 tim\
   Aktivitet 3 = 0,24 / 62,5 tim

1. **CPI för projekt** = 0,13 beräknat enligt följande:\
   **CPI för projekt** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI för projekt** = 10 / 75\
   **CPI för projekt** = .13

1. **EAC för projekt** = 225 tim beräknat enligt följande:\
   **EAC för projekt** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för projekt** = 30 / .13333\
   **EAC för projekt** = 225 tim

#### Komplicerat exempel: projektet har underordnade uppgifter {#complicated-example-project-has-children-tasks}

PIM = timbaserad

EAC-metod = Beräkna på projektnivå

1. Skapa projekt A med sex uppgifter där Aktivitet 3 är överordnad Aktiviteter 4 och 5 och Aktivitet 1 är överordnad Aktiviteter 2 och 3 enligt nedan:\
   Aktivitet 1\
      Aktivitet 2\
      Aktivitet 3\
         Aktivitet 4\
         Aktivitet 5\
   Aktivitet 6

1. Tilldela uppgifter 2, 4, 5 och 6 till Användare 1 vars kostnad/timme är 100,00 USD.
1. Lägg till planerade/faktiska timmar för varje uppgift och % slutfört enligt tabellen nedan.

   >[!NOTE]
   >
   >För uppgifter 1 och 3 lägger du bara till faktiska timmar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Uppgift</strong> </p> </th> 
   <th> <br> <p><strong>Antal timmar</strong> </p> </th> 
   <th> <br> <p><strong>Agera timmar</strong> </p> </th> 
   <th> <p><strong>% klart</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> </td> 
   <td> <p>10 tim</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>5 timmar</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> </td> 
   <td> <p>10 tim</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 4</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 5</p> </td> 
   <td> <p>15 tim</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 6</p> </td> 
   <td> <p>20 tim</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Lägg till 50 timmar direkt i projektet (Mer > Timmar > Loggtimmar).
1. **CPI för aktivitet 2** = .1 beräknad enligt följande:\
   **CPI för aktivitet 2** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI för aktivitet 2** = 1 / 10\
   **CPI för aktivitet 2** = .1

1. **EAC för uppgift 2** = 50 tim beräknat enligt följande:\
   **EAC för uppgift 2** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för uppgift 2** = 5 / .1\
   **EAC för uppgift 2** = 50 tim

1. CPI/EAC för uppgifter 4, 5 och 6 är följande:\
   Aktivitet 4: 0,4 / 25 tim\
   Aktivitet 5: 0,75/20 tim\
   Aktivitet 6: 1,2 / 16,67 tim

1. **CPI för aktivitet 3** = 0,38 beräknat enligt följande:\
   **CPI för aktivitet 3** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI för aktivitet 3** = 11.5 / 30\
   **CPI för aktivitet 3** = 0,38

1. **EAC för uppgift 3** = 65,22 tim beräknat enligt följande:\
   **EAC för uppgift 3** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för uppgift 3** = 25 / .383333\
   **EAC för uppgift 3** = 65,22 tim

1. **CPI för aktivitet 1** = 0,25 beräknat enligt följande:\
   **CPI för aktivitet 1** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI för aktivitet 1** = 12.5 / 50\
   **CPI för aktivitet 1** = 0,25

1. **EAC för uppgift 1** = 120 tim beräknat enligt följande:\
   **EAC för uppgift 1** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för uppgift 1** = 30/.25\
   **EAC för uppgift 1** = 120 tim

1. **CPI för projekt** = 0,22 beräknat enligt följande:\
   **CPI för projekt** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI för projekt** = 24.5 / 110\
   **CPI för projekt** = .22272\
   **CPI för projekt** = .22

1. **EAC för projekt** = 224,49 tim beräknat enligt följande:\
   **EAC för projekt** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för projekt** = 50 / .22272\
   **EAC för projekt** = 224,49 tim

### PIM= Kostnadsbaserad {#pim-cost-based}

* [Enkelt exempel: projektet saknar underordnade uppgifter](#simple-example-project-has-no-children-tasks)
* [Komplicerat exempel: projektet har underordnade uppgifter](#complicated-example-project-has-children-tasks)

#### Enkelt exempel: projektet saknar underordnade uppgifter {#simple-example-project-has-no-children-tasks-1}

PIM = kostnadsbaserad

EAC-metod = Beräkna på projektnivå

1. Skapa projekt A med tre uppgifter (inga underordnade uppgifter) som alla är tilldelade till Användare 1 vars kostnad/timme är 100,00 USD.
1. Lägg till planerade/faktiska timmar för varje uppgift och % slutfört enligt tabellen nedan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Uppgift</strong> </p> </th> 
   <th> <br> <p><strong>Antal timmar</strong> </p> </th> 
   <th> <br> <p><strong>Plans - kr</strong> </p> </th> 
   <th> <br> <p><strong>Agera timmar</strong> </p> </th> 
   <th> <br> <p><strong>Lag - Lbr.kostnad</strong> </p> </th> 
   <th> <p><strong>% klart</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>5 timmar</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>25 tim</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>25 tim</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> <p>15 tim</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>25 tim</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Lägg till utgifter för varje uppgift enligt tabellen nedan:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Uppgift</strong> </p> </th> 
   <th> <p><strong>Utgift</strong> </p> </th> 
   <th> <p><strong>Planerat belopp</strong> </p> </th> 
   <th> <p><strong>Faktiskt belopp</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>Aktivitet 1 Utg 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>Aktivitet 1 exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>Aktivitet 2 - exp</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> <p>Aktivitet 3 - exp</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Lägg till två utgifter i projektet (dvs. inte knutna till en uppgift) enligt följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Utgift</strong> </p> </th> 
   <th> <p><strong>Planerat belopp</strong> </p> </th> 
   <th> <p><strong>Faktiskt belopp</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 1 exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Baserat på ovanstående värden fastställs de uppkomna/ej uppkomna kostnaderna enligt följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Uppgift</strong> </p> </th> 
   <th> <p><strong>Ej fakturerad planerad kostnad</strong> </p> </th> 
   <th> <p><strong>Inkommande planerad utgift</strong> </p> </th> 
   <th> <p><strong>Faktisk kostnad uppkom</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$200.00</p> </td> 
   <td> <p>$100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>$3,000.00</p> </td> 
   <td> <p>$2,300.00</p> </td> 
   <td> <p> $2,700.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. Kör Beräkna om ekonomi från projektåtgärder
1. **CPI för aktivitet 1** = .14
1. **CPI****för uppgift 1** = 0,14 beräknat enligt följande:\
   **CPI**  **för uppgift 1** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *    ELSE* CPI = CPI_Labor\
   **CPI****för uppgift 1** = (100+300) / (2500+400)\
   **CPI**  **för uppgift 1** = 400 / 2900\
   **CPI**  **för uppgift 1**  = 0,14***

1. **EAC****för uppgift 1** = $13 400.00\
   **CPI-arbete**  **för uppgift 1** = OM Faktisk arbetskostnad &lt;> 0 SEDAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI-arbete**  **för uppgift 1** = 100/2500\
   **CPI-arbete**  **för uppgift 1** = .04 ****** EAC-arbete ****för uppgift 1 **=*IF *CPI_Labor &lt;> 0*SEDAN *EAC-arbete = Planerad arbetskostnad/CPI_Labor\
   *    ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC-arbete ****för uppgift 1** = 500.00/.04\
   **EAC Labor****för aktivitet 1** = $12 500.00\
   **EAC-utgift****för aktivitet 1** = IncurrusActualExpenseCost + NotIncoundsPlannedExpense\
   **EAC-utgift****för aktivitet 1** = $400.00 + $500.00\
   **EAC-utgift****för aktivitet 1** = $900.00\
   **EAC****för uppgift 1** = EAC Labor + EAC-kostnad\
   **EAC****för uppgift 1**  = $12 500.00 + $900.00\
   **EAC****för uppgift 1**  = $13 400.00

1. Här är CPI-/EAC-värdena för Aktivitet 2 och Aktivitet 3:\
   Aktivitet 2 = 0,19 / $8,433.33\
   Aktivitet 3 = 0,44 / $6,950.00

1. **CPI för projekt** = 0,32 beräknat enligt följande:\
   **CPI****för projekt** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****för projekt** = (1000 + 2300) / (7500 + 2700)\
   **CPI****för projekt** = 3300 / 10200\
   **CPI****för projekt** = .32

1. **EAC för projekt** = $28 200.00 beräknat enligt följande:\
   **CPI-arbete****för projekt** = OM Faktisk arbetskostnad &lt;> 0 SEDAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed/Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI-arbete****för projekt** = 1000 / 7500\
   **CPI-arbete****för projekt** = .13333\
   **CPI-arbete****för projekt** = .13

   **EAC Labor****for Project** = *IF* CPI_Labor &lt;> 0 *SEDAN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC Labor****for Project** = 3000/ .13333\
   **EAC Labor****for Project** = $22 500.00

   **EAC-utgift****Projekt** =

   ```
   IncurredActualExpenseCost + NotIncurredPlannedExpense
   ```

   **EAC-utgift****Projekt** = $3000.00 + 2700.00\
   **EAC-utgift****Projekt** = $5 700.00

   **EAC****Project** = EAC Labor + EAC-kostnad\
   **EAC****Project**  = $22 500.00 + $5 700.00\
   **EAC****Project**  = $28 200.00

#### Komplicerat exempel: projektet har underordnade uppgifter {#complicated-example-project-has-children-tasks-1}

PIM = kostnadsbaserad

EAC-metod = Beräkna på projektnivå

1. Skapa projekt A med sex uppgifter där Aktivitet 3 är överordnad Aktiviteter 4 och 5 och Aktivitet 1 är överordnad Aktiviteter 2 och 3 enligt nedan:\
   Aktivitet 1\
      Aktivitet 2\
      Aktivitet 3\
         Aktivitet 4\
         Aktivitet 5\
   Aktivitet 6

1. Tilldela uppgifter 2, 4, 5 och 6 till Användare 1 vars kostnad/timme är 100,00 USD.
1. Lägg till planerade/faktiska timmar för varje uppgift och % slutfört enligt tabellen nedan.

   >[!NOTE]
   >
   >För uppgifter 1 och 3 lägger du bara till faktiska timmar.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <br> <p><strong>Uppgift</strong> </p> </th> 
   <th> <br> <p><strong>Antal timmar</strong> </p> </th> 
   <th> <br> <p><strong>Plans - kr</strong> </p> </th> 
   <th> <br> <p><strong>Agera timmar</strong> </p> </th> 
   <th> <br> <p><strong>Lag - Lbr.kostnad</strong> </p> </th> 
   <th> <p><strong>% klart</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>5 timmar</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> </td> 
   <td> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 4</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 5</p> </td> 
   <td> <p>15 tim</p> </td> 
   <td> <p>$1,500.00</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>50%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 6</p> </td> 
   <td> <p>20 tim</p> </td> 
   <td> <p>$2,000.00</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>60%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Lägg till 50 timmar direkt i projektet (Mer > Timmar > Loggtimmar) så att 5 000,00 USD av den faktiska arbetskostnaden registreras direkt i projektet. ****
1. Lägg till utgifter för varje uppgift enligt tabellen nedan (jag har lagt till en tom rad mellan varje uppgift för att göra den lättare att läsa):

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Uppgift</strong> </p> </th> 
   <th> <p><strong>Utgift</strong> </p> </th> 
   <th> <p><strong>Planerat belopp</strong> </p> </th> 
   <th> <p><strong>Faktiskt belopp</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>Aktivitet 1 Utg 1</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>-$400.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>Aktivitet 1 exp 2</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>Aktivitet 1 Utg. 3</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>Aktivitet 2, exp 1</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>Aktivitet 2, exp 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>Aktivitet 2 exp. 3</p> </td> 
   <td> <p>-$200.00</p> </td> 
   <td> <p>$600.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>Aktivitet 2 exp 4</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> <p>Aktivitet 3 - exp</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 4</p> </td> 
   <td> <p>Aktivitet 4 Utg. 1</p> </td> 
   <td> <p>$800.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 4</p> </td> 
   <td> <p>Aktivitet 4, exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 4 </p> </td> 
   <td> <p>Aktivitet 4 Utg. 3</p> </td> 
   <td> <p>-200.00</p> </td> 
   <td> <p>$0.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 5</p> </td> 
   <td> <p>Aktivitet 5 Utg. 1</p> </td> 
   <td> <p>$700.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 5</p> </td> 
   <td> <p>Aktivitet 5 exp 2</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 5</p> </td> 
   <td> <p>Aktivitet 5 Utg. 3</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>-$200.00</p> </td> 
  </tr> 
  <tr> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
   <td> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 6</p> </td> 
   <td> <p>Aktivitet 6 Utg. 1</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 6</p> </td> 
   <td> <p>Aktivitet 6 exp 2</p> </td> 
   <td> <p>$500.00</p> </td> 
   <td> <p>-$300.0</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Lägg till två utgifter i projektet (dvs. inte knutna till en uppgift) enligt följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Utgift</strong> </p> </th> 
   <th> <p><strong>Planerat belopp</strong> </p> </th> 
   <th> <p><strong>Faktiskt belopp</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Project Exp 1</p> </td> 
   <td> <p>$1,000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 1 exp 2</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p> $0.00 <strong></strong></p> </td> 
  </tr> 
 </tbody> 
</table>

1. På grundval av ovanstående värden fastställs de uppkomna/ej uppkomna kostnaderna enligt följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th> <p><strong>Uppgift</strong> </p> </th> 
   <th> <p><strong>Ej fakturerad planerad kostnad</strong> </p> </th> 
   <th> <p><strong>Inkommande planerad utgift</strong> </p> </th> 
   <th> <p><strong>Faktisk kostnad uppkom</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td> <p>Aktivitet 1</p> </td> 
   <td> <p>$400.00</p> </td> 
   <td> <p>-$500.00</p> </td> 
   <td> <p>$800.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>-$400.00</p> </td> 
   <td> <p>$300.00</p> </td> 
   <td> <p>$1,300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$1,000.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 4</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>-$100.00</p> </td> 
   <td> <p>$300.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 5</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$1,100.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 6</p> </td> 
   <td> <p>$0.00</p> </td> 
   <td> <p>$600.00</p> </td> 
   <td> <p>$700.00</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Projekt</p> </td> 
   <td> <p>$2,500.00</p> </td> 
   <td> <p>$1000.00</p> </td> 
   <td> <p>$1,500.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Kör Beräkna om ekonomi från projektåtgärder
1. **CPI** för uppgift 2 = 0,17, beräknad enligt följande:\
   **Processoraktivitet 2** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN* CPI = (TotalBudgetedCostWorkPerformed + IncurringadPlaneradKostnad) / (ActualLaborCost + IncurredActualExpenseCost)\
   *   ELSE* CPI = CPI_Labor\
   **CPI****Aktivitet 2** = (100+300) / (1000+1300)\
   **CPI****Aktivitet 2**  = 400 / 2300\
   **CPI****Aktivitet 2**  = .17

1. **EAC** för uppgift 2 = $5 900.00\
   **CPI-arbete****Aktivitet 2** = OM Faktisk arbetskostnad &lt;> 0 THAN CPI_Labor = TotalBudgetedCostWorkPerformed / Faktisk arbetskostnad\
      ELSE CPI_Labor = 1\
   **CPI-arbete****Aktivitet 2** = 100/1000\
   **CPI-arbete****Aktivitet 2** = .1

   **EAC Labor****Aktivitet 2** = *IF* CPI_Labor &lt;> 0 *SEDAN*

   ```
   EAC Labor = Planned Labor Cost/CPI_Labor
   ```

   *   ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC Labor****Aktivitet 2** = 500.00/.1\
   **EAC Labor****Aktivitet 2** = $5 000.00 ****** EAC-utgift ****Aktivitet 2 **= IncurrusActualExpenseCost + NotIncoundsPlannedExpense\
   **EAC-utgift ****Uppgift 2** = $1 300.00 + -$400.00\
   **EAC-utgift****Aktivitet 2** = $900.00

   **EAC****Aktivitet 2** = EAC Labor + EAC-kostnad\
   **EAC****Aktivitet 2**  = $5 000.00 + $900.00\
   **EAC****Aktivitet 2**  = $5 900.00

1. CPI/EAC för uppgifter 4, 5 och 6 bestäms på samma sätt så jag bara anger värdena nedan:\
   Aktivitet 4: .23 / $3 400.00\
   Aktivitet 5: 0,64 / 3 100,00 kr\
   Aktivitet 6: 1,06 / $2,366,67

1. CPI för uppgift 3 = 0,31 beräknat enligt följande:\
   **CPI****Aktivitet 3** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****Aktivitet 3**  = (1 150 + 500) / (3 000 + 2 400)\
   **CPI****Aktivitet 3**  = 1650 / 5400\
   **CPI****Aktivitet 3**  = .31 ****** EAC för uppgift 3 **= $9,521.74 beräknat enligt följande:\
   **CPI-arbete ****Aktivitet 3** = OM Faktisk arbetskostnad &lt;> 0 SEDAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI-arbete****Aktivitet 3** = 1150/3000\
   **CPI-arbete****Aktivitet 3** = .383333\
   **CPI-arbete****Aktivitet 3** = 0,38

   **EAC Labor****Aktivitet 3** = *IF* CPI_Labor &lt;> 0 *SEDAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC Labor****Aktivitet 3** = $2 500.00 / .38333\
   **EAC Labor****Aktivitet 3** = $6 521.74

   **EAC-utgift****Aktivitet 3** = IncurrusActualExpenseCost + NotIncoundsPlannedExpense\
   **EAC-utgift****Aktivitet 3** = $2 400.00 + $600.00\
   **EAC-utgift****Aktivitet 3** = $3 000.00

   **EAC****Uppgift 3** = EAC Labor + EAC-kostnad\
   **EAC****Uppgift 3**  = $6 521.74 + $3 000.00\
   **EAC****Uppgift 3**  = $9,521.74

1. CPI för uppgift 1 = 0,16 beräknat enligt följande:\
   **CPI****Aktivitet 1** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****Aktivitet 1**  = (1250 + 300) / (5000 + 4500)\
   **CPI****Aktivitet 1**  = 1550 / 9500=\
   **CPI****Aktivitet 1**  = .16

1. EAC för uppgift 1 är $17 100,00 beräknat enligt följande:\
   **CPI-arbete****Aktivitet 1** = OM Faktisk arbetskostnad &lt;> 0 SEDAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI-arbete****Aktivitet 1** = 1250 / 5000\
   **CPI-arbete****Aktivitet 1** = 0,25

   **EAC Labor****Aktivitet 1** = *IF* CPI_Labor &lt;> 0 *SEDAN* EAC-arbete = Planerad arbetskostnad/CPI_Labor\
   *   ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC Labor****Aktivitet 1** = $3 000.00 / .25\
   **EAC Labor****Aktivitet 1** = $12 000.00

   **EAC-utgift****Aktivitet 1** = IncurrusActualExpenseCost + NotIncoundsPlannedExpense\
   **EAC-utgift****Aktivitet 1** = $4500 + 600\
   **EAC-utgift****Aktivitet 1** = $5 100.00

   **EAC****Aktivitet 1** = EAC Labor + EAC-kostnad\
   **EAC****Aktivitet 1**  = $12 000.00 + 5 100.00\
   **EAC****Aktivitet 1**  = $17 100.00

1. CPI för Project är 0,25\
   **CPI****för projekt** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor

   **CPI****för projekt** = (2450 + 1900) / (11000 + 6700)\
   **CPI****för projekt** = 4350 / 17700\
   **CPI****för projekt** = 0,25

1. **EAC för projekt** = $32,248.98 beräknat enligt följande:\
   **CPI-arbete****för projekt** = OM Faktisk arbetskostnad &lt;> 0 SEDAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI-arbete****för projekt** = 2450 / 11000\
   **CPI-arbete****för projekt** = .22272\
   **CPI-arbete****för projekt** = .22

   **EAC Labor****for Project** = *IF* CPI_Labor &lt;> 0 *SEDAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC Labor****for Project** = $5 000.00 / .22272\
   **EAC Labor****for Project** = $22,448.97959\
   **EAC Labor****for Project** = $22,448.98

   **EAC-utgift****Projekt** = IncurrusActualExpenseCost + NotIncoundsPlannedExpense\
   **EAC-utgift****Projekt** = $3 100.00 + $6 700.00\
   **EAC-utgift****Projekt** = $9 800.00

   **EAC****Project** = EAC Labor + EAC-kostnad\
   **EAC****Project**  = $22 448.98 + 9 800.00\
   **EAC****Project**  = $32 248.98
