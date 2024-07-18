---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Översikt över initiativ i scenarioplaneraren
description: Scenarioplaneraren finns endast i den nya Adobe Workfront-upplevelsen och kräver ytterligare en licens. Mer information om Workfront Scenarioplan finns i Översikt över scenarioplanen.
author: Alina
feature: Workfront Scenario Planner
exl-id: d67f51e5-7c5c-436b-b0c3-e5afbd7cebca
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '934'
ht-degree: 0%

---

# Initiativöversikt i [!DNL Scenario Planner]

[!DNL Scenario Planner] är bara tillgängligt i den nya [!DNL Adobe Workfront]-upplevelsen och kräver ytterligare en licens. Mer information om [!DNL Workfront Scenario Planner] finns i [Översikt [!DNL Scenario Planner] Översikt](../scenario-planner/scenario-planner-overview.md).
Som affärschef kan du skapa initiativ för planer i [!DNL Adobe Workfront Scenario Planner]. Mer information om hur du skapar planer finns i artikeln [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Översikt över initiativ

Med hjälp av [!DNL Workfront Scenario Planner] kan du beräkna och granska följande information för varje initiativ:

* Uppskatta vilken typ och hur många roller som kan behövas för att slutföra initiativet. Detta ökar antalet obligatoriska arbetsuppgifter för planen samt beräknar de personkostnader som du kan granska för ett initiativ.
* Uppskatta de fasta kostnaderna i samband med det arbete som krävs för att slutföra projektet.
* Uppskatta den planerade förmån som företaget kan få när projektet är slutfört.

Om du vill visa information om dina initiativ kan du komma åt enskilda initiativ inom en plan. Mer information om att skapa och komma åt initiativ finns i artikeln [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

## Överväganden om initiativ

Tänk på följande när du skapar initiativ:

* Du måste skapa en plan innan du kan skapa ett initiativ.
* Du kan skapa initiativ från grunden eller importera projekt till en plan. Projekten blir initiativ inom planen.

  Mer information om att skapa initiativ från grunden finns i [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

  Mer information om hur du importerar projekt till en plan för att skapa initiativ från projekt finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Initiativen är mindre planeringsenheter än planer och de skapas endast som en del av en plan.
* Det kortaste initiativet kan ha en varaktighet på en månad. Det längsta initiativet kan ha en varaktighet på fem år.
* Du kan inte utföra verkligt arbete på ett initiativ. På initiativnivå kan ni definiera vilka resurser som behövs och vilka kostnader dessa resurser kommer att medföra, så att ni kan börja genomföra ett av kraven i planen. Om ditt företag till exempel har en plan för att expandera och förvärva ett nytt kontor på en ny plats, kan din avdelning ha ett initiativ för att installera nätverksinfrastrukturen för den nya platsen.
* Du kan skapa flera initiativ i en plan. Med varje initiativ kan ni utforma en strategi på hög nivå för att uppnå arbetet på avdelningen.
* Ni kan prioritera initiativ inom en plan för att se till att det viktigaste initiativet får mest budget och mest resurser.
* När du skapar initiativ i en plan kan alla som ser den planen också se alla initiativ i planen.

  <!--
  <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: this might change when we add to the access levels granularity)</p>
  -->

* Du kan publicera initiativ för att skapa projekt eller för att uppdatera projekt som är länkade till dem. Mer information om publiceringsinitiativ finns i [Uppdatera eller skapa projekt genom att publicera initiativen i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).

## Finansiell information om initiativ

Du kan granska ekonomisk information om enskilda initiativ för att förstå hur initiativen passar in i planen. Mer information om hur du kommer åt ett initiativ finns i artikeln [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

Följande ekonomiska indikatorer för ett initiativ kan visas i en plan:

<!--
<p>(NOTE: several instances drafted in the table below!) </p>
-->

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs total amount]</td> 
   <td> <p style="font-weight: normal;">Detta är en beräkning av den totala kostnaden för ett initiativ. </p> <p style="font-weight: normal;">[!DNL Workfront] Beräknar det totala kostnadsvärdet för ett initiativ med hjälp av följande formel:</p> <p style="font-weight: normal;"><code>Initiative Costs = Fixed Costs + People Costs</code> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Fixed Costs]</td> 
   <td> <p><span style="font-weight: normal;">Det här är en manuell inmatning där du kan beräkna <span>en månadskostnad för fasta kostnader för varje månad i initiativet.</span> Detta inkluderar inte kostnaderna som är associerade med rollerna som lagts till i initiativet som fångas in i fältet [!UICONTROL People Cost].</span> </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL People Costs]</td> 
   <td> <p style="font-weight: normal;">Detta är en total beräkning av kostnaderna i samband med arbetsrollerna för initiativet under hela dess löptid. Antalet beror på hur många heltidsanställda eller timmar du uppskattar för en jobbroll för varje månad i initiativet. </p> 
     <p><b>TIPS</b>  
     <ul> 
      <li> <p>Antalet heltidsekvivalenter per månad för samma jobbroll kan skilja sig från månad till månad.</p> </li> 
      <li> <p>[!DNL Workfront] Parlamentet anser att det finns 160 arbetstimmar på en månad. </p> </li> 
     </ul> 
     <p>[!DNL Workfront] beräknar [!UICONTROL People Costs] för ett initiativ med följande formel:</p> <p><code>Initiative People Costs = SUM(Monthly people cost)</code> </p> 
    <p> [!DNL Workfront] beräknar de månatliga personkostnaderna för varje månad under initieringens varaktighet med följande formel:</p> 
     <p><code>Monthly People Costs = SUM(Job role hourly rate * 160 * Number of FTEs)</code> </p> 
      <p><b>EXEMPEL</b></p>
      <p>Om du har ett projekt med en varaktighet på sex månader som kräver 1 Designer med en timtaxa på 50 USD per månad och en Web Designer med en timtaxa på 100 USD under två månader av initiativet, beräknas startkostnaderna enligt följande:</p>
      <code>Initiative People Costs = 50*160*6 + 100*160*2 = 48,000 + 32,000 = 80,000</code>        
  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Planned Benefit]</td> 
   <td>Det här är ett manuellt tävlingsbidrag där du kan uppskatta den totala fördel som din avdelning skulle få genom att slutföra det här initiativet. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Net Value amount]</td> 
   <td> <p style="font-weight: normal;">Detta representerar värdet av ert initiativ när ni tar hänsyn till de totala kostnaderna och den planerade förmånen som beräknas på initiativet. [!DNL Workfront] beräknar nettovärdet för ett initiativ med följande formel:</p> <p style="font-weight: normal;"><code>Initiative Net Value = Initiative Planned Benefit - Initiative Costs</code> </p> </td> 
  </tr> 
 </tbody> 
