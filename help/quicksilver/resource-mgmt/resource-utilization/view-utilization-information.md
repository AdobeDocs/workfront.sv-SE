---
product-area: resource-management
navigation-topic: resource-utilization
title: Visa information om resursutnyttjande
description: Du kan visa användningen av dina resurser med hjälp av användningsrapporten.
author: Alina, Lisa
feature: Resource Management
exl-id: 785ee3e9-1b2d-4180-bc78-c41e71c5244d
source-git-commit: d2b62f2ec2f52c54129b342d68c336c782601242
workflow-type: tm+mt
source-wordcount: '7854'
ht-degree: 0%

---

# Visa information om resursutnyttjande

{{highlighted-preview}}

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;this is linked to the UI from the Utilization report. ALWAYS keep this information. DO NOT DELETE!!)</p>
-->

Du kan visa användningen av dina resurser med hjälp av användningsrapporten.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: Vazgen's response about these hours ie below and he asked us to NOT document them:</p>
<p>It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours.</p>
<p>In some cases, like for Planned Hours, it takes them from Assignments</p>
<p>But Budgeted Hours come from projects.</p>
<p>And Actual Hours are their own object - Hour)</p>
</div>
-->

<!--
<p style="color: #dc143c;" data-mc-conditions="QuicksilverOrClassic.Draft mode">This report displays information about the assignments on work items for projects in your environment, like Planned, Actual, and Budgeted Hours, FTE, or Cost.&nbsp;These are hours,&nbsp;FTE, or costs associated with the assignments and not with the tasks and issues themselves.(PRIVATE NOTE:&nbsp;Vazgen's response about these hours: It queries Assignments first to get the tasks, issues, projects to display in the view. And then from those gets the hours. In some cases, like for Planned Hours, it takes them from Assignments; But Budgeted Hours come from projects. And Actual Hours are their own object - Hour.)</p>
-->

## Åtkomstkrav

Du måste ha följande för att få tillgång till användningsrapporten:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">Adobe Workfront-plan*</td> 
   <td> <p>Pro eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licens*</td> 
   <td> <p>Plan </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>Visa eller öka åtkomsten till följande:</p> 
    <ul> 
     <li> <p>Resurshantering </p> </li> 
     <li> <p>Projekt</p> </li> 
     <li> <p>Portfolio</p> </li> 
     <li> <p>Program</p> </li> 
     <li> <p>Finansiella data om du vill visa information efter kostnad</p> </li> 
    </ul> <p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Visa åtkomst till projekt, portföljer och program för att komma åt användningssektionen i resursområdet</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-highloighted-350x145.png" style="width: 350;height: 145;"> </p> <p>Hantera åtkomst till projektet för att få åtkomst till användningsavsnittet i ett projekt</p> <p data-mc-conditions="QuicksilverOrClassic.Quicksilver"> <img src="assets/nwe-utilization-section-on-project-highloighted-350x289.png" style="width: 350;height: 289;"> </p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta Workfront-administratören om du vill veta vilken plan, licenstyp eller åtkomst du har.

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">You must have View access to the projects you want to view utilization information for as described in this section. If you are still unable to access this information, contact your Workfront administrator. (NOTE:&nbsp;replaced with above table)</p>
-->

I följande avsnitt beskrivs hur du visar och använder användningsinformation.

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<h2>Prerequisites for accessing utilization information</h2>
<p>(NOTE: drafted, replaced with above table)</p>
<p>To access utilization information as described in this section, ensure that the following conditions are met:</p>
<ul>
<li>You have at least&nbsp;View access to the project, program, or portfolio for which you want to view the utilization information.</li>
<li>Your Workfront administrator must grant you at least View access to&nbsp;Financial&nbsp;Data in your Access Level to be able to view cost and revenue information in the Utilization report. The Workfront administrator must enable both View Role Billing & Cost Rates as well as View User Billing &&nbsp;Cost Rates when they grant you the View access to Financial Data. For information about granting access to&nbsp;Financial&nbsp;Data, see <a href="../../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md" class="MCXref xref">Grant access to financial data</a>. </li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;drafted. No longer the case.) </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Reporting area. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is included on any layout template that is assigned to you and that is applied to either the projects you view or to the Resourcing area. </p>
</li>
<li>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization tab is available by default in the Reporting area if the system administrator has not assigned a custom layout template to you. </p>
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">The Utilization section is available by default in the Resourcing area if the system administrator has not assigned a custom layout template to you. </p>
</li>
</ul>
</div>
-->

## Översikt över användningsrapporten {#overview-of-the-utilization-report}

Med användningsrapporten kan du visa förloppet, kostnaden eller intäkterna för ett projekt, ett program eller en portfölj i en enda rapport. Du kan också jämföra intäkter med kostnad.

Du kan visa användningsrapporten i området Resurser om du vill visa användning för flera projekt, eller så kan du visa den på nivån för ett projekt, om du vill visa användning för de enskilda resurser (jobbroller och användare) som är associerade med projektet.

