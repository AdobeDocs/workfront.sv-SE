---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna index för kostnadsprestanda (CPI)
description: Kostnadsprestandaindexet (CPI) beskriver förhållandet på projekt- eller aktivitetsnivå mellan den planerade kostnaden och den faktiska kostnaden. Projektledare granskar den här mätningen för att identifiera aktiviteter eller projekt som för närvarande spåras under- eller överkostnadsbaserat vid en viss tidpunkt.
author: Lisa
feature: Work Management
exl-id: 7f2efe26-7292-482d-986c-2d2077a7ca52
source-git-commit: 23a4d055871c9138818e70fa1cd936581dbd7552
workflow-type: tm+mt
source-wordcount: '583'
ht-degree: 0%

---

# Beräkna index för kostnadsprestanda (CPI)

<!-- Audited: 5/2025 -->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link.)</p>
-->

Kostnadsprestandaindexet (CPI) beskriver förhållandet på projekt- eller aktivitetsnivå mellan den planerade kostnaden och den faktiska kostnaden. Projektledare granskar den här mätningen för att identifiera aktiviteter eller projekt som för närvarande spåras under- eller överkostnadsbaserat vid en viss tidpunkt. Kostnaden kan mätas i timmar eller dollar, beroende på din PIM-metod (Performance Index Method). Mer information om hur du ställer in prestandaindexmetoden finns i [Ange prestandaindexmetod (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

Endast organisationer som kräver tidsregistrering kan använda CPI. Dessutom är kostnadsbaserade PIM-värden endast korrekta i organisationer som har definierat kostnadsnivåer för uppgiftstilldelningar (jobbroller eller användare).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Adobe Workfront package</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td>Adobe Workfront-licens</td> 
   <td>
   <p>Ljus eller högre</p>
   <p>Granska eller högre</p></td>  
  </tr> 
  <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td>Visa åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td>Objektbehörigheter</td> 
   <td>Visa eller högre behörigheter för projektet med behörighet att visa ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över kostnadsprestandaindex (CPI)

### CPI-värdet {#the-cpi-value}

Projektledare är införstådda med att ett CPI-värde på 1 innebär att projektet är exakt budgeterat. Värden större än 1 visar att ett projekt ligger under budget (färre timmar eller utgifter har bokförts än vad som ursprungligen planerats), och värden mindre än 1 innebär att ett projekt ligger över budget (fler timmar eller utgifter har bokförts än vad som ursprungligen planerats). Ju längre bort från 1, desto större avvikelse från planen.

| **CPI-värde** | **Indikation för budget** |
|---|---|
| 1 | I plan eller budget |
| > 1 (större än 1) | Under budget |
| &lt; 1 (mindre än 1) | Över budget |


### Hur CPI beräknas {#how-cpi-is-calculated}

I Adobe Workfront beror beräkningen för CPI på vilken prestandaindexmetod som valts för projektet. Mer information om hur du ställer in prestandaindexmetoden finns i [Ange prestandaindexmetod (PIM)](../../../manage-work/projects/project-finances/set-pim.md).

* [CPI-beräkningar vid användning av timbaserad PIM](#cpi-calculations-when-using-hour-based-pim)
* [CPI-beräkningar vid användning av kostnadsbaserad PIM](#cpi-calculations-when-using-cost-based-pim)

#### CPI-beräkningar vid användning av timbaserad PIM {#cpi-calculations-when-using-hour-based-pim}

If

```
Actual Hours > 0 THEN CPI = Total Budgeted Cost Work Performed / Actual Hours
```

Annars

```
CPI = 1
```

* **För en icke-överordnad aktivitet:**

  ```
  Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete / 100)
  ```

* **För en överordnad aktivitet:**
Totalt utfört budgeterat kostnadsarbete = summan av fältet Totalt budgeterat kostnadsarbete utfört för alla direkta underordnade aktiviteter.

* **För ett projekt:**
Totalt utfört budgeterat kostnadsarbete = summan av fältet Totalt budgeterat kostnadsarbete utfört för alla aktiviteter på den översta nivån (överordnade och fristående aktiviteter).

Mer information om totalt budgeterat kostnadsarbete som utförts (BCWP) finns i [Beräkna budgeterat kostnadsarbete som utförts (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

#### CPI-beräkningar vid användning av kostnadsbaserad PIM {#cpi-calculations-when-using-cost-based-pim}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>CPI = (Planned Cost of Work Performed + Planned Cost of Incurred Expenses) / (Total Actual Cost + Actual Cost of Incurred Expenses) </code> </p>
-->

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>NOTE: this used to be here before - above - but Anna sent me the one below. I kept the other one, although she is still researching its validity - see this issue: https://hub.workfront.com/issue/5fc7b1cf00012aeebf9e822db8ea2513/overview)</code> </p>
-->

If

```
Actual Labor Cost + Incurred Actual Expense Cost <> 0 THEN CPI = (Total Budgeted Cost Work Performed + Incurred Planned Expense Cost) / (Actual Labor Cost + Incurred Actual Expense Cost)
```



Annars

```
CPI = 1
```

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode"><code>(NOTE: above: this used to say: CPI = CPI Labor, but Anna had me fix it on July 21, 2021)</code> </p>
-->

Fälten i den här beräkningen beskrivs nedan:

```
Total Actual Cost = Actual (logged) Hours * Hourly Rate of assignees
```

```
Incurred Actual Expense Cost = Actual Cost
```

Uppkomna utgifter är den utgift för vilken faktisk kostnad > 0

```
Planned Cost of Incurred Expenses = Total of Planned Cost of all incurred expenses
```



<!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Old calculation - taken out by Lilit and replaced below: Planned Cost of Work Performed= (planned labor cost) * (percent complete) / 100 where planned labor cost is the planned hours allocated to assignees * their rates.)</p>
  -->

* Planerad kostnad för utfört arbete beräknas enligt följande formel:

  ```
  Planned Cost of Work Performed = Planned cost * Percent Complete / 100
  ```

Totalt budgeterat kostnadsarbete som utförts beräknas för följande:

* **För en icke-överordnad aktivitet:**

  ```
  Total Budgeted Cost Work Performed = Planned Labor Cost * Percent Complete / 100
  ```

* **För en överordnad aktivitet:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field from all direct child tasks)
  ```

* **För ett projekt:**

  ```
  Total Budgeted Cost Work Performed = SUM(Total Budgeted Cost Work Performed field for all top-level tasks)
  ```



## Hitta CPI i ett projekt eller en uppgift

Du kan visa CPI för ett projekt eller en uppgift i ett projekt, en uppgiftslista eller en rapport. Dessutom kan du visa den på projekt- eller aktivitetsnivå.

1. Gå till det projekt eller den uppgift där du vill visa CPI:n.
1. Expandera **Projektinformation** eller **Aktivitetsinformation** i den vänstra panelen, beroende på om du visar CPI för ett projekt eller en uppgift.

1. Klicka på **Ekonomi**. Processorn visas i fältet **CPI/SPI/CSI**.

   ![CPI i projekt](assets/cpi-on-project-nwe.png)
