---
content-type: overview;how-to-procedural
product-area: projects
navigation-topic: financials
title: Beräkna uppskattning vid slutförande
description: Uppskattningen vid slutförande (Estiate at Completion, EAC) är en prestandamätning som representerar den beräknade totala kostnaden för ditt projekt eller din uppgift när den är klar.
author: Lisa
feature: Work Management
exl-id: 9061fa56-cff3-4fe2-866e-1fdda9d43efc
source-git-commit: b983a780198743a2b87b4b48cf4d6afdf1cee437
workflow-type: tm+mt
source-wordcount: '848'
ht-degree: 0%

---

# Beräkna uppskattning vid slutförande

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Linked to the product. Do not change link!) </p>
-->

Uppskattningen vid slutförande (Estiate at Completion, EAC) är en prestandamätning som representerar den beräknade totala kostnaden för ditt projekt eller din uppgift när den är klar.

Med den här inställningen kan du definiera hur EAC-värdet ska beräknas. 

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens</td> 
   <td>
   <p>Nytt: Ljus eller högre</p>
   <p>eller</p>
   <p>Aktuell: Granska eller senare</p></td>  
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td>Visa åtkomst till projekt och finansiella data</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td>Visa eller högre behörigheter för projektet med behörighet att visa ekonomi</td> 
  </tr> 
 </tbody> 
</table>

Mer information om informationen i den här tabellen finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Definiera hur EAC ska beräknas

Som en del av projektsysteminställningarna kan Adobe Workfront-administratören definiera hur EAC ska beräknas. EAC kan beräknas på något av följande två sätt:

* [Beräkna på projektnivå](#calculate-at-the-project-level)
* [Samla in uppgifter och underuppgifter](#roll-up-from-tasks-and-subtasks)

Mer information om hur du ställer in projektinställningar i Workfront, inklusive hur du beräknar offerten vid slutförande, finns i [Konfigurera systemomfattande projektinställningar](../../../administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

Som projektledare kan du även ändra den här inställningen på projektnivå på underfliken Ekonomi i projektet. Mer information om hur du redigerar underfliken Ekonomi i ett projekt finns i [Hantera information i projektfinansieringsdelen](../../../manage-work/projects/project-finances/manage-project-finance-area.md).

### Beräkna på projektnivå {#calculate-at-the-project-level}

EAC för den överordnade uppgiften och projektet bestäms genom att de faktiska timmarna/den faktiska arbetskostnaden anges i EAC-formlerna. Beräkningen inkluderar Faktiska timmar/kostnader och utgifter som lagts till direkt i den överordnade uppgiften eller projektet.

### Samla in uppgifter och underuppgifter {#roll-up-from-tasks-and-subtasks}

EAC för den överordnade uppgiften och projektet bestäms genom att sammanfatta EAC för varje underordnad uppgift. Den här beräkningen exkluderar faktiska timmar/kostnader och utgifter som läggs till direkt i den överordnade aktiviteten eller projektet.

## Beräkna EAC utifrån prestandaindexmetoden (PIM)

I Workfront beror beräkningen för EAC på projektets valda PIM-metod (Performance Index Method). Mer information om hur du anger PIM för ditt system eller för ditt projekt finns i [Ange PIM (Performance Index Method)](../../../manage-work/projects/project-finances/set-pim.md).

* [Beräkna EAC med timbaserad PIM](#calculate-eac-using-hour-based-pim)
* [Beräkna EAC med kostnadsbaserad PIM](#calculate-eac-using-cost-based-pim)

### Beräkna EAC med timbaserad PIM {#calculate-eac-using-hour-based-pim}

```
EAC = Total Planned Hours / CPI*
```

&#42;Om kostnadsprestandaindex [Beräkna kostnadsprestandaindex (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md) = 0, EAC = totalt antal planerade timmar + faktiska timmar. Detta inträffar när timmar har hämtats, men projektet/aktiviteten är slutförd till 0 %.

Mer information om hur du beräknar CPI finns i [Beräkna kostnadsprestandaindex (CPI)](../../../manage-work/projects/project-finances/calculate-cpi.md).

### Beräkna EAC med kostnadsbaserad PIM {#calculate-eac-using-cost-based-pim}

EAC för ett projekt beräknas med följande formel:

```
EAC = EAC Labor + EAC Expense 
```

<pre>EAC Labor =  <em>OM</em> CPI-arbete &lt;&gt; 0 THEN EAC-arbete = Planerad arbetskostnad/CPI-arbete</pre><pre><em>ELSE</em> EAC  Arbete = Planerad arbetskostnad + faktisk arbetskostnad</pre><pre>CPI-arbete = OM Faktisk arbetskostnad &lt;&gt; 0 THAN CPI-arbete = TotalBudgetedCostWorkPerformed / Faktisk arbetskostnad</pre><pre>ELSE CPI Labor = 1 </pre>Följande fält beaktas vid beräkning av EAC:

* Totalt utfört budgeterat kostnadsarbete (BCWP) = resultatet av multiplicering av den budgeterade kostnaden för det planerade arbetet (budgeterad kostnad) och den procentandel av uppgiften som har slutförts hittills.

  Mer information om totalt budgeterat kostnadsarbete som utförts (BCWP) finns i [Beräkna budgeterat kostnadsarbete som utförts (BCWP)](../../../manage-work/projects/project-finances/calculate-bcwp.md).

   * **För en icke-överordnad aktivitet:**

     ```
     Total Budgeted Cost Work Performed = Planned Hours * (Percent Complete/100)
     ```

   * **För en överordnad aktivitet:**
Totalt utfört budgeterat kostnadsarbete = summan av fältet Totalt budgeterat kostnadsarbete utfört för alla direkta underordnade aktiviteter.

   * **För ett projekt:**
Totalt utfört budgeterat kostnadsarbete = summan av fältet Totalt budgeterat kostnadsarbete utfört för alla aktiviteter på den översta nivån (överordnade och fristående aktiviteter). 

* EAC-utgift = resultatet av att addera den faktiska kostnaden för upplupen kostnad till den ej uppkomna planerade kostnaden. Den beräknas med följande formel:

  ```
  EAC Expense = Incurred Actual Expense Cost + Not Incurred Planned Expense
  ```

   * Faktisk utgiftskostnad = Summan av fältet Planerat belopp för alla utgifter där fältet Faktiskt belopp > 0. Om du t.ex. skapar en utgift för Uppgift 1 och anger $500.00 i fältet Planerat belopp och ett belopp > 0 i fältet Faktiskt belopp (t.ex. $600.00), är den förväntade kostnaden för den här uppgiften $500.00.
   * Ej upplupen planerad utgift = Summan av fältet Planerat belopp för alla utgifter där fältet Faktiskt belopp = 0. Om du till exempel skapar två utgifter för Uppgift 1 där värdet i fältet Planerat belopp för den första utgiften är 500,00 USD och värdet i fältet Faktiskt belopp är 600,00 USD och för den andra utgiften, är värdet i fältet Planerat belopp 300,00 USD och värdet i fältet Faktiskt belopp är 0,00 USD. Ej fakturerad kostnad för den här aktiviteten är 300,00 USD. 

## Hitta EAC i ett projekt eller en uppgift

1. Gå till det projekt eller den uppgift där du vill visa EAC.
1. Expandera **Projektinformation** eller **Aktivitetsinformation** i den vänstra panelen av projektet eller aktiviteten, beroende på var du visar EAC.

1. Klicka på **Ekonomi**. 

   EAC-värdet visas i fältet **Uppskattning vid slutförande**.

   ![EAC i projekt](assets/eac-highlighted-on-project-350x112.png)
