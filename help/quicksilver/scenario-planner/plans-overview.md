---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Översikt över planer i scenarioplaneraren
description: Som affärschef kan du använda Adobe Workfront Scenario Planner för att beskriva strategin för din organisations närmaste och långsiktiga framtid genom att beskriva dess ettårsplaner, treårsplaner eller femårsplaner.
author: Alina
feature: Workfront Scenario Planner
exl-id: df2b895b-8bc1-4a55-b0d7-8a06db420315
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1262'
ht-degree: 0%

---

# Planer - översikt i [!DNL Scenario Planner]

The [!DNL Scenario Planner] kräver en separat licens utöver [!DNL Adobe Workfront] licens. Mer information om [!DNL Workfront Scenario Planner], se [The [!DNL Scenario Planner] översikt](../scenario-planner/scenario-planner-overview.md).

Som affärschef kan du använda [!DNL Adobe Workfront Scenario Planner] för att beskriva strategin för er framtida framtid på kort och lång sikt genom att beskriva sina ettårsplaner, treårsplaner eller femårsplaner.

## Åtkomstkrav

Så här använder du [!DNL Adobe Workfront Scenario Planner] du måste ha följande åtkomst:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p><a href="https://www.workfront.com/plans" target="_blank">[!DNL Adobe Workfront] plan</a>*</p> </td> 
   <td>[!UICONTROL Business] eller högre</td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p>Licenstyp*</p> </td> 
   <td> <p>[!UICONTROL Review] eller senare. Mer information finns i <a href="../administration-and-setup/add-users/access-levels-and-object-permissions/wf-licenses.md" class="MCXref xref">[!DNL Adobe Workfront] licensöversikt</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du får [!DNL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader">Åtkomstnivå*</td> 
   <td> <p>[!UICONTROL View] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Information om hur en Workfront-administratör kan ändra åtkomstnivån finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td role="rowheader"> <p>Objektbehörigheter</p> </td> 
   <td> <p>[!UICONTROL View] behörigheter eller högre för en plan<!--
      <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
        (NOTE: this might change if they have permissions for initiatives/ scenarios, etc) 
      </MadCap:conditionalText>
     --></p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta [!DNL Workfront] administratör.

## Planer - översikt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add information about utilization percentage for job roles - per this story?? - https://hub.workfront.com/task/5eb0784900083e1f2cabb60d6e0d04d3/overview)</p>
-->

Du kan identifiera varje resultat för en högnivåorganisation och lägga till det som en plan i [!DNL Workfront Scenario Planner]. En plan är den största arbetsposten i [!DNL Scenario Planner]. För att göra det enklare att genomföra planen kan du dela upp den i flera initiativ och ange vilka steg enskilda organisationsenheter måste ta för att slutföra planen.

Sedan kan ni koppla initiativ till verkliga projekt för att visa hur verkliga arbetsfaktorer faktiskt fullbordar planen. Den här artikeln innehåller allmän information om planer. Mer information om initiativ finns i [Översikt över initiativen i [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

Du kan definiera de arbetsresurser och ekonomiska resurser som behövs för att slutföra arbetet som identifieras i planen. Ni kan också se vilka arbetsresurser och ekonomiska resurser som krävs för att initiativen i planen ska kunna slutföras.

Du kan beräkna och granska följande information för varje plan:

* Uppskatta typen och antalet jobbroller som är tillgängliga för att genomföra planen.
* Beräkna den budget ditt företag behöver för att slutföra planen.
* Granska utnyttjandeprocenten för varje jobbroll mot de obligatoriska jobbrollerna som är kopplade till initiativen.
* Granska utnyttjandeprocenten för din plans budget mot kostnaderna för initiativen.
* Granska planens nettovärde vid en given tidpunkt.
* Information på plannivå ändras när du väljer olika scenarier. Varje scenario har olika budget- och personinformation.

Mer information om att skapa planer finns i artikeln [Skapa och redigera planer i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Mer information om att skapa scenarier finns i [Skapa och jämföra planscenarier i [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

## Överväganden om planer

Tänk på följande när du skapar planer:

* Du kan skapa planer för ett team, en hel avdelning eller till och med hela företaget. Planer är stora planeringsenheter som skisserar ett företags strategi på hög nivå.
* Den kortaste planen kan ha en varaktighet på ett år. Den längsta planen kan ha en varaktighet på 5 år.
* Du kan inte utföra verkligt arbete på en plan. Du kan grovt uppskatta om du har de resurser och den budget som krävs för att starta planeringsarbetet. Om ditt företag till exempel vill expandera och förvärva ett nytt kontor på en ny plats, måste du vidta de åtgärder som kan anges först i en plan på den övre ledningsnivån.
* Du kan skapa flera scenarier för samma plan. När din ursprungliga plan innehåller för många motstridiga initiativ vill du skapa flera scenarier där du kan redigera initiativ eller budgetar och kostnader för att se vad som är den idealiska situationen för att genomföra planen. Initiativ kan vara i konflikt med varandra när de försöker använda samma resurser under samma tidsperiod. Du kan sedan jämföra scenarier för att se vad som är mest meningsfullt och vilket som ska användas av företaget innan de börjar lägga till det verkliga arbetet för att uppnå det. Mer information om att skapa scenarier finns i artikeln [Skapa och jämföra planscenarier i [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
* Du kan lägga till flera initiativ i en plan för att ange hur mindre planeringsenheter kommer att bidra till att planen slutförs. Om du t.ex. planerar att expandera till en viss marknad kan du ha flera initiativ på avdelningsnivå som i slutänden bidrar till att expandera på alla nivåer i organisationen. Mer information om hur du skapar initiativ finns i artikeln [Skapa och redigera i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).
* När du skapar en plan är du den enda personen som kan visa den. Du måste ha kontakt med andra användare och de kan komma åt planen om de har minst Visa åtkomst till [!DNL Scenario Planner] på deras åtkomstnivå.

## Jobbrollsinformation för planer

Du kan granska allmän information om jobbroller för planer som anger antalet lediga roller som är tillgängliga för planen samt mängden jobbroller som krävs för att initiativen ska slutföras. Du kan visa den här informationen i [!UICONTROL Job Roles] i planens sidhuvud.

![](assets/job-role-box-on-plan-not-expanded-fte-350x141.png)

Du kan visa följande i rutan Jobbroll:

| Information | Beskrivning |
|---|---|
| Indikator för heltidsekvivalenter/timmar | The ([!UICONTROL FTE]) eller ([!UICONTROL Hours]) bredvid indikatorn &quot;[!UICONTROL Job Role]&quot; anger om planen var konfigurerad att använda FTE eller Timmar när den skapades. Planen, alla scenarier och initiativ använder den här enheten. |
| [!UICONTROL Available] | Antalet FTE eller timmar för jobbroll som är tillgängliga för det aktuella scenariot. |
| Obligatoriskt | Antal heltidsanställda eller timmar för jobbroller som krävs för alla initiativ i det aktuella scenariot så att de kan slutföras. |

Mer information om hur du får åtkomst till en plan och visar detaljerad information om jobbroller finns i [Skapa och redigera planer i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Finansiell information om planer

Du kan granska ekonomisk information om en plan, särskilt dess planerade budget, hur den budgeten används och vad planens nettovärde är. Nettovärdet för en plan baseras på nettovärdet av dess initiativ. Du kan visa den här informationen i [!UICONTROL Financial] och [!UICONTROL Summary] i planens sidhuvud.

![](assets/budget-net-value-boxes-on-plan-not-expanded-350x86.png)

Du kan visa följande i [!UICONTROL Financial] och [!UICONTROL Summary] i planen:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Budget] </p> <p role="rowheader"> </p> </td> 
   <td>Det här är det penningbelopp som ditt företag fastställer och som är tillgängligt för att genomföra planen. Workfront fördelar budgeten jämnt för varje månad under perioden. Budgetar är vanligtvis inställda för ett år, men kan också fastställas för en 3- eller 5-årsperiod. Valutan inom parenteserna till vänster om rubriken för den finansiella lådan anger systemets valuta. </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!UICONTROL Costs]</td> 
   <td> <p>Detta är den totala kostnaden för alla initiativ i planen. Workfront beräknar kostnaderna för planen enligt följande formel:</p> <p><code>Plan Costs = SUM(Initiative Costs)</code> </p> <p>Mer information om hur initialkostnader beräknas finns i <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Skapa och redigera i [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">UTIL (budgetutnyttjandeprocent)</td> 
   <td> <p>Detta är en beräknad procentandel mellan kostnaderna i samband med initiativ och den budget som definierats för planen. </p> <p>[!DNL Workfront] beräknar budgetutnyttjandeprocenten för en plan med följande formel: </p> <p><code>Utilization percentage = (Plan Costs* 100))/ Plan Budget</code> </p> <p>Kostnaderna beräknas med följande formel:</p> <p><code>Plan Costs = SUM(Initiatives People Costs, Initiatives Fixed Costs)</code> </p> <p>Tips: Användningsprocenten är avrundad och har en decimal. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Net Value] area <span>i [!UICONTROL Summary] box</span></p> <p role="rowheader"> </p> </td> 
   <td> <p>Detta är en beräkning av alla nettovärden för alla initiativ i planen. </p> <p>Workfront beräknar nettovärdet för planen enligt följande formel: </p> <p><code>Plan Net Value = SUM(Initiative Planned Benefit - People Costs)</code> </p> <p>eller</p> <p><code>Plan Net Value = SUM(Initiative Net Value)</code> </p> <p>Mer information om de initiativa nettovärdena finns i artikeln <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Översikt över initiativen i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om hur du får tillgång till en plan och visar detaljerad ekonomisk information om den finns i [Skapa och redigera planer i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).


