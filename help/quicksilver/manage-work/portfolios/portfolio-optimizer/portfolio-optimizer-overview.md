---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio Optimizer - översikt
description: The [!UICONTROL Portfolio Optimizer] är det verktyg som används för projektutvärdering och -jämförelse. Processen för att granska och jämföra värden för affärsärenden för projekt som tilldelats en portfölj är hur en portföljförvaltare kan prioritera projekt och generera det bästa värdet för en organisation.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: fb1c7ade6622db391e0dac54f37603efe9dc0a58
workflow-type: tm+mt
source-wordcount: '1320'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] översikt

The [!UICONTROL Portfolio Optimizer] är det verktyg som används för projektutvärdering och -jämförelse. Gransknings- och jämförelseprocessen [!UICONTROL Business Case] Värdet för projekt som tilldelas en portfölj är hur en portföljförvaltare kan prioritera projekt och generera det mest värdet för en organisation.

![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Syftet med [!UICONTROL portfolio optimizer] ska tillhandahålla ett gränssnitt genom vilket en portföljförvaltare, styrkommitté eller produktledning kan se sammanfattande information om varje projekts affärsplan. Projekten kan sedan prioriteras enligt strategiska värden och mål, eller enligt deras övergripande poäng.

The [!UICONTROL Portfolio Optimizer] kan bara hjälpa dig om du har uppfyllt följande krav:

* The [!UICONTROL Business Cases] har slutförts i projekten. Mer information finns i artiklarna i [Definiera ett affärsärende: artikelindex](../../projects/define-a-business-case/define-business-case.md).
* En portfölj definieras i området Projektöversikt i avsnittet Projektinformation för de projekt som du vill granska.
* Du har angett projektbudget och planerad förmån för de projekt som du vill granska. Fast kostnad och Fast intäkt är valfria men tillför ytterligare värde. Mer information finns i [Projektfinansieringsfält](../../projects/project-finances/project-finances-overview-1.md).

Mer information om hur du hittar [!UICONTROL Portfolio Optimizer], se [Leta reda på [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanser i [!UICONTROL Portfolio Optimizer]

* [De finansiella områdena i [!UICONTROL Portfolio Optimizer]](#the-financial-areas-in-the-portfolio-optimizer)
* [De finansiella områdena i [!UICONTROL Portfolio Optimizer]](#the-financial-fields-in-the-portfolio-optimizer)

Du kan se portföljens ekonomiska status när som helst under projektens livstid när du använder [!UICONTROL Portfolio Optimizer].

Tänk på följande när du arbetar med ekonomi i [!UICONTROL Portfolio Optimizer]:

* Varje projekt får en poäng när deras [!UICONTROL Business Cases] fylls i enligt de kriterier som de matchar i [!UICONTROL Portfolio Optimizer]. Låga eller höga justeringsprojekt får till exempel högre poäng.

  Mer information om hur du beräknar portföljoptimeringspoängen för ett projekt finns i artikeln [Översikt över [!UICONTROL Portfolio Optimizer] Poäng](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* De ekonomiska beräkningarna för [!UICONTROL Portfolio Optimizer] använder [!UICONTROL Budgeted Cost] i [!UICONTROL Business Case] av projektet.
* Du kan prioritera projekt manuellt i [!UICONTROL Portfolio Optimizer], med beaktande av all information om dem. Detta omfattar till exempel ekonomiska data, anpassning till deras styrkort och avkastning.

### De finansiella områdena i [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Du kan visa ekonomisk information i följande områden i [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL Portfolio Header]**: I det här området visas ekonomisk information som samlats in från alla projekt i portföljen. Den visas på alla flikar i objektet Portfolio.
* **[!UICONTROL Portfolio Finances for Selected Projects]**: I det här området visas ekonomisk information som samlats in från de projekt som valts ut i [!UICONTROL Portfolio Optimizer]. Du kan lägga till eller ta bort projekt och förstå hur detta påverkar portföljens ekonomi genom att visa informationen i det här området.
* **[!UICONTROL Projects Finances]**: I det här området visas den ekonomiska informationen för varje projekt i [!UICONTROL Portfolio Optimizer].

### De finansiella områdena i [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Följande ekonomiska fält visas i [!UICONTROL Portfolio Optimizer]:

* [Portfolio header](#portfolio-header)
* [Portfolio finanser för utvalda projekt](#portfolio-finances-for-selected-projects)

#### Portfolio header {#portfolio-header}

![](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] beräknar de finansiella fälten i portföljrubriken med hjälp av information från projekt med status som bara motsvarar med [!UICONTROL Approved] eller [!UICONTROL Current].

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Fältets namn</strong> </th> 
   <th><strong>Beskrivning</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL On Time]</td> 
   <td> <p>Procentandel projekt i portföljen som anses vara [!UICONTROL On Time]. Det här är synligt från alla flikar i Portfolio.</p> <p>Ett projekt anses vara [!UICONTROL On Time] när projektet <strong>[!UICONTROL Condition]</strong> är <strong>[!UICONTROL On Target]</strong>. <br>Mer information om [!UICONTROL Project Conditions], se artikeln <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Översikt över projektvillkor och villkorstyp</a>.</p> <p>The <strong>[!UICONTROL On Time]</strong> procentandelen beräknas med hjälp av följande formel:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Antal [!UICONTROL On Time] Projekt/Totalt antal projekt i en [!UICONTROL Current] eller [!UICONTROL Approved] status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>Procentandel projekt i portföljen som anses vara [!UICONTROL On Budget]. Det här är synligt från alla flikar i en [!UICONTROL Portfolio].</p> <p>Projekt är <strong>[!UICONTROL On Budget]</strong> när de inte har överskridit sin fördefinierade budget. <br>Mer information om budgeten för ett projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Manage] Information inom projektfinansieringsområdet</a>.</p> <p>The [!UICONTROL On Budget] procentandelen beräknas med hjälp av följande formel:</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Antal [!UICONTROL On Budget] Projekt/totalt antal projekt </em><em>i en [!UICONTROL Current] eller [!UICONTROL Approved] status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>Räntabilitet (för portfölj)</td> 
   <td> <p>The [!UICONTROL Return on Investment] (avkastning) för portföljen beräknas med hänsyn tagen till den totala [!UICONTROL Benefit] i [!UICONTROL Portfolio] och summan av [!UICONTROL Budgeted Costs] av projekten. Det här är synligt från alla flikar i Portfolio.</p> <p>Portfolio ROI-värdet beräknas med följande formel:</p> <p><em>PORTFOLIO ROI = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Mer information om hur avkastningen beräknas för ett projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Beräkna räntabilitet</a> .</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] eller [!UICONTROL Alignment Score] </td> 
   <td> <p>Ett genomsnitt av alla [!UICONTROL Project Alignment Score] värden som beräknas när [!UICONTROL Scorecard] i [!UICONTROL Business Case] av projektet. Justeringspoängen för varje projekt listas i [!UICONTROL Alignment] kolumn i [!UICONTROL Portfolio Optimizer]. Detta visas från alla flikar i en portfölj.</p> <p>Mer information om hur du genererar justeringspoäng för ett projekt finns i artikeln <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Tillämpa ett styrkort på ett projekt och generera ett justeringsresultat</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>Summan av alla [!UICONTROL Net Values] av alla projekt i portföljen. Detta visas från alla flikar i en portfölj.</p> <p>Mer information om hur [!UICONTROL Net Value] beräknas för ett projekt, se artikeln <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Beräkna nettovärde</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio finanser för utvalda projekt {#portfolio-finances-for-selected-projects}

![](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Fältets namn</strong> </th> 
   <th> <p><strong>Beskrivning</strong> </p> <p> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>[!UICONTROL Number of projects]</td> 
   <td> <p>Det totala antalet aktiva projekt i portföljen. Projekt som betraktas som aktiva i en portfölj kan ha någon av följande statusvärden:</p> 
    <ul> 
     <li>[!UICONTROL Current]</li> 
     <li>[!UICONTROL Planning]</li> 
     <li>[!UICONTROL Approved]</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Budget]</td> 
   <td>Du kan uppdatera det här fältet manuellt för att ange den totala budgeten för hela portföljen. Den här budgeten används för alla projekt i portföljen. </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Remaining]</td> 
   <td> <p>Den återstående budgeten efter alla [!UICONTROL Budgeted Costs] för alla projekt i portföljen har dragits av från portföljens budget.</p> <p>The [!UICONTROL Remaining Portfolio Budget] beräknas med följande formel:</p> <p><em>[!UICONTROL Remaining Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - Totalt [!UICONTROL Budgeted Cost] av alla Portfolio-projekt</em> </p> <p>Det övergripande [!UICONTROL Budgeted Cost] av alla projekt i portföljen representeras i indikatorfältet i budgetfältet. </p> <p>Mer information om hur du spårar kostnader i ett projekt finns i artikeln<a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Cost]</td> 
   <td> <p>Summan av kostnaderna för alla projekt som visas i [!UICONTROL Portfolio Optimizer]. Kostnaden för varje projekt är densamma som [!UICONTROL Budgeted Cost] för projektet så som det visas i [!UICONTROL Business Case Summary]. </p> <p>Mer information om de finansiella områdena för projekt i [!UICONTROL Business Case], se avsnittet"Understanding Financial Fields in the Business Case" i artikeln <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Skapa ett affärsärende för ett projekt </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>Summan av alla [!UICONTROL Potential Risk Costs] av alla projekt i portföljen. The [!UICONTROL Potential Risk Cost] för varje projekt listas i [!UICONTROL Risk] kolumn i [!UICONTROL Portfolio Optimizer]. </p> <p>Mer information om att beräkna risker för projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Beräkna potentiella riskkostnader </a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>Summan av alla [!UICONTROL Planned Benefit] värden för alla projekt i portföljen. Det planerade förmånsvärdet för varje projekt listas i [!UICONTROL Benefit] kolumn i [!UICONTROL Portfolio Optimizer]. </p> <p>Mer information om [!UICONTROL Planned Benefit] för ett projekt, se artikeln <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Översikt över projektplanerad förmån</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk to Net Value] indikator</td> 
   <td> <p>Mäter [!UICONTROL Potential Risk] värdet med beaktande av [!UICONTROL Net Value] tillhandahålls av alla projekt i portföljen. För att uppnå maximal effektivitet i portföljen vill du se att [!UICONTROL Risk] indikatorn är låg och [!UICONTROL Net Value] indikatorn är hög. </p> <p>Mer information om beräkning av risk för [!UICONTROL Net Value], se artikeln <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Beräkna risk till nettovärde i en portfölj</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa [!UICONTROL Portfolio Optimizer]

Du kan bara anpassa projektlistområdet i [!UICONTROL Portfolio Optimizer] genom att använda inställningar för att ändra informationen i listan.

Följande ikoner och alternativ är tillgängliga för [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td>Ikon i Portfolio-optimering</td> 
   <td>Namn</td> 
   <td>Funktion</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Set project priority]</td> 
   <td>Använd den här ikonen när du vill spara projektordningen utifrån deras prioritet. </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-optimize-icon-in-optimizer.png"> </td> 
   <td>[!UICONTROL Optimize portfolio]</td> 
   <td>Använd den här ikonen för att optimera portföljen baserat på följande ekonomiska värden för projekten:
    <ul>
     <li>[!UICONTROL Cost]</li>
     <li>[!UICONTROL Alignment]</li>
     <li>[!UICONTROL Value]</li>
     <li>[!UICONTROL Risk to Benefit]</li>
     <li>[!UICONTROL ROI]</li>
    </ul><p>Mer information om hur du optimerar din portfölj finns i artikeln <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimera projekt i [!UICONTROL Portfolio Optimizer] </a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL Undo]/ [!UICONTROL Redo] ikoner</td> 
   <td>Använd de här ikonerna om du vill avbryta eller göra om ändringarna i [!UICONTROL Portfolio Optimizer] innan du sparar.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/ [!UICONTROL Hide unchecked] projekt</td> 
   <td>Använd de här ikonerna för att visa eller dölja projekt i portföljen som du inte har markerat.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Med den här ikonen exporterar du data i [!UICONTROL Project Prioritization] området på [!UICONTROL Portfolio Optimizer]. Du kan exportera den till följande format:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Avgränsad</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Med den här ikonen ändrar du de projektfält som visas i kolumnerna i [!UICONTROL Portfolio Optimizer]eller för att ändra vilka projekt du visar i [!UICONTROL Optimizer], baserat på deras status. </p> <p>Tips:  
     <ul> 
      <li> <p>Inte alla [!DNL Workfront] standardfält är tillgängliga att lägga till i kolumnerna. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Du kan bara lägga till anpassade fält som har ett annat värde än noll i något av projekten i portföljen.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
