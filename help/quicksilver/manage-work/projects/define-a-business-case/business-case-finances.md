---
content-type: overview
navigation-topic: business-case-and-scorecards
title: Översikt över finansiella fält för ärenden
description: Underfliken Affärsärende innehåller finansiella fält för projektet. För att vissa av de finansiella fälten ska få sina värden måste motsvarande områden i affärsärendet fyllas i.
author: Becky
feature: Work Management
exl-id: d420fc3e-e98d-47a0-a456-b2df17d72f34
source-git-commit: fa0b4322b9f7c1d506cf194645c7ae50ad8c0f0b
workflow-type: tm+mt
source-wordcount: '745'
ht-degree: 0%

---

# Översikt över finansiella fält för ärenden

Underfliken Affärsärende innehåller finansiella fält för projektet. För att vissa av de finansiella fälten ska få sina värden måste motsvarande områden i affärsärendet fyllas i.  

Följande finansiella projektfält visas i affärsärendet:

<table border="1" cellspacing="15" cellpadding="1"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th scope="col">Fältets namn</th> 
   <th scope="col">Beskrivning</th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td>Justerad </td> 
   <td> <p>Visar projektets justering enligt styrkortet. Ett högt procentvärde anger att projektet är väl anpassat till organisationens syfte och mål. <br>Mer information om hur du använder styrkort finns i <a href="../../../administration-and-setup/set-up-workfront/configure-system-defaults/create-scorecard.md" class="MCXref xref">Skapa ett styrkort</a>.</p> <p>Det här fältet visas i området Affärsärendesammanfattning. </p> </td> 
  </tr> 
  <tr> 
   <td>Budgeterad kostnad</td> 
   <td> <p>Den totala kostnad som beräknas vara associerad med projektet när projektet startas.</p> <p>Budgeterad kostnad för projektet beräknas med följande formel:<br></p> <p><code>Budgeted Cost =&nbsp;Budgeted Expense Cost + Budgeted Labor Cost </code> <br> </p> <p>Adobe Workfront använder budgeterade timmar från resursplaneraren för att beräkna den budgeterade arbetskostnaden.<br>Mer information om beräkning av budgeterad kostnad finns i <a href="../../../manage-work/projects/project-finances/budgeted-cost.md" class="MCXref xref">Beräkna budgeterad kostnad</a>. </p> <p>Det här fältet visas i området Affärsärendesammanfattning.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgeterad utgift</td> 
   <td> <p>Den budgeterade kostnaden för alla utgifter i projektet. </p> <p>Detta beräknas med följande formel:</p> <p><code>Budgeted Expense Cost = SUM(Planned Amount of Expenses on the project) </code></p> <p>Mer information om hur du beräknar utgifter finns i <a href="../../../manage-work/projects/project-finances/manage-project-expenses.md" class="MCXref xref">Hantera projektutgifter </a>.</p> <p>Det här fältet visas i området Utgifter.</p> </td> 
  </tr> 
  <tr> 
   <td>Budgeterad arbetskostnad</td> 
   <td> <p>Kostnaden som är associerad med de resurser som har tilldelats för att slutföra arbetet i projektet.</p> <p>Budgeterad arbetskostnad för projektet beräknas med följande formel:<br></p> <p><code>Budgeted Labor Cost = SUM(Estimated/ Budgeted hours for each job role on the project * Cost per Hour rate of each job role on the project) </code><br></p> <p>Workfront använder budgeterade timmar från resursplaneraren för att beräkna den budgeterade arbetskostnaden.<br>Mer information om beräkning av budgeterad arbetskostnad finns i <a href="../../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Förstå budgeterad arbetskostnad och budgeterade timmar för projekt</a>.</p> <p>Det här fältet visas i området Resursbudgetering i affärsärendet. </p> </td> 
  </tr> 
  <tr> 
   <td>Planerad kostnad</td> 
   <td> <p>Detta är samma som Budgeterad utgift. </p> <p>Obs! Den planerade kostnaden för utgifter skiljer sig från den planerade kostnaden för projektet. Den planerade kostnaden beräknas som det planerade beloppet för utgifterna i projektet, medan den planerade kostnaden beräknas med hjälp av projektets planerade timmar. </p> <p>Det här fältet visas i området Utgifter för varje utgift.</p> </td> 
  </tr> 
  <tr> 
   <td>Nettovärde</td> 
   <td> <p>Detta är det totala förväntade värdet av projektet efter att man har beräknat dess nytta och tagit bort kostnaderna.</p> <p>Nettovärdet för projektet beräknas med följande formel:<br></p> <p><code>Net Value = Planned Benefit - Budgeted Cost - Potential Risk</code>. <br></p> <p>Mer information om hur du beräknar nettovärde finns i <a href="../../../manage-work/projects/project-finances/calculate-net-value.md" class="MCXref xref">Beräkna nettovärde</a>.<br></p> <p>Det här fältet visas i området Affärsärendesammanfattning.</p> </td> 
  </tr> 
  <tr> 
   <td>Planerad förmån</td> 
   <td>En manuell uppskattning av den monetära fördelen för organisationen när projektet är klart. Det kan vara vilket belopp som helst och det är specifikt för dig och för varje projekt du hanterar. Den planerade förmånen får inte ha ett negativt värde. Det här fältet visas i området Affärsärendesammanfattning och kan redigeras i området Projektinformation i affärsärendet. </td> 
  </tr> 
  <tr> 
   <td>Potentiell kostnad för risker</td> 
   <td> <p>Detta är den potentiella kostnaden för alla risker i projektet. </p> <p>Detta beräknas med följande formel:</p> <p><code>Potential Risk = SUM(Potential Cost * Probability of Risk) </code></p> <p>Mer information om risker i projektet finns i <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Skapa och redigera risker i projekt</a>.</p> <p>Det här fältet visas i området Affärsärendesammanfattning.</p> </td> 
  </tr> 
  <tr> 
   <td>Potentiell risk</td> 
   <td> <p>I affärsfallssammanfattningen är detta beloppet för kostnaden för alla risker om de skulle inträffa, baserat på sannolikheten för dem. Om en risk till exempel har en potentiell kostnad på 100 USD och en sannolikhet på 10 %, är den potentiella risken 10 USD. Den potentiella risken i affärsärendesammanfattningen beräknas enligt följande formel:</p> <p><code>Potential&nbsp;Risk = SUM(Risk Potential Cost x Probability)</code> för alla risker. </p> </td> 
  </tr> 
  <tr> 
   <td>Riskreduceringskostnad</td> 
   <td> <p>Kostnaden för reduceringsplanen för de risker du uppskattar kan uppstå i projektet.<br>Mer information om risker i projektet finns i <a href="../../../manage-work/projects/define-a-business-case/create-edit-risks-on-projects.md" class="MCXref xref">Skapa och redigera risker i projekt</a>.</p> <p>Det här fältet visas i området Risker för varje risk som anges i projektet.</p> </td> 
  </tr> 
  <tr> 
   <td>Potentiell kostnad för en risk</td> 
   <td> <p>Den uppskattade finansiella kostnaden när de risker som definierats för projektet faktiskt skulle inträffa, oavsett sannolikhet. </p> <p>Det här är ett manuellt uppdaterat fält som visas för varje risk i området Risker i affärsärendet. </p> </td> 
  </tr> 
  <tr> 
   <td>Totala potentiella kostnader för risker</td> 
   <td> <p>Här anges den totala uppskattade finansiella kostnaden för alla risker som definierats i projektet när de faktiskt har inträffat. </p> <p>Detta beräknas med följande formel:</p> <p><code>Risks Total Potential Cost = SUM(Potential Cost of all risks on the project) </code></p> <p>Det visas som ett valutanummer bredvid titeln på området Risker i affärsärendet.</p> </td> 
  </tr> 
 </tbody> 
</table>