</table>

<!--drafted content from People Costs:
(NOTE: drafted below)</p> 
       <p>Depending on whether the plan is set up to use FTEs or hours, Workfront uses the following formulas to calculate People Cost:</p> 
       <ul> 
        <li> <p>When using FTEs: </p> <p><code>People Costs = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, where 160 is the total number of working hours in a month. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Example: </b></span></span><span style="font-weight: normal;"> When estimating resources using FTEs,(NOTE: drafted and yellow and fix the rest of the sentence)
      <p>When using hours:</p> 
      <p><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> 
      <p>For information about setting up the plan to use hours or FTE, see <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Create and edit plans in the Scenario Planner</a>.</p>-->

## Initiativinformation i rapporter

Du kan visa initialinformation i rapporter enligt tabellen nedan. Den här informationen är endast tillgänglig i din Workfront-instans när ditt företag har köpt en licens för Workfront Scenario Planner.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td><b>Typ av rapportering</b></td> 
   <td><b>Initiativinformation</b></td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative] </td> 
   <td>Namn, Varaktighet, Start- och slutdatum, Inloggad av, ID, Senast publicerad*, Alla projektfält inklusive anpassade fält*</td> 
  </tr> 
  <tr> 
   <td>[!UICONTROL Initiative Job Role]</td> 
   <td>All initieringsinformation som anges ovan, (Jobbroll) ID, Projekt*, Planerade timmar för projekttilldelning*, Antal jobbroller, Alla projektfält inklusive anpassade fält*</td> 
  </tr> 
  <tr> 
   <td><p>[!UICONTROL Project]*</p></td> 
   <td> <p>All information om initiativet enligt ovan*</p> </td> 
  </tr> 
 </tbody> 
</table>

*Dessa fält innehåller information från det projekt som är kopplat till initiativet, endast när projektet skapades från ett projekt eller publicerades till ett projekt minst en gång. Mer information om publiceringsinitiativ finns i [Uppdatera eller skapa projekt genom att publicera initiativen i  [!DNL Scenario Planner]](../scenario-planner/publish-scenarios-update-projects.md).