Mer information om hur du använder och använder användningsrapporten finns i [Följ upp framsteg, kostnader och intäkter med användningsrapporten](#track-progress-cost-and-revenue-with-the-utilization-report) i den här artikeln.

* [Spåra timmar (förlopp)](#track-hours-progress)
* [Spåra kostnad](#track-cost)
* [Spåra intäkter](#track-revenue)
* [Jämför intäkter med planerade och faktiska kostnader](#compare-revenue-against-planned-and-actual-costs)

### Spåra timmar (förlopp) {#track-hours-progress}

Du kan följa förloppet genom att visa hur budgeterade och planerade timmar jämförs med faktiska timmar.

När du håller reda på förloppet för ett projekt, program eller en portfölj inkluderas framsteg mot både uppgifter och problem i användningsrapporten.

Följande information finns i användningsrapporten när timmar spåras:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Kolumnrubrik vid visning av timmar</strong> </th> 
   <th><strong> -funktion</strong> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgeterade timmar</strong> </td> 
   <td scope="col"> <p>Det totala antalet budgeterade timmar för de inkluderade projekten. Du kan visa det totala antalet budgeterade timmar för den totala livslängden för de inkluderade projekten, eller så kan du visa det totala budgeterade timmarna endast för det angivna datumintervallet (du kan ange en enskild vecka eller månad). </p> <p>Budgeterade timmar fylls i från information som är tillgänglig i den nya resursbudgeteringsområdet för affärsärendet eller resursplaneraren<em>.</em></p> <p>Budgeterade timmar visas i användningsrapporten på någon av följande rader:</p> 
    <ul> 
     <li> Budgeterade timmar summeras efter jobbroll och av enskilda användare i utnyttjanderapporten enligt följande:<br><strong>Enskild användare:</strong> Budgeterade timmar summeras för varje användare i utnyttjanderapporten. Dessa budgeterade timmar är associerade med de uppgifter och utgåvor som användaren är tilldelad till i de inkluderade projekten. (Du kan expandera raden för motsvarande jobbroll för att visa en lista över användare med den jobbrollen.)<br><strong>Jobbroll:</strong> Budgeterade timmar summeras efter jobbroll i utnyttjanderapporten.<br>Budgeterade timmar visas i en viss jobbroll som ett resultat av något av följande scenarier: 
     <li>Jobbrollen definieras som den primära jobbrollen för användaren som är tilldelad uppgiften eller utleveransen där de budgeterade timmarna är associerade. </li> 
       <li>När du visar användningsinformation för ett enskilt projekt används jobbrollen för användaren som tilldelats timarna, oavsett om det inte finns någon tilldelning för uppgiften eller utgåvan, en annan användare tilldelas utan jobbrolltilldelning, en annan användare tilldelas med en annan jobbroll eller ett annat team tilldelas.</li> 
       <li>När du visar användningsinformation för flera projekt, program eller portföljer, används endast jobbrollen för användaren som tilldelats timmarna när rollen tilldelas för en aktivitet eller utgåva i ett projekt. </li> 
       <li>Jobbrollen tilldelas till uppgiften eller utgåvan som har associerade budgeterade timmar och användaren som är tilldelad uppgiften eller utgåvan har inte någon jobbroll definierad i systemet.</li> 
      </ul></li> 
    </ul> 
    <ul> 
     <li> <p><strong>Ej allokerade timmar</strong>: Budgeterade timmar visas i användningsrapporten i avsnittet Ej allokerade timmar när budgeterade timmar är associerade med en uppgift eller utgåva och det inte finns någon användare eller roll tilldelad till uppgiften eller utgåvan.<br>Det här avsnittet visas bara när det finns timmar i projektet som matchar den här beskrivningen och när du visar användningsrapporten från eller från ett projekt. </p> <p>Det här avsnittet visas bara när det finns timmar i projektet som matchar den här beskrivningen och när du visar användningsrapporten från eller från ett projekt. </p> </li> 
    </ul> <p>Mer information om budgeterade timmar finns i avsnittet Hitta budgeterade timmar för ett projekt i <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Förstå budgeterad arbetskostnad och budgeterade timmar för projekt</a> artikel.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planerade timmar</strong> </td> 
   <td scope="col"> <!-- Yay, no errors, warnings, or alerts! -->

<p>
Planerade timmar för de inkluderade projekt som är associerade med tilldelningarna för varje uppgift och utgåva. Du kan visa det totala antalet planerade timmar för alla tilldelningar i projektet under den totala tiden för de inkluderade projekten, eller så kan du bara visa totalt antal planerade timmar för det angivna datumintervallet (du kan ange en enskild vecka eller månad). 
</p>
<p>
<strong>TIPS </strong>
</p>
<p>
De planerade timmarna från artiklar med en varaktighet på 0 räknas inte. 
</p>
<p>
Planerade timmar i användningsrapporten tar hänsyn till om de planerade timmarna har omfördelats under en uppgifts- eller utgivningsperiod. 
</p>
<p>
När användarens dagliga allokering för timmar har ändrats med hjälp av arbetsbelastningsutjämnaren, kan informationen i användningsrapporten påverkas om de datum som valts i användningsrapporten bara innehåller en del av en uppgifts eller ärendets varaktighet. 
</p>
<p>
Mer information om hur du ändrar tilldelningar för användare finns i <a href="../workload-balancer/manage-user-allocations-workload-balancer.md">Hantera användarallokeringar i Utjämning av arbetsbelastning</a>.


</p>
<p>
Planerade timmar visas på användningsrapporten på någon av följande rader:
</p>
<ul>

<li>Planerade timmar sammanfattas efter jobbroll och av enskilda användare i utnyttjanderapporten enligt följande: 
<ul>

<li><strong>Enskild användare</strong>: Planerade timmar sammanfattas för varje användare i användningsrapporten. De här planerade timmarna är kopplade till de uppgifter och utgåvor som användaren är tilldelad till i de inkluderade projekten. (Du kan expandera raden för motsvarande jobbroll för att visa en lista över användare med den jobbrollen.)

<li><strong>Jobbroll</strong>: Planerade timmar sammanfattas av jobbroll i utnyttjanderapporten för ett enskilt projekt.<br>Planerade timmar visas i en viss jobbroll som ett resultat av något av följande scenarier:  
<ul>

<li>Jobbrollen definieras som den primära jobbrollen för användaren som är tilldelad till uppgiften eller utgåvan där de planerade timmarna är associerade.

<li>När du visar användningsinformation för ett enskilt projekt visas inte timmarna som är associerade med en jobbroll för jobbrollen i följande scenarier:   
<ul>

<li>Det finns ingen tilldelning för aktiviteten eller problemet

<li>En användare har tilldelats utan jobbrolltilldelning

<li>En användare har tilldelats en annan jobbroll

<li>Ett team har tilldelats uppgiften eller utgåvan
</li>   
</ul>

<li>När du visar användningsinformation för flera projekt, program eller portföljer, används endast jobbrollen för användaren som tilldelats timmarna när rollen tilldelas för en aktivitet eller utgåva i ett projekt. Jobbrollstimmar visas inte separat när du visar användningsrapporten för flera projekt.

<li>Jobbrollen tilldelas till uppgiften eller utgåvan som har associerade planerade timmar och användaren som är tilldelad uppgiften eller utgåvan har inte någon jobbroll definierad i systemet.
</li>  
</ul>

<li><strong>Ej allokerade timmar</strong>: Planerade timmar visas i användningsrapporten i avsnittet Ej allokerade timmar när Planerade timmar är associerade med en aktivitet eller ett problem och det inte finns någon användare eller roll tilldelad till uppgiften eller problemet. Det här avsnittet visas bara när det finns timmar i projektet som matchar den här beskrivningen och när användningsrapporten för ett enskilt projekt visas. <br>Mer information om planerade timmar finns i <a href="../../manage-work/tasks/task-information/planned-hours.md">Översikt över planerade timmar</a>.
</li> 
</ul>
</li> 
</ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Faktiska timmar</strong> </td> 
   <td> <p> Totalt antal loggade timmar för uppgifter, utleveranser, <span>och i projektet</span> för de projekt som ingår. Du kan visa de totala faktiska timmarna för den övergripande livstiden för de inkluderade projekten, eller så kan du bara visa de totala faktiska timmarna för det angivna datumintervallet (du kan ange en enskild vecka eller månad). </p> <p>Varning: Användningsrapporten innehåller timmar som loggats till projektet, underordnade uppgifter, utgåvor och överordnade uppgifter med minst en tilldelning. Det omfattar inte timmar som loggats till överordnade uppgifter utan tilldelningar. Vi rekommenderar att du inte använder överordnade uppgifter som arbetsuppgifter och endast tilldelar underordnade uppgifter till dina resurser. </p> <p>Faktiska timmar visas i användningsrapporten på någon av följande rader:</p> 
    <ul> 
     <li> Faktiska timmar sammanfattas efter jobbroll och av enskilda användare i utnyttjanderapporten för ett projekt enligt följande:<br><strong>Enskild användare:</strong> Faktiska timmar visas i användningsrapporten på raden för den användare som loggade timmarna. (Du kan expandera raden för motsvarande jobbroll för att visa en lista över användare med den jobbrollen som har loggade timmar.)<br><strong>Jobbroll:</strong> Faktiska timmar som loggas av användare som är associerade med dessa roller sammanfattas i användningsrapporten på raden för motsvarande jobbroll.<br>Faktiska timmar visas i en viss jobbroll som ett resultat av något av följande scenarier: 
      <ul> 
       <li>Jobbrollen definieras som den primära jobbrollen för användaren som loggade timmarna.</li> 
       <li>Det finns ingen tilldelning för aktiviteten eller problemet</li> 
       <li>En annan användare har tilldelats utan jobbrolltilldelning</li> 
       <li>En annan användare har tilldelats en annan jobbroll</li> 
       <li> <p>Ett team har tilldelats.</p> </li> 
      </ul></li>  
     <p>Om användaren som loggar timmarna inte har någon jobbroll associerad med sin profil, är den jobbroll som används för användningsrapporten den jobbroll som tilldelats uppgiften eller utgåvan där timmar loggas eller den jobbroll som är associerad med den primära ägaren av uppgiften eller utgåvan. </p> 
     <li><strong>Övriga timmar:</strong> Faktiska timmar visas i användningsrapporten i avsnittet Andra timmar, på raden för användaren som loggade in timmarna.<br>Timmar visas i det här avsnittet när användaren som loggade timmarna inte har någon jobbroll definierad i systemet.<br>Det här avsnittet visas bara när det finns timmar i projektet som matchar den här beskrivningen. </li> 
    </ul> </td> 
  </tr> 
  <tr> 
   <td><strong>Budgeterad avvikelse (för timmar)</strong> </td> 
   <td> <p>Det totala antalet budgeterade timmar minus det totala antalet faktiska timmar för de inkluderade projekten. Du kan visa den totala budgeterade avvikelsen för den totala livslängden för de inkluderade projekten, eller så kan du visa den totala budgeterade avvikelsen endast för det angivna datumintervallet (du kan ange en enskild vecka eller månad). </p> <p>Om värdet är positivt visas det i grönt. Detta anger att det totala antalet budgeterade timmar är större än de faktiska timmarna.</p> <p>Om värdet är negativt visas det i rött. Detta anger att det totala antalet budgeterade timmar är mindre än de faktiska timmarna.</p> <p> <img src="assets/utilization-variance-budgeted-350x96.png" style="width: 350;height: 96;"> </p> </td> 
  </tr> 
  <tr> 
   <td><strong>Planerad avvikelse (för timmar)</strong> </td> 
   <td> <p>Det totala antalet planerade timmar minus det totala antalet faktiska timmar i de inkluderade projekten. Du kan visa den totala planerade avvikelsen för den övergripande livslängden för de inkluderade projekten, eller så kan du bara visa den totala planerade avvikelsen för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> <p>Om värdet är positivt visas det i grönt. Detta anger att det totala antalet planerade timmar är större än de faktiska timmarna.</p> <p>Om värdet är negativt visas det i rött. Detta anger att det totala antalet planerade timmar är mindre än det faktiska antalet timmar.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Spåra kostnad {#track-cost}

Du kan spåra kostnader genom att visa hur de budgeterade kostnaderna och de planerade kostnaderna jämförs med de faktiska kostnaderna.

När du spårar kostnaderna för ett projekt, program eller en portfölj kommer information i användningsrapporten från uppgifter. Kostnadsinformation från uppgifter finns alltid i användningsrapporten. Kostnaden för uppgifter beräknas utifrån uppgiftens kostnadstyp. Mer information om kostnadstypen för uppgifter finns i&quot;Ändra kostnadstyper för enskilda uppgifter&quot; i [Spåra kostnader](../../manage-work/projects/project-finances/track-costs.md).

Du kan visa kostnadsinformation i användningsrapporten på följande sätt:

* För en viss vecka eller månad, eller för hela projektet, programmet eller portföljen.
* Per roll eller individ, för projekt.

Valutan som används i utnyttjanderapporten bestäms av den valuta som har angetts för projektet. Mer information om hur du justerar valutan för ett projekt finns i [Ändra projektvalutan](../../manage-work/projects/project-finances/change-project-currency.md).

Följande information finns i användningsrapporten när du spårar kostnad:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Kolumnrubrik vid visning av kostnad</strong> </th> 
   <th> <p><strong> -funktion</strong> </p> </th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgeterad kostnad</strong> </td> 
   <td scope="col"> <p>Budgeterad kostnad för de inkluderade projekten. Du kan visa den totala budgeterade kostnaden för den övergripande livscykeln för de inkluderade projekten, eller så kan du bara visa den totala budgeterade kostnaden för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> <p>Eftersom den budgeterade kostnaden i användningsrapporten är inriktad på kostnad per roll är beräkningen densamma som den budgeterade arbetskostnaden inom andra områden i Workfront. Mer information om hur budgeterad arbetskostnad beräknas finns i <a href="../../manage-work/projects/project-finances/budgeted-labor-cost.md" class="MCXref xref">Förstå budgeterad arbetskostnad och budgeterade timmar för projekt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planerad kostnad</strong> </td> 
   <td scope="col"> <p>Den totala planerade kostnaden för de inkluderade projekten. Du kan visa den totala planerade kostnaden för den totala livscykeln för de inkluderade projekten, eller så kan du bara visa den totala planerade kostnaden för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> <p><span class="preview">Observera att för vyerna vecka, månad och kvartal beräknas de planerade kostnaderna som ett genomsnitt av den valda perioden när kostnadstarifferna för jobbroller eller användare är gällande.</span></p><p>Information om hur den planerade kostnaden för projektet beräknas finns i avsnittet"Hur Workfront beräknar planerade, budgeterade och faktiska kostnader" i artikeln <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Faktisk kostnad</strong> </td> 
   <td scope="col"> <p>Den totala faktiska kostnaden för de inkluderade projekten. Du kan visa den totala faktiska kostnaden för den övergripande livscykeln för de inkluderade projekten, eller så kan du bara visa den totala faktiska kostnaden för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> <p>Information om hur den faktiska kostnaden för projektet beräknas finns i avsnittet"Hur Workfront beräknar planerade, budgeterade och faktiska kostnader" i artikeln <a href="../../manage-work/projects/project-finances/track-costs.md" class="MCXref xref">Spåra kostnader</a>.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Budgeterad avvikelse (för kostnad)</strong> </td> 
   <td scope="col"> <p>Den totala budgeterade kostnaden minus den totala faktiska kostnaden för de inkluderade projekten. Du kan visa den totala budgeterade avvikelsen för den totala livslängden för de inkluderade projekten, eller så kan du visa den totala budgeterade avvikelsen endast för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> <p>Om värdet är positivt visas det i grönt. Detta anger att den totala budgeterade kostnaden är större än den faktiska kostnaden.</p> <p>Om värdet är negativt visas det i rött. Detta anger att den totala budgeterade kostnaden är mindre än den faktiska kostnaden.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Planerad avvikelse (för kostnad)</strong> </td> 
   <td> <p>Den totala planerade kostnaden minus den totala faktiska kostnaden för de inkluderade projekten. Du kan visa den totala planerade avvikelsen för den övergripande livslängden för de inkluderade projekten, eller så kan du bara visa den totala planerade avvikelsen för det angivna datumintervallet (du kan ange en enskild vecka eller månad). </p> <p>Om värdet är positivt visas det i grönt. Detta anger att den totala planerade kostnaden är större än den faktiska kostnaden.</p> <p>Om värdet är negativt visas det i rött. Detta anger att den totala planerade kostnaden är mindre än den faktiska kostnaden.</p> </td> 
  </tr> 
 </tbody> 
</table>

### Spåra intäkter {#track-revenue}

Du kan spåra intäkter genom att visa hur de budgeterade och planerade intäkterna jämförs med de faktiska intäkterna.

När du spårar intäkten för ett projekt, ett program eller en portfölj inkluderas endast intäkter från uppgifter i användningsrapporten.

Informationen i följande tabell är tillgänglig i användningsrapporten när du spårar intäkt.

Mer information om fälten och hur Workfront beräknar dem finns i följande artiklar:

* [Spåra kostnader](../../manage-work/projects/project-finances/track-costs.md)
* [Översikt över fakturering och intäkt](../../manage-work/projects/project-finances/billing-and-revenue-overview.md)

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Kolumnrubrik vid visning av intäkt</strong> </th> 
   <th> <strong> -funktion</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Budgeterade intäkter</strong> </td> 
   <td scope="col"> <p>Den totala budgeterade timmen multiplicerad med Roll Billing Rate för de inkluderade projekten. Du kan visa den totala budgeterade intäkten för den övergripande livslängden för de inkluderade projekten, eller så kan du bara visa den totala budgeterade intäkten för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planerad intäkt</strong> </td> 
   <td scope="col"> <p>Planerad intäkt i användningsrapporten är den intäkt som är associerad med de planerade timmarna som tilldelats resurserna för aktiviteterna i projektet.</p> <p>Workfront beräknar projektets planerade inkomster för utnyttjanderapporten enligt följande formel:</p> <p><code>Project Planned Revenue = SUM&nbsp;(All Tasks Planned Revenue)</code> </p> 
   <p><b>ANMÄRKNING</b>
   <p>Projektets planerade inkomster som visas i utnyttjanderapporten skiljer sig från den planerade intäkten som visas i området Projektinformation och projektrapporter. </p> <p>Planerad intäkt i området Projektinformation återspeglar aktivitetsintäkten och projektets fasta intäkt. Planerad intäkt i användningsrapporten visar planerad intäkt som bara är associerad med aktiviteterna i projektet. </p> 
     <div class="example" data-mc-autonum="<b>Example: </b>">  
      <p>Om projektet har 1 uppgift med 10 timmar, som tilldelats en konsult med en timtaxa på 20 USD och projektet har en fast intäkt på 100 USD, visar användningsrapporten 200 USD för planerad intäkt (den planerade intäkten som är associerad med timmarna för uppgiften). I avsnittet Projektinformation visas $300 (den planerade intäkten från aktiviteten och den fasta intäkten för projektet). </p> 
     </div> <p>Mer information om planerad intäkt utanför användningsrapporten för uppgiften och projektet finns i <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkt</a>.</p> </p> <p>Hur användningsrapporten beräknar och visar planerade intäkter för de inkluderade projekten tar hänsyn till uppgiftens intäktstyp. </p> <p>Beroende på intäktstypen för varje uppgift i projektet finns följande scenarier: </p> <p><strong>Fast intäkt:</strong> Oavsett uppgiftstilldelningarna beräknas alltid aktivitetens intäkt med det fasta belopp som har angetts för aktiviteten.</p> <p><b>VIKTIGT</b>

Till skillnad från inom andra områden av Workfront beräknar användningsrapporten Planerad intäkt för uppgifter med fast intäkt genom att dividera Fast intäkt jämnt med antalet planerade timmar för uppgiften. </p> <p>En aktivitet har till exempel en intäkt på $200. Om aktiviteten har 4 planerade timmar blir varje timme 50 dollar. Detta distribueras på användar- och rollnivå. Distributionen är unik för användningsrapporten.</p> <p><b>ANMÄRKNING</b>

Om du har en aktivitet med fast intäkt och det inte finns några planerade timmar för uppgiften, visas inte Intäkter i användningsrapporten eftersom det inte går att distribuera den till timmarna. Om du har planerat timmar för uppgifter med fast intäkt och inga tilldelningar visas Intäkter som Ej allokerad intäkt. </p> <p><strong>Roll varje timme:</strong> Inkomsterna för aktiviteten beräknas med den faktureringsränta som har angetts för en viss roll, multiplicerat med antalet planerade timmar som är associerat med den rollen. Workfront använder följande formel:</p> <p><code>Planerad intäkt per timme för roll = SUM(Planerade timmar från roll för alla aktiviteter) * Faktureringshastighet för roll</code></p><p><span class="preview"><b>OBS!</b> Timtaxan för fakturering i formeln tar hänsyn till eventuella datumändringar i räntesatsen.</span></p>   <p><strong>Användartimme:</strong> Inkomsterna för aktiviteten beräknas med hjälp av den angivna faktureringssatsen för en viss användare, multiplicerat med antalet planerade timmar som är associerat med den användaren. Workfront använder följande formel:</p> <p><code>Planerad intäkt per timme för användare = SUM(Planerade timmar från användare för alla uppgifter) * Faktureringshastighet för användare</code> </p> <p><span class="preview"><b>OBS!</b> Timtaxan för fakturering i formeln tar hänsyn till eventuella datumändringar i räntesatsen.</span></p> <p><b>Roll timvis eller Användartimme plus fast</b> </p> <p><b>VIKTIGT</b>

Till skillnad från andra områden i Workfront beräknar användningsrapporten den planerade intäkten genom att dividera den fasta intäkten jämnt med antalet planerade timmar för uppgiften. </p> <p>Följande fall finns: </p>
<ul>
<li> <p><strong>Roll timvis plus fast:</strong> Inkomsterna för aktiviteten beräknas med den faktureringsränta som har angetts för en viss roll, multiplicerat med antalet planerade timmar som är associerat med rollen. Dessutom läggs ett fast belopp som anges för aktiviteten till i rollfrekvensen. Workfront använder följande formel:</p> <p><code>Roll timvis plus fast planerad intäkt = [SUM (Planerade timmar från roll för alla uppgifter) * Rollfaktureringshastighet] + SUM(aktivitetens tak eller fasta belopp/uppgiftens planerade timmar)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Användarens timlön plus fast:</strong> Faktureringssatsen som har angetts för en viss användare, multiplicerat med antalet planerade timmar för aktiviteten från den användaren. Dessutom läggs ett fast belopp som anges för aktiviteten till i användarfrekvensen. Workfront använder följande formel:</p> <p><code>Planerad intäkt per timme för användare plus fast planerad intäkt = [SUM (Planerade timmar från användare för alla uppgifter) * Faktureringshastighet för användare] + SUM(aktivitetens tak eller fasta belopp/uppgiftens planerade timmar)</code> </p> </li>
</ul> <p><b>Roll eller användarens timma med ände</b> </p> <p><b>VIKTIGT</b>

Till skillnad från i andra områden i Workfront, om den planerade inkomsten överskrider taket, anses beloppet över det högsta beloppet som en fast intäkt. Planerad intäkt beräknas genom att den fasta intäkten delas jämnt med antalet planerade timmar för uppgiften och sedan läggs till i beloppet för Socket och rollen eller användarens timintäkt. <br></p> <p>Följande fall finns: </p>
<ul>
<li> <p><strong>Roll timvis med ändpunkt:</strong> Aktiviteter faktureras varje timme som i Roll-timmen, men de har ett maxbelopp som du kan ange. Workfront använder följande formel:</p> <p><code>Roll timvis med planerad kostnad = [SUM (Planerade timmar från roll för alla uppgifter och ärenden) * Roll Faktureringshastighet] + ändpunkt Uppgiftens belopp + SUM(Belopp över uppgifternas startbelopp / Planerade timmar)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Användarens timma med versaler:</strong> Aktiviteter faktureras varje timme som användaren anger, men de har ett maxbelopp som du kan ange. Workfront använder följande formel: </p> <p><code>Användaren per timme med Planerad intäkt för kap. = [SUM (Planerade timmar från användare för alla uppgifter) * Faktureringshastighet för användare] + ändpunkt Uppgiftens belopp + SUM(Belopp över uppgifternas startbelopp / Planerade timmar)</code> </p> </li>
</ul> <p>Mer information om vilken roll eller användare som ska beaktas vid beräkning av planerad intäkt finns i <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkt</a>.</p> </td>
</tr> 
  <tr> 
   <td><strong>Faktisk intäkt</strong> </td> 
   <td> <p>Faktisk intäkt är den intäkt som är associerad med aktivitetens faktiska timmar <span>och projektet</span>. Mer information om faktisk intäkt finns i avsnittet Spåra intäktsbelopp i artikeln <a href="../../manage-work/projects/project-finances/billing-and-revenue-overview.md" class="MCXref xref">Översikt över fakturering och intäkt</a>.</p>

<p>Hur användningsrapporten beräknar faktisk intäkt för de inkluderade projekten varierar beroende på vilken intäktstyp som har angetts för uppgiften, enligt följande:</p> <p><strong>Fast intäkt:</strong> Oavsett uppgiftstilldelningarna beräknas alltid aktivitetens intäkt med det fasta belopp som har angetts för aktiviteten.</p> <p><b>VIKTIGT</b>

Till skillnad från i andra områden i Workfront beräknar användningsrapporten Faktisk intäkt genom att dividera Fast intäkt jämnt med antalet timmar som loggats för uppgiften. </p> <p> </p> <p>En aktivitet har till exempel en faktisk intäkt på $200. Om aktiviteten har fyra faktiska timmar blir varje timme 50 USD. Detta distribueras på användar- och rollnivå. Distributionen är unik för användningsrapporten.</p> <p><b>ANMÄRKNING</b>

Om du har en aktivitet med fast intäkt och det inte finns några faktiska timmar för uppgiften, visas inte den faktiska intäkten i användningsrapporten eftersom det inte finns något sätt att fördela timmar. </p> <p><strong>Roll varje timme:</strong> Inkomsterna för aktiviteten beräknas med den faktureringsränta som har angetts för en viss roll, multiplicerat med antalet faktiska timmar.</p> <p>Workfront använder följande formel:</p> <p><code>Verklig intäkt per timme för roll = SUM (faktiska timmar från roll för alla aktiviteter) * Faktureringshastighet för roll</code> </p> <p><span class="preview"><b>OBS!</b> Timtaxan för fakturering i formeln tar hänsyn till eventuella datumändringar i räntesatsen.</span></p> <p><strong>Användartimme:</strong> Inkomsterna för aktiviteten beräknas med den faktureringsfrekvens som har angetts för en viss användare, multiplicerat med antalet timmar som loggats mot uppgiften från den användaren. Workfront använder följande formel:</p> <p><code>Faktisk intäkt per timme för användare = SUM(faktisk tid från användare för alla uppgifter) * Faktureringshastighet för användare</code></p> <p><span class="preview"><b>OBS!</b> Timtaxan för fakturering i formeln tar hänsyn till eventuella datumändringar i räntesatsen.</span></p> <p><b>Roll eller användarens timlön plus fast</b> </p> <p><b>VIKTIGT</b>

Till skillnad från i andra områden i Workfront beräknar användningsrapporten Faktisk intäkt genom att dividera Fast intäkt jämnt med antalet timmar som loggats för uppgiften. </p> <p>Följande fall finns: </p>
<ul>
<li> <p><strong>Roll timvis plus fast:</strong> Den faktureringsfrekvens som har angetts för en viss roll, multiplicerat med antalet timmar som loggats mot uppgiften från en användare med den rollen. Dessutom läggs ett fast belopp som anges för aktiviteten till i rollfrekvensen. </p> <p>Workfront använder följande formel:</p> <p><code>Roll timvis plus fast faktisk intäkt = [SUM (Faktiska timmar från roll för alla uppgifter) * Rollfaktureringshastighet] + SUM(aktivitetens tak eller fasta belopp/uppgiftens faktiska timmar)</code> </p> </li>
</ul>
<ul>
<li> <p><strong>Användarens timlön plus fast:</strong> Den faktureringsfrekvens som har angetts för en viss användare, multiplicerat med antalet timmar som loggats mot uppgiften från den användaren. Dessutom läggs ett fast belopp som anges för aktiviteten till i användarfrekvensen. </p> <p>Workfront använder följande formel:</p> <p><code>Användaren per timme plus fast faktisk intäkt = [SUM (Faktiska timmar från roll för alla uppgifter) * Faktureringshastighet för användare] + SUM(aktivitetens tak eller fasta belopp/aktivitetens användartimmar)</code> </p> </li>
</ul> <p><b>Roll eller användarens timma med ände</b> </p> <p><b>VIKTIGT</b>

Till skillnad från i andra områden i Workfront, om den planerade inkomsten överskrider taket, anses beloppet över det högsta beloppet som en fast intäkt. Planerad intäkt beräknas genom att den fasta intäkten delas jämnt med antalet planerade timmar för uppgiften och sedan läggs till i beloppet för Socket och rollen eller användarens timintäkt. <br></p> <p>Följande scenarier finns:</p>
<ul>
<li> <p><strong>Roll timvis med ändpunkt:</strong> Aktiviteter faktureras varje timme som i Roll-timmen, men de har ett maxbelopp som du kan ange. Workfront använder följande formel:</p> <p><code>Roll timvis med faktisk omsättning för kap. = [SUM (Faktiska timmar från roll för alla uppgifter och ärenden) * Roll Faktureringshastighet] + ändpunkt Uppgiftens belopp + SUM(Belopp över beloppets gräns/faktiska timmar för uppgiften)</code></p> </li>
</ul>
<ul>
<li> <p><strong>Användarens timma med versaler:</strong> Aktiviteter faktureras varje timme som användaren anger, men de har ett maxbelopp som du kan ange.</p> <p> Workfront använder följande formel:</p> <p><code>Användarens timma med den faktiska kostnaden = [SUM (Faktiska timmar från roll för alla uppgifter och ärenden) * Faktureringshastighet för användare] + ändpunkt Uppgiftens belopp + SUM(Belopp över beloppets gräns/faktiska timmar för uppgiften)</code> </p> </li>
</ul>
<div>
<p><strong>Projektintäkter</strong>: Inkomsterna som är kopplade till de timmar som är inloggade i projektet beräknas med hänsyn till beloppet Fakturering per timme för den primära jobbrollen för användaren som loggar tiden. Vi rekommenderar inte att du loggar på projektet. </p>
<p><b>ANMÄRKNING</b>

Om användaren inte är associerad med en jobbroll eller om fakturering per timme för den primära rollen är noll, beräknar Workfront faktisk intäkt med användarens faktureringsbelopp per timme. Om användaren inte har ett faktureringsbelopp per timme i sin profil är Faktisk intäkt noll. </p>
</div> </td>
</tr> 
  <tr> 
   <td><strong>Budgeterad avvikelse (för intäkt)</strong> </td> 
   <td> <p>Total faktisk intäkt minus budgeterad intäkt för de inkluderade projekten.<br>Du kan visa den totala budgeterade avvikelsen för den totala livslängden för de inkluderade projekten, eller så kan du visa den totala budgeterade avvikelsen endast för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> <p>Om värdet är positivt visas det i grönt. Detta anger att den totala budgeterade inkomsten är större än den faktiska inkomsten.</p> <p>Om värdet är negativt visas det i rött. Detta anger att den totala budgeterade inkomsten är mindre än den faktiska inkomsten.</p> </td> 
  </tr> 
  <tr> 
   <td><strong>Planerad avvikelse (för intäkt)</strong> </td> 
   <td> <p>Total faktisk intäkt minus den totala planerade intäkten för de inkluderade projekten.<br>Du kan visa den totala planerade avvikelsen för den övergripande livslängden för de inkluderade projekten, eller så kan du bara visa den totala planerade avvikelsen för det angivna datumintervallet (du kan ange en enskild vecka eller månad). </p> <p>Om värdet är positivt visas det i grönt. Detta anger att den totala planerade intäkten är större än den faktiska intäkten.</p> <p>Om värdet är negativt visas det i rött. Detta anger att den totala planerade intäkten är mindre än den faktiska intäkten.</p> </td> 
  </tr> 
 </tbody> 
</table>

<!--Note from the table about Actual revenue: 
     <p>Actual Revenue is displayed in the Utilization report only after the task is marked as Complete or Done (or a status that equates with Complete).</p>
    -->

<!--More notes from the table: 
     <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE:&nbsp;the note below is duplicated in this article: /Content/Manage work/Projects/Project Finances/billing-and-revenue-overview.html and in the glossary)</p>
   -->

### Jämför intäkter med planerade och faktiska kostnader {#compare-revenue-against-planned-and-actual-costs}

Du kan visa Planerad eller Faktisk kostnad tillsammans med Planerad intäkt. Marginalen (%) visas också (marginalen beräknas som Intäkter - Kostnad / Intäkter).

Följande information finns i användningsrapporten när du jämför intäkter med planerade och faktiska kostnader:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <thead> 
  <tr> 
   <th><strong>Kolumnrubrik vid visning av intäkter kontra kostnad (planerad)</strong> </th> 
   <th> <strong> -funktion</strong></th> 
  </tr> 
 </thead> 
 <tbody> 
  <tr> 
   <td scope="col"><strong>Planerad kostnad</strong> </td> 
   <td scope="col"> Den totala planerade kostnaden för de inkluderade projekten. Du kan visa den totala planerade kostnaden för den totala livscykeln för de inkluderade projekten, eller så kan du bara visa den totala planerade kostnaden för det angivna datumintervallet (du kan ange en enskild vecka eller månad). </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Planerad intäkt</strong> </td> 
   <td scope="col"> <p>Planerad intäkt är den intäkt som är associerad med aktiviteternas planerade timmar. </p> <p>Hur utnyttjanderapporten beräknar och visar den planerade intäkten för de inkluderade projekten varierar beroende på vilken intäktstyp som har angetts för uppgiften, enligt beskrivningen i <a href="#track-revenue" class="MCXref xref">Spåra intäkter</a> i den här artikeln.</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Marginal</strong> </td> 
   <td scope="col"> <p>Marginalprocenten beräknas enligt följande:</p> <p><code>Planned Revenue - Planned Cost / Planned Revenue * 100. </code></p> <p><b>ANMÄRKNING</b>

Om Planerad intäkt är lika med 0 visas Marginal som 0. </p> </td>
</tr> 
  <tr> 
   <td scope="col"> <p scope="col"><strong>Kolumnrubrik vid visning av intäkter kontra kostnad (faktisk)</strong> </p>  </td> 
   <td scope="col"><p><strong> -funktion</strong></p></td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Faktisk kostnad</strong> </td> 
   <td scope="col"> <p>Den totala faktiska kostnaden för de inkluderade projekten. Du kan visa den totala faktiska kostnaden för den övergripande livscykeln för de inkluderade projekten, eller så kan du bara visa den totala faktiska kostnaden för det angivna datumintervallet (du kan ange en enskild vecka eller månad).</p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Faktisk intäkt</strong> </td> 
   <td> <p>Faktisk intäkt är den intäkt som är associerad med aktiviteternas faktiska timmar.</p> <p>Faktisk intäkt visas i användningsrapporten först när uppgiften har markerats som Fullständig eller Klar (eller en status som motsvarar Fullständig).</p> <p>Hur användningsrapporten beräknar faktisk intäkt för de inkluderade projekten varierar beroende på vilken typ av intäkt som har angetts för uppgiften, enligt beskrivningen i <a href="#track-revenue" class="MCXref xref">Spåra intäkter</a> i den här artikeln. </p> </td> 
  </tr> 
  <tr> 
   <td scope="col"><strong>Marginal</strong> </td> 
   <td> <p>Marginalprocenten beräknas enligt följande:</p> <p>Faktisk omsättning - faktisk kostnad/faktisk intäkt * 100. </p> <p><b>ANMÄRKNING</b>

Om Faktisk omsättning är lika med 0 visas Marginal som 0. </p> </td>
</tr> 
 </tbody> 
</table>

<!--Note from the table from above "Function" header in the middle of the table; right after the "Planned Revenue"/"Margin" definition: 
     <p scope="col" data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This needs to be either split in two tables of formatted differently)</p>
    -->

## Följ upp framsteg, kostnader och intäkter med användningsrapporten {#track-progress-cost-and-revenue-with-the-utilization-report}

Du kan spåra förloppet eller kostnaden för ett projekt, program eller en portfölj.

Du kan visa information om utnyttjanderapporten för en viss vecka eller månad, eller under hela projekttiden.

Så här spårar du förloppet eller kostnaden för ett eller flera projekt med en utnyttjanderapport:

1. Gör något av följande, beroende på om du visar användningsinformation för ett enskilt projekt, flera projekt, ett program eller en portfölj:

   * Så här visar du användningsinformation för ett enskilt projekt:

      1. Gå till ett projekt som du vill visa användningsinformation för och klicka sedan på **Visa mer > Utnyttjande**.
      1. Användningsinformation visas automatiskt när du visar ett enskilt projekt och du behöver inte använda ett filter.\
         Om du vill filtrera användningsrapporten kan du använda ett filter och sedan klicka på **Kör**.\
         Mer information om hur du filtrerar användningsrapporten finns i avsnittet [Information om filteranvändning](#filter-utilization-information) i den här artikeln.\
         Användningsinformation visas för enskilda användare och roller (användarna grupperas i sin associerade roll).

   * Så här visar du användningsinformation för flera projekt:

      1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen.
      1. Tillämpa ett filter på användningsrapporten och klicka sedan på **Kör**.\
         Du måste ange ett eller flera projekt i filtret innan du kör användningsrapporten. Mer information om hur du filtrerar användningsrapporten finns i avsnittet [Information om filteranvändning](#filter-utilization-information) i den här artikeln.\
         Användningsinformation visas för enskilda roller och projekt (roller grupperas i deras associerade projekt).

   * Så här visar du användningsinformation för ett program:

      1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen och klicka på **Visa**>**Program**.
      1. Tillämpa ett filter på användningsrapporten och klicka sedan på **Kör**.\
         Du måste ange ett eller flera program i filtret innan du kör användningsrapporten. Mer information om hur du filtrerar användningsrapporten finns i avsnittet [Information om filteranvändning](#filter-utilization-information) i den här artikeln.\
         Användningsinformation visas för enskilda projekt och program (projekten grupperas inom det tillhörande programmet).

   * Så här visar du användningsinformation för en portfölj:

      1. Klicka på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen och klicka på **Visa**>**Portfolio**.
      1. Tillämpa ett filter på användningsrapporten och klicka sedan på **Kör**.\
         Du måste ange en eller flera portföljer i filtret innan du kör användningsrapporten. Mer information om hur du filtrerar användningsrapporten finns i avsnittet [Information om filteranvändning](#filter-utilization-information) i den här artikeln.\
         Användningsinformation visas för enskilda projekt, program och portföljer (projekten grupperas i respektive tillhörande program och programmen grupperas i respektive associerad portfölj).

1. Klicka på knappen **Visa** och välj sedan något av följande:

   * **Kostnad**
   * **Timmar**
   * **Intäkter**
   * **Intäkter kontra kostnader (planerade)**
   * **Intäkter kontra kostnader (faktisk)**.

   Det alternativ du väljer avgör vilka kolumner och vilken information som är tillgänglig i rapporten. Mer information om den tillgängliga informationen i varje kolumn finns i tabellen i steg 5.\
   ![](assets/utilization-view-dropdown.png)

1. (Valfritt) Välj det datumintervall som utnyttjandeinformationen ska visas för. Du kan visa information för en viss vecka eller månad till vänster om **Övergripande** kolumn. Information om det övergripande projektet, programmet eller portföljen visas alltid i **Övergripande** kolumn.\
   Mer information finns i avsnittet [Justera det datumintervall som information visas för](#adjust-the-date-range-for-which-information-is-displayed) i den här artikeln.

1. (Valfritt) Klicka på en kolumnrubrik om du vill sortera användningsrapporten efter informationen i den kolumnen. Sortering fungerar bara när du inkluderar flera objekt i rapporten. Du kan till exempel sortera resultatet av rapporten när du tittar på mer än ett projekt (eller portfölj eller program). Du kan inte sortera resultaten när du bara tittar på ett projekt (eller en portfölj eller ett program) åt gången.
1. Använd informationen i avsnittet [Översikt över användningsrapporten](#overview-of-the-utilization-report) i den här artikeln om du vill veta mer om varje kolumn i användningsrapporten.

## Information om filteranvändning {#filter-utilization-information}

Du kan filtrera innehållet som visas i en användningsrapport för ett projekt. Du kan filtrera på uppgifter, ärenden, roller och anpassade data. När du tillämpar ett filter på användningsrapporten innehåller användningsrapporten information som baseras på de kriterier du väljer.

Du kan skapa ett filter eller använda ett filter som du har skapat tidigare.

* [Skapa eller ändra ett filter](#create-or-modify-a-filter)
* [Använda ett sparat filter](#apply-a-saved-filter)
* [Duplicera ett filter](#duplicate-a-filter)
* [Byta namn på ett filter](#rename-a-filter)
* [Ta bort ett filter](#delete-a-filter)

### Skapa eller ändra ett filter {#create-or-modify-a-filter}

När du skapar ett filter har alla Workfront-användare som har tillgång till användningsrapporten även tillgång till det filter som du skapar. När du ändrar ett befintligt filter ändras filtret på samma sätt för alla användare som har tillgång till användningsrapporten.

Så här skapar eller ändrar du ett filter:

1. Om du vill filtrera användningsinformation för ett enskilt projekt går du till det projekt som du vill filtrera användningsinformationen för och klickar sedan på **Visa mer>Användning** i den vänstra panelen.

   eller

   Om du vill filtrera användningsinformation för flera projekt, för ett program eller för en portfölj klickar du på ikonen Huvudmeny ![](assets/main-menu-icon.png) i Workfront övre högra hörn, **Resurser**, **Användning** i den vänstra panelen och **Visa**>**Program** eller **Portfolio** eller **Projekt**.

1. Klicka på **Filter** om du vill visa filteralternativen.

1. (Villkorligt) Om du vill ändra ett befintligt filter klickar du på **Filter** och välj sedan det filter som du vill ändra.
1. Ange följande information för att skapa eller ändra filtret:

   * **Portfolio:** Börja skriva namnet på portföljen som innehåller den information du vill inkludera i användningsrapporten och klicka sedan på namnet när det visas i listrutan.\
     Upprepa den här processen om du vill inkludera information från flera portföljer i användningsrapporten.\
     Om du vill inkludera alla portföljer från systemet i filtret klickar du på **Lägg till alla**. (Det här alternativet är endast tillgängligt om du har färre än 10 portföljer i systemet.)

   * **Program:** Börja skriva namnet på programmet som innehåller den information du vill inkludera i användningsrapporten och klicka sedan på namnet när det visas i listrutan.\
     Upprepa den här processen om du vill inkludera information från flera uppgifter i användningsrapporten.\
     Om du redan har definierat några portföljer i filtret måste det program du anger finnas bland de portföljer som redan ingår i filtret. Om så inte är fallet inkluderas inte data från programmet i användningsrapporten.\
     Om du vill inkludera alla program från systemet i filtret klickar du på **Lägg till alla**. (Det här alternativet är bara tillgängligt om du har färre än 20 program i systemet.)

   * **Projekt:** Börja skriva namnet på det projekt som innehåller den information du vill inkludera i användningsrapporten och klicka sedan på namnet när det visas i listrutan.\
     Upprepa den här processen om du vill inkludera information från flera projekt i användningsrapporten.\
     Om du redan har definierat några portföljer eller program i filtret måste projektet du anger finnas i någon av portföljerna eller programmen som redan ingår i filtret. Om så inte är fallet inkluderas inte data från projektet i användningsrapporten.\
     Om du vill inkludera alla projekt från systemet i filtret klickar du på **Lägg till alla**. (Det här alternativet är bara tillgängligt om du har färre än 250 projekt i systemet.)

   * **Uppgifter:** Börja skriva namnet på uppgiften som innehåller den information du vill inkludera i användningsrapporten och klicka sedan på namnet när den visas i listrutan.\
     Upprepa den här processen om du vill inkludera information från flera uppgifter i användningsrapporten.\
     Om du redan har definierat portföljer, program eller projekt i filtret måste den uppgift du anger finnas i någon av portföljerna, programmen eller projekten som redan ingår i filtret. Om så inte är fallet inkluderas inte data från uppgiften i användningsrapporten.

   * **Problem:** Börja skriva namnet på det problem som innehåller den information du vill inkludera i användningsrapporten och klicka sedan på namnet när det visas i listrutan.\
     Upprepa den här processen om du vill inkludera information från flera utgåvor i användningsrapporten.\
     Om du redan har definierat portföljer, program eller projekt i filtret måste den utgåva du anger finnas i någon av portföljerna, programmen eller projekten som redan ingår i filtret. Om så inte är fallet inkluderas inte data från problemet i användningsrapporten.\
     Kostnadsinformation för utleveranser ingår inte alltid i användningsrapporten. Mer information om när kostnadsinformation om problem ingår i användningsrapporten finns i avsnittet [Följ upp framsteg, kostnader och intäkter med användningsrapporten](#track-progress-cost-and-revenue-with-the-utilization-report) i den här artikeln.

   * **Roller:** Börja skriva namnet på den roll du vill ska visas i användningsrapporten och klicka sedan på namnet när det visas i listrutan. Upprepa den här processen om du vill ta med ytterligare roller.\
     Användningsrapporten innehåller endast information om de roller du anger. En uppgift innehåller till exempel 10 faktiska timmar. 6 av dessa timmar kommer från en Designer-roll och 4 är från en Developer-roll. Om du filtrerar användningsrapporten efter roll för Designer tas de fyra timmarna som kommer från utvecklarrollen inte med i rapporten.

   * **Lägg till filterregel:** Klicka **Lägg till filterregel** klickar du i det första fältet och börjar sedan skriva det fältnamn som du vill filtrera på. Om fältet är tillgängligt fylls det i för varje objekt där det kan kopplas. Klicka på fältets namn för att lägga till det i filtret.

     >[!IMPORTANT]
     >
     >Du måste ange fältnamnet och inte fältetiketten. Fältetiketten visas i ett anpassat formulär som är kopplat till ett objekt. Mer information om skillnaden mellan etiketten och namnet på ett anpassat fält finns i  [Skapa eller redigera ett anpassat formulär](../../administration-and-setup/customize-workfront/create-manage-custom-forms/create-or-edit-a-custom-form.md).

     Mer information om fälten som visas i kolumnerna finns i [Ordlista för Adobe Workfront-terminologi](../../workfront-basics/navigate-workfront/workfront-navigation/workfront-terminology-glossary.md).\
     Välj filter och villkorsmodifierare för filtret. Tillgängliga modifierare beskrivs i [Filter- och villkorsmodifierare](../../reports-and-dashboards/reports/reporting-elements/filter-condition-modifiers.md).

1. Om du vill skapa ett nytt filter klickar du på **Spara filter**.\
   eller\
   Om du vill ändra ett befintligt filter klickar du på listrutepilen bredvid **Spara filter** och sedan klicka **Spara nytt filter**.\
   I **Filternamn** fält, ange ett namn för filtret och klicka sedan på **Spara**.\
   Användningsområdet filtreras med den information som finns i filtret.

### Använda ett sparat filter {#apply-a-saved-filter}

1. Om du vill använda ett filter på användningsrapporten för ett enskilt projekt går du till det projekt som du vill filtrera för och klickar sedan på **Visa mer>Användning** i den vänstra panelen.

   eller

   Om du vill använda ett filter på användningsrapporten för flera projekt, för ett program eller för en portfölj klickar du på **Huvudmeny** icon ![](assets/main-menu-icon.png) i Workfront övre högra hörn, **Resurser**, **Användning** i den vänstra panelen och **Visa**>**Program** eller **Portfolio** eller **Projekt**.

1. Klicka **Sparade filter** väljer du sedan det filter som du vill använda i listrutan.

### Duplicera ett filter {#duplicate-a-filter}

1. Om du vill duplicera ett filter i utnyttjanderapporten för ett enskilt projekt går du till det projekt som du vill duplicera filtret för och klickar sedan på **Visa mer>Användning** i den vänstra panelen.

   eller

   Om du vill duplicera ett filter i användningsrapporten för flera projekt, för ett program eller för en portfölj klickar du på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen.

1. Klicka **Sparade filter**, för musen över det filter som du vill duplicera i listrutan och klicka sedan på **Duplicera** ikon.

   ![](assets/utilization-filter-duplicate.png)\
   Dialogrutan Duplicera filter visas.

1. I **Filternamn** anger du ett namn för det nya filtret och klickar sedan på **Spara**.

### Byta namn på ett filter {#rename-a-filter}

När du byter namn på ett filter visas det nya namn du väljer för alla Workfront-användare som har tillgång till användningsrapporten.

Så här byter du namn på ett filter:

1. Om du vill byta namn på ett filter i användningsrapporten för ett enskilt projekt går du till det projekt som du vill byta namn på filtret för och klickar sedan på **Visa mer>Användning** i den vänstra panelen.

   eller

   Om du vill byta namn på ett filter i användningsrapporten för flera projekt, för ett program eller för en portfölj klickar du på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen.

1. Klicka **Sparade filter**, för musen över det filter som du vill duplicera i listrutan och klicka sedan på **Byt namn** ikon.\
   ![](assets/utilization-filter-rename.png)\
   Dialogrutan Byt namn på filter visas.

1. I **Filternamn** anger du ett namn för det nya filtret och klickar sedan på **Spara**.

### Ta bort ett filter {#delete-a-filter}

När du tar bort ett filter tas filtret bort för alla Workfront-användare som har tillgång till användningsrapporten.

Så här tar du bort ett filter:

1. Om du vill ta bort ett filter i användningsrapporten för ett enskilt projekt går du till det projekt som du vill ta bort filtret för och klickar sedan på **Visa mer>Användning** i den vänstra panelen.

   eller

   Klicka på knappen **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen.

1. Klicka **Sparade filter**, för musen över det filter som du vill duplicera i listrutan och klicka sedan på **Ta bort** ikon.

   ![](assets/utilization-filter-delete.png)

1. Klicka **Ta bort** när du får en fråga om du vill ta bort filtret.

## Justera det datumintervall som information visas för {#adjust-the-date-range-for-which-information-is-displayed}

Du kan justera det datumintervall för vilket användningsinformation visas. Du kan välja ett tidigare eller framtida datum. De ändringar du gör visas bara för dig.

1. Om du vill justera datumintervallet för användningsrapporten för ett enskilt projekt går du till det projekt som du vill justera datumintervallet för och klickar sedan på **Visa mer>Användning** i den vänstra panelen.

   eller

   Om du vill justera datumintervallet för användningsrapporten för flera projekt, för ett program eller för en portfölj klickar du på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen.

1. Klicka på datumintervallet bredvid **Exportera** -knappen.

   Den aktuella veckan är markerad som standard.

1. Välj bland följande alternativ:

   * **Vecka:** Välj det här alternativet om du vill välja en viss vecka (från söndag till lördag).
   * **Månad:** Välj det här alternativet om du vill välja en viss månad.

   Datumintervallet du väljer visas i användningsrapporten till vänster om **Övergripande** kolumn.\
   Workfront kommer ihåg om du vill visa en vecka- eller månadsvy. Nästa gång du öppnar utnyttjanderapporten visas den aktuella veckan eller den aktuella månaden, beroende på vilket alternativ du väljer.

## Exportera användningsinformation

Du kan exportera användningsinformation för ett projekt, ett program eller en portfölj från Workfront. Information kan bara exporteras i formaten XLSX, TSV och PDF.

När negativa tal visas i Microsoft Excel visas de inom parentes.

Så här exporterar du användningsinformation:

1. Om du vill exportera användningsinformation för ett enskilt projekt går du till det projekt som du vill exportera användningsinformation för och klickar sedan på **Användning** -fliken (beroende på layoutinställningarna kan den finnas under **Mer** -fliken).

   eller

   Om du vill exportera användningsinformation för flera projekt, för ett program eller för en portfölj klickar du på **Huvudmeny** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **Resurser** sedan **Användning** i den vänstra panelen.

1. Klicka **Exportera**, som finns i det övre vänstra hörnet av **Användning** -fliken.

1. Välj bland följande alternativ:

   * **PDF:** Exporterar rapporten i PDF-format. Det här är det rekommenderade formatet om du tänker skriva ut rapporten.\
     Välj antingen **Letter - stående**, **Letter - liggande**, eller **Andra storlekar** (innehåller alternativ för export i Legal (8,5 x 14 tum), Ledger (11 x 17 tum) och A4).\
     Beroende på vilket operativsystem du använder kan du ha möjlighet att öppna eller spara filen. Öppna filen med det associerade programmet eller spara den på hårddisken.

   * **Excel:** Exporterar rapporten i XLSX-format. Detta är det rekommenderade formatet om du tänker analysera data i Excel ytterligare.\
     Beroende på vilket operativsystem du använder kan du ha möjlighet att öppna eller spara filen. Öppna filen med det associerade programmet eller spara den på hårddisken.

   * **Tabbavgränsad:** Exporterar rapporten i TSV-format. Detta är det rekommenderade formatet om du tänker importera data till tredjepartsprogram för ytterligare analys.\
     Beroende på vilket operativsystem du använder kan du ha möjlighet att öppna eller spara filen. Öppna filen med det associerade programmet eller spara den på hårddisken.

1. Läs informationen i artikeln [Exportera data](../../reports-and-dashboards/reports/creating-and-managing-reports/export-data.md) om du vill veta hur du använder den exporterade filen.

## Visa användningsinformation i ett diagram

Du kan visualisera data från användningsrapporten i en diagramvy.

1. Om du vill visa en användningsrapport för ett enskilt projekt i ett diagramformat går du till det projekt du vill visa och klickar sedan på **Visa mer > Utnyttjande** i den vänstra panelen.

   eller

   Om du vill visa en användningsrapport i ett diagramformat för flera projekt, för ett program eller för en portfölj klickar du på **Rapportering** i det globala navigeringsfältet för att gå till rapportområdet och klicka sedan på **Användning** -fliken.

1. Klicka på knappen **Diagram** ikon.\
   ![](assets/utilization-chart.png)\
   Användningsrapporten visas i en diagramvy.

1. (Valfritt) Konfigurera detta för att visa projekt, program eller Portfolio genom att välja lämpligt alternativ i dialogrutan **Visa** nedrullningsbar meny.
1. (Valfritt) För musen över en viss tidpunkt i rapporten för att visa data för den tidpunkten.

   ![](assets/utilization-chart-hover-350x176.png)

1. (Valfritt) Justera filtren för att bestämma vilken information som visas i diagrammet. Mer information om hur du justerar filtren finns i avsnittet [Information om filteranvändning](#filter-utilization-information) i den här artikeln.
1. (Valfritt) Konfigurera tidsramen för diagramrapporten enligt beskrivningen i avsnittet [Justera det datumintervall som information visas för](#adjust-the-date-range-for-which-information-is-displayed) i den här artikeln.
