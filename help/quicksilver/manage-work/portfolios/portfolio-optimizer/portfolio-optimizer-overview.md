---
content-type: overview
product-area: portfolios
navigation-topic: portfolio-optimizer
title: Portfolio Optimizer - översikt
description: '[!UICONTROL Portfolio Optimizer] är det verktyg som används för projektutvärdering och jämförelse. Processen för att granska och jämföra värden för affärsärenden för projekt som tilldelats en portfölj är hur en portföljförvaltare kan prioritera projekt och generera det bästa värdet för en organisation.'
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1e48a24c-65de-49c2-85a8-dc931ac40c52
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '1333'
ht-degree: 0%

---

# [!UICONTROL Portfolio Optimizer] - översikt

<!-- Audited: 01/2024 -->

[!UICONTROL Portfolio Optimizer] är det verktyg som används för projektutvärdering och jämförelse. Gransknings- och jämförelseprocessen för [!UICONTROL Business Case]-värden för projekt som tilldelats en portfölj är hur en portföljförvaltare kan prioritera projekt och generera det högsta värdet för en organisation.

![Portfolio-optimering med projekt](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

Syftet med [!UICONTROL portfolio optimizer] är att tillhandahålla ett gränssnitt genom vilket en portföljförvaltare, styrkommitté eller produktledning kan visa sammanfattande information om varje projekts affärsmodell. Projekten kan sedan prioriteras enligt strategiska värden och mål, eller enligt deras övergripande poäng.

[!UICONTROL Portfolio Optimizer] kan bara hjälpa dig om du har uppfyllt följande krav:

* [!UICONTROL Business Cases] har slutförts i projekten. Mer information finns i artiklarna i [Definiera ett affärsärende: artikelindex](../../projects/define-a-business-case/define-business-case.md).
* En portfölj definieras i området Projektöversikt i avsnittet Projektinformation för de projekt som du vill granska.
* Du har angett projektbudget och planerad förmån för de projekt som du vill granska. Fast kostnad och Fast intäkt är valfria men tillför ytterligare värde. Mer information finns i [Projektfinansieringsfält](../../projects/project-finances/project-finances-overview-1.md).

Mer information om hur du hittar [!UICONTROL Portfolio Optimizer] finns i [Leta reda på [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/locate-portfolio-optimizer.md).

## Finanser i [!UICONTROL Portfolio Optimizer]

Du kan se portföljens ekonomiska status när som helst under projektens livstid när du använder [!UICONTROL Portfolio Optimizer].

Tänk på följande när du arbetar med ekonomi i [!UICONTROL Portfolio Optimizer]:

* Alla projekt får ett poängvärde när deras [!UICONTROL Business Cases] slutförs enligt vilka kriterier de matchar i [!UICONTROL Portfolio Optimizer]. Låga eller höga justeringsprojekt får till exempel högre poäng.

  Mer information om hur du beräknar portföljoptimeringspoängen för ett projekt finns i [Översikt över [!UICONTROL Portfolio Optimizer] bakgrundsmusiken ](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

* De ekonomiska beräkningarna för [!UICONTROL Portfolio Optimizer] använder [!UICONTROL Budgeted Cost] i [!UICONTROL Business Case] för projektet.
* Du kan prioritera dina projekt i [!UICONTROL Portfolio Optimizer] manuellt, med hänsyn tagen till all information om dem. Detta inkluderar till exempel ekonomiska data, anpassning till deras styrkort och avkastning.

### De ekonomiska områdena i [!UICONTROL Portfolio Optimizer] {#the-financial-areas-in-the-portfolio-optimizer}

Du kan visa ekonomisk information i följande områden av [!UICONTROL Portfolio Optimizer]:

* **[!UICONTROL Portfolio Header]**: I det här området visas ekonomisk information som samlats in från alla projekt i portföljen. Den visas på alla flikar i Portfolio-objektet.
* **[!UICONTROL Portfolio Finances for Selected Projects]**: I det här området visas ekonomisk information som samlats in från de projekt som har valts i [!UICONTROL Portfolio Optimizer]. Du kan lägga till eller ta bort projekt och förstå hur detta påverkar portföljens ekonomi genom att visa informationen i det här området.
* **[!UICONTROL Projects Finances]**: I det här området visas den ekonomiska informationen för varje projekt i [!UICONTROL Portfolio Optimizer].

### De ekonomiska fälten i [!UICONTROL Portfolio Optimizer] {#the-financial-fields-in-the-portfolio-optimizer}

Följande ekonomiska fält visas i [!UICONTROL Portfolio Optimizer]:

* [Portfolio header](#portfolio-header)
* [Portfolio finanser för utvalda projekt](#portfolio-finances-for-selected-projects)

#### Portfolio header {#portfolio-header}

![Portfolio header](assets/portfolio-header-nwe-350x14.png)

[!DNL Adobe Workfront] beräknar de ekonomiska fälten i portföljrubriken med hjälp av information från projekt med statusvärden som bara motsvarar [!UICONTROL Approved] eller [!UICONTROL Current].

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
   <td> <p>Procentandelen projekt i portföljen som betraktas som [!UICONTROL On Time]. Detta visas från alla flikar i en portfölj.</p> <p>Ett projekt anses vara [!UICONTROL On Time] när projektet <strong>[!UICONTROL Condition]</strong> är <strong>[!UICONTROL On Target]</strong>. <br>Mer information om [!UICONTROL Project Conditions] finns i artikeln <a href="../../../manage-work/projects/manage-projects/project-condition-and-condition-type.md" class="MCXref xref">Översikt över projektvillkor och villkorstyp</a>.</p> <p>Procentandelen <strong>[!UICONTROL On Time]</strong> beräknas med följande formel:</p> <p><em>[!UICONTROL On Time Portfolio Percentage] = Antal [!UICONTROL On Time] projekt/totalt antal projekt i en [!UICONTROL Current] eller [!UICONTROL Approved] status </em> </p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL On Budget]</td> 
   <td> <p>Procentandelen projekt i portföljen som betraktas som [!UICONTROL On Budget]. Detta visas från alla flikar i en [!UICONTROL portfolio].</p> <p>Projekt är <strong>[!UICONTROL On Budget]</strong> när de inte har överskridit sin fördefinierade budget. <br>Mer information om budgeten för ett projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/manage-project-finance-area.md" class="MCXref xref">[!UICONTROL Manage] information i projektfinansieringsdelen </a>.</p> <p>Procentandelen [!UICONTROL On Budget] beräknas med följande formel:</p> <p><em>[!UICONTROL On Budget Portfolio Percentage] = Antal [!UICONTROL On Budget] projekt/totalt antal projekt </em><em> i en [!UICONTROL Current] eller [!UICONTROL Approved] status</em> </p> </td> 
  </tr> 
  <tr> 
   <td>Räntabilitet (för portfölj)</td> 
   <td> <p>[!UICONTROL Return on Investment] (ROI) för portföljen beräknas genom att ta hänsyn till totalt [!UICONTROL Benefit] för [!UICONTROL Portfolio] och totalt [!UICONTROL Budgeted Costs] för projekten. Detta visas från alla flikar i en portfölj.</p> <p>Portfolio avkastningsvärde beräknas med följande formel:</p> <p><em>Portfolio ROI = ([!UICONTROL Total Benefit] - [!UICONTROL Total Budgeted Cost])/ [!UICONTROL Total Cost] * 100</em> </p> <p>Mer information om hur avkastningen beräknas för ett projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/calculate-roi.md" class="MCXref xref">Beräkna avkastning på investering (ROI)</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Aligned] eller [!UICONTROL Alignment Score] </td> 
   <td> <p>Ett genomsnitt av alla [!UICONTROL Project Alignment Score]-värden, som beräknas efter att [!UICONTROL Scorecard] har slutförts i [!UICONTROL Business Case] för projektet. Justeringspoängen för varje projekt listas i kolumnen [!UICONTROL Alignment] i [!UICONTROL Portfolio Optimizer]. Detta visas från alla flikar i en portfölj.</p> <p>Mer information om hur du genererar justeringspoäng för ett projekt finns i artikeln <a href="../../../manage-work/projects/define-a-business-case/apply-scorecard-to-project-to-generate-alignment-score.md" class="MCXref xref">Använda ett styrkort för ett projekt och generera ett justeringspoäng</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Net Value]</td> 
   <td> <p>Summan av alla [!UICONTROL Net Values] av alla projekt i portföljen. Detta visas från alla flikar i en portfölj.</p> <p>Mer information om hur [!UICONTROL Net Value] beräknas för ett projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Beräkna nettovärde</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

#### Portfolio finanser för utvalda projekt {#portfolio-finances-for-selected-projects}

![Portfolio finanser](assets/portfolio-finances-for-selected-projects-in-optimizer-nwe-350x29.png)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Fältets namn</strong> </th> 
   <th><strong>Beskrivning</strong></th> 
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
   <td> <p>Den återstående budgeten efter alla [!UICONTROL Budgeted Costs] för alla projekt i portföljen har dragits av från portföljens budget.</p> <p>[!UICONTROL Remaining Portfolio Budget] beräknas med följande formel:</p> <p><em>[!UICONTROL Remaining Portfolio Budget] = [!UICONTROL Total Portfolio Budget] - Totalt [!UICONTROL Budgeted Cost] för alla Portfolio-projekt </em> </p> <p>Den totala [!UICONTROL Budgeted Cost] för alla projekt i portföljen visas i indikatorfältet i budgetfältet. </p> <p>Mer information om hur du spårar kostnader för ett projekt finns i <a href="../../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Total Cost]</td> 
   <td> <p>Summan av kostnaderna för alla projekt som visas i [!UICONTROL Portfolio Optimizer]. Kostnaden för varje projekt är densamma som för [!UICONTROL Budgeted Cost] i projektet som det visas i [!UICONTROL Business Case Summary]. </p> <p>Mer information om de finansiella fälten i projekt i [!UICONTROL Business Case] finns i avsnittet"Understanding Financial Fields in the Business Case" i artikeln <a href="../../../manage-work/projects/define-a-business-case/create-business-case.md" class="MCXref xref">Create a Business Case for a project</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk] </td> 
   <td> <p>Summan av alla [!UICONTROL Potential Risk Costs] av alla projekt i portföljen. [!UICONTROL Potential Risk Cost] för varje projekt visas i kolumnen [!UICONTROL Risk] i [!UICONTROL Portfolio Optimizer]. </p> <p>Mer information om hur du beräknar risker för projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/potential-risk-cost.md" class="MCXref xref">Beräkna potentiella riskkostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Benefit]</td> 
   <td> <p>Summan av alla [!UICONTROL Planned Benefit]-värden för alla projekt i portföljen. Det planerade förmånsvärdet för varje projekt listas i kolumnen [!UICONTROL Benefit] i [!UICONTROL Portfolio Optimizer]. </p> <p>Mer information om [!UICONTROL Planned Benefit] för ett projekt finns i artikeln <a href="../../../manage-work/projects/project-finances/project-planned-benefit.md" class="MCXref xref">Översikt över projektplanerad förmån</a>.</p> </td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Risk to Net Value] indikator</td> 
   <td> <p>Mäter värdet [!UICONTROL Potential Risk], med beaktande av [!UICONTROL Net Value] som tillhandahålls av alla projekt i portföljen. För att uppnå maximal effektivitet i portföljen vill du se att indikatorn [!UICONTROL Risk] är låg och att indikatorn [!UICONTROL Net Value] är hög. </p> <p>Mer information om hur du beräknar risk för [!UICONTROL Net Value] finns i artikeln <a href="../../../manage-work/portfolios/portfolio-optimizer/calculate-risk-to-net-value-in-portfolio.md" class="MCXref xref">Beräkna risk till nettovärde i en portfölj</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Anpassa [!UICONTROL Portfolio Optimizer]

Du kan bara anpassa projektlistområdet för [!UICONTROL Portfolio Optimizer] genom att använda inställningar för att ändra informationen i listan.

Följande ikoner och alternativ är tillgängliga för [!UICONTROL Portfolio Optimizer]:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><strong>Ikon i Portfolio Optimizer</strong></td> 
   <td><strong>Namn</strong></td> 
   <td><strong>Funktion</strong></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-set-priority-icon.png"> </td> 
   <td>[!UICONTROL Set project priority]</td> 
   <td><p>Använd den här ikonen när du vill spara projektordningen utifrån deras prioritet.</p>
   <p>Du måste ha behörigheten Hantera för alla projekt i listan för att kunna använda <b>Ange projektprioritet</b></p>.
    </td> 
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
    </ul><p>Mer information om hur du optimerar din portfölj finns i artikeln <a href="../../../manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md" class="MCXref xref">Optimera projekt i [!UICONTROL Portfolio Optimizer]</a>.</p></td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-undo-redo-icons-optimizer.png"> </td> 
   <td>[!UICONTROL Undo]/ [!UICONTROL Redo] ikoner</td> 
   <td>Använd de här ikonerna om du vill avbryta eller göra om de ändringar du gjorde i [!UICONTROL Portfolio Optimizer] innan du sparade.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/hide-show-unselected-portfolio-optimizer-142x74.png" alt="hide_show_unselected_portfolio_optimizer.png" style="width: 142;height: 74;"> </td> 
   <td>[!UICONTROL Show]/[!UICONTROL Hide] omarkerade projekt</td> 
   <td>Använd de här ikonerna för att visa eller dölja projekt i portföljen som du inte har markerat.</td> 
  </tr> 
  <tr> 
   <td> <img src="assets/nwe-export-optimizer-icon-350x173.png" style="width: 350;height: 173;"> </td> 
   <td>[!UICONTROL Export] </td> 
   <td> <p>Använd den här ikonen om du vill exportera data i området [!UICONTROL Project Prioritization] i [!UICONTROL Portfolio Optimizer]. Du kan exportera den till följande format:</p> 
    <ul> 
     <li>PDF</li> 
     <li>[!DNL Excel]</li> 
     <li>[!UICONTROL Tab] Avgränsad</li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td> <img src="assets/preferences-portfolio-optimizer.png" alt="preferences_portfolio_optimizer.png"> </td> 
   <td>[!UICONTROL Preferences]</td> 
   <td> <p>Använd den här ikonen om du vill ändra de projektfält som visas i kolumnerna för [!UICONTROL Portfolio Optimizer], eller om du vill ändra vilka projekt som visas i [!UICONTROL Optimizer] utifrån deras status. </p> <p>Tips:  
     <ul> 
      <li> <p>Alla [!DNL Workfront] standardfält är inte tillgängliga för tillägg i kolumnerna. </p> </li> 
     </ul> 
     <ul> 
      <li> <p>Du kan bara lägga till anpassade fält som har ett annat värde än noll i något av projekten i portföljen.</p> </li> 
     </ul> </p> </td> 
  </tr> 
 </tbody> 
</table>
