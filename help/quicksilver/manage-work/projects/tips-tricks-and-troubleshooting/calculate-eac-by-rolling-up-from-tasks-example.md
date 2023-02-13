---
content-type: tips-tricks-troubleshooting
product-area: projects
navigation-topic: tips-tricks-and-troubleshooting-projects
title: Beräkningsexempel - Beräkna EAC som en sammanslagning av uppgifter
description: PIM = timbaserad
author: Alina
feature: Work Management
exl-id: 68b582c9-f72a-4000-9d28-f7dafa23541f
source-git-commit: a849ecaf6097dcdc924aaab2867f37bf57d5bc09
workflow-type: tm+mt
source-wordcount: '873'
ht-degree: 4%

---

# Beräkningsexempel - Beräkna EAC som en sammanslagning av uppgifter

## EAC-metod: samla in uppgifter eller underuppgifter

* [PIM= Timbaserad](#pim-hour-based)
* [PIM= Kostnadsbaserad](#pim-cost-based)

### PIM= Timbaserad {#pim-hour-based}

* [Enkelt exempel: projektet saknar underordnade uppgifter](#simple-example-project-has-no-children-tasks)
* [Komplicerat exempel: projektet har underordnade uppgifter](#complicated-example-project-has-children-tasks)

#### Enkelt exempel: projektet saknar underordnade uppgifter {#simple-example-project-has-no-children-tasks}

PIM = timbaserad

EAC-metod = Samla in uppgifter/underaktiviteter

1. Skapa projekt A med tre uppgifter (inga underordnade uppgifter) som alla är tilldelade till Användare 1 vars kostnad/timme är 100,00 USD.
1. Lägg till planerade/faktiska timmar för varje uppgift och % slutfört enligt tabellen nedan:

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
   <td> <p>5 timmar</p> </td> 
   <td> <p>25 tim</p> </td> 
   <td> <p>20%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 2</p> </td> 
   <td> <p>10 tim</p> </td> 
   <td> <p>25 tim</p> </td> 
   <td> <p>30%</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Aktivitet 3</p> </td> 
   <td> <p>15 tim</p> </td> 
   <td> <p>25 tim</p> </td> 
   <td> <p>40%</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Beräkna om ekonomi
1. **CPI för aktivitet 1** = 0,04 beräknat enligt följande:\
   **CPI för aktivitet 1** = *IF* Faktiska timmar > 0 *SEDAN* CPI = TotalBudgetedCostWorkPerformed/Actual Hours\
       *ELSE* CPI = 1\
   **CPI för aktivitet 1** = 1 / 25\
   **CPI för aktivitet 1** = .04

1. **EAC för uppgift 1** = 125 tim beräknat enligt följande:\
   **EAC för uppgift 1** = *IF* CPI &lt;> 0 *SEDAN* EAC = Planerade timmar/CPI\
       *ELSE*

   ```
   EAC = Planned  Hours + Actual  Hours
   ```

   **EAC för uppgift 1** = 5 / .04\
   **EAC för uppgift 1** = 125 tim

1. CPI/EAC för uppgifter 2 och 3 är:\
   Aktivitet 2 = 0,12 / 83,33 tim\
   Aktivitet 3 = 0,24 / 62,5 tim

1. **CPI för projekt** = 0,13 beräknat enligt följande:\
   **CPI för projekt** = *IF* Faktiska timmar > 0 *SEDAN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI för projekt** = 10 / 75\
   **CPI för projekt** = .13

1. **EAC för projekt** = 270,83 tim beräknat enligt följande\
   **EAC för projekt** = EAC-uppgift 1 + EAC-uppgift 2 + EAC-uppgift 3\
   **EAC för projekt** = 125 + 83.33 + 62.5\
   **EAC för projekt** = 270,83 tim

#### Komplicerat exempel: projektet har underordnade uppgifter {#complicated-example-project-has-children-tasks}

PIM = timbaserad

EAC-metod = Samla in uppgifter/underaktiviteter

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

1. Lägg till 50 timmar direkt i projektet (Mer > Timmar > Loggtimmar) så att 5 000,00 USD av den faktiska arbetskostnaden registreras direkt i projektet.
1. Kör omberäkning av ekonomi
1. **CPI för aktivitet 2** = .1 beräknad enligt följande:\
   **CPI för aktivitet 2** = *IF* Faktiska timmar > 0 *SEDAN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI för aktivitet 2** = 1 / 10\
   **CPI för aktivitet 2** = .1

1. **EAC för uppgift 2** = 50 tim beräknat enligt följande:\
   **EAC för uppgift 2** = *IF* CPI &lt;> 0 *SEDAN*

   ```
   EAC = Planned Hours / CPI
   ```

       *ELSE* EAC = Planerade timmar + faktiska timmar\
   **EAC för uppgift 2** = 5 / .1\
   **EAC för uppgift 2** = 50 tim

1. CPI/EAC för uppgift 4, Aktivitet 5 och Aktivitet 6:\
   Aktivitet 4 = 0,4 / 25 tim\
   Aktivitet 5 = 0,75 / 20 tim\
   Aktivitet 6 = 1.2 / 16,67 tim

1. **CPI för aktivitet 3** = 0,38\
   **CPI för aktivitet 3** = *IF* Faktiska timmar > 0 *SEDAN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI för aktivitet 3** = 11.5 / 30\
   **CPI för aktivitet 3** = 0,38

1. **EAC för uppgift 3** = EAC-uppgift 4 + EAC-uppgift 5\
   **EAC för uppgift 3** = 25 + 20\
   **EAC för uppgift 3** = 45 tim

1. **CPI för aktivitet 1** = 0,25 beräknat enligt följande:\
   **CPI för aktivitet 1** = *IF* Faktiska timmar > 0 *SEDAN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI för aktivitet 1** = 12.5 / 50\
   **CPI för aktivitet 1** = 0,25

1. **EAC för uppgift 1** = EAC-uppgift 2 + EAC-uppgift 3\
   **EAC för uppgift 1** = 50 + 45\
   **EAC för uppgift 1** = 95 tim

1. CPI för projekt = 0,22 beräknat enligt följande:\
   **CPI för projekt** = *IF* Faktiska timmar > 0 *SEDAN*

   ```
   CPI = TotalBudgetedCostWorkPerformed/Actual Hours
   ```

       *ELSE* CPI = 1\
   **CPI för projekt** = 24.5 / 110\
   **CPI för projekt** = .22272\
   **CPI för projekt** = .22

1. **EAC för projekt** = EAC-uppgift 1 + EAC-uppgift 6\
   **EAC för projekt** = 95 + 16,67\
   **EAC för projekt** = 111,67 tim

### PIM= Kostnadsbaserad {#pim-cost-based}

* [Enkelt exempel: projektet saknar underordnade uppgifter](#simple-example-project-has-no-children-tasks)

#### Enkelt exempel: projektet saknar underordnade uppgifter {#simple-example-project-has-no-children-tasks-1}

PIM = kostnadsbaserad

EAC-metod = Samla in uppgifter/underaktiviteter

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
   <td> <p>$2,700.00</p> </td> 
  </tr> 
 </tbody> 
</table>

1. Kör Beräkna om ekonomi från projektåtgärder
1. **CPI****för uppgift 1** = 0,14 beräknat enligt följande:\
   **CPI****för uppgift 1**  = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost) / (ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****för uppgift 1**  = (100+300) / (2500+400)\
   **CPI****för uppgift 1**  = 400 / 2900\
   **CPI****för uppgift 1**  = .14

1. **EAC****för uppgift 1** = $13 400.00\
   **CPI-arbete****för aktivitet 1** = OM Faktisk arbetskostnad &lt;> 0 SEDAN

   ```
   CPI_Labor = TotalBudgetedCostWorkPerformed / Actual Labor Cost
   ```

      ELSE CPI_Labor = 1\
   **CPI-arbete****för aktivitet 1** = 100/2500\
   **CPI-arbete****för aktivitet 1** = .04

   **EAC Labor****för aktivitet 1** = *IF* CPI_Labor &lt;> 0 *SEDAN*

   ```
   EAC Labor = Planned Labor Cost / CPI_Labor
   ```

   *   ELSE* EAC-arbetskostnad = Planerad arbetskostnad + faktisk arbetskostnad\
   **EAC Labor****för aktivitet 1** = 500.00/.04\
   **EAC Labor****för aktivitet 1** = $12 500.00

   **EAC-utgift****för aktivitet 1** = IncurrusActualExpenseCost + NotIncoundsPlannedExpense\
   **EAC-utgift****för aktivitet 1** = $400.00 + $500.00\
   **EAC-utgift****för aktivitet 1** = $900.00

   **EAC****för uppgift 1** = EAC Labor + EAC-kostnad\
   **EAC****för uppgift 1**  = $12 500.00 + $900.00\
   **EAC****för uppgift 1**  = $13 400.00

1. Här är CPI-/EAC-värdena för Aktivitet 2 och Aktivitet 3:\
   Aktivitet 2 = 0,19 / $8,433.33\
   Aktivitet 3 = 0,44 / SEK 6 950,00***

1. Projektets CPI = 0,32\
   **CPI****för projekt** = *IF* Faktisk arbetskostnad + IncisiveActualExpenseCost &lt;> 0 *SEDAN*

   ```
   CPI = (TotalBudgetedCostWorkPerformed + IncurredPlannedExpenseCost)/(ActualLaborCost + IncurredActualExpenseCost)
   ```

   *   ELSE* CPI = CPI_Labor\
   **CPI****för projekt** = (1000 + 2300) / (7500 + 2700)\
   **CPI****för projekt** = 3300 / 10200\
   **CPI****för projekt** = .32

1. EAC för projektet är 28 783,33 USD\
   **EAC****för projekt** = EAC-uppgift 1 + EAC-uppgift 2 + EAC-uppgift 3\
   **EAC****för projekt** = $13 400.00 + $8 433.33 + $6 950.00\
   **EAC****för projekt** = $28,783.33
