---
content-type: overview
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Översikt över planer i scenarioplaneraren
description: Som affärschef kan du använda Adobe Workfront Scenario Planner för att beskriva strategin för din organisations närmaste och långsiktiga framtid genom att beskriva dess ettårsplaner, treårsplaner eller femårsplaner.
author: Alina
feature: Workfront Scenario Planner
exl-id: df2b895b-8bc1-4a55-b0d7-8a06db420315
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '1140'
ht-degree: 0%

---

# Översikt över planer i [!DNL Scenario Planner]

Som affärschef kan du använda [!DNL Adobe Workfront Scenario Planner] för att beskriva strategin för din organisations närmaste och långsiktiga framtid genom att beskriva dess ettåriga, tre eller fem årsplaner.

## Åtkomstkrav

Mer information om åtkomstkrav för att komma åt scenarioplaneraren finns i [Åtkomst krävs för att använda scenarioplaneraren](/help/quicksilver/scenario-planner/access-needed-to-use-sp.md).

## Planer - översikt

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: add information about utilization percentage for job roles - per this story?? - https://hub.workfront.com/task/5eb0784900083e1f2cabb60d6e0d04d3/overview)</p>
-->

Du kan identifiera varje resultat för en högnivåorganisation och lägga till det som en plan i [!DNL Workfront Scenario Planner]. En plan är den största arbetsposten i [!DNL Scenario Planner]. För att göra det enklare att genomföra planen kan du dela upp den i flera initiativ och ange vilka steg enskilda organisationsenheter måste ta för att slutföra planen.

Sedan kan ni koppla initiativ till verkliga projekt för att visa hur verkliga arbetsfaktorer faktiskt fullbordar planen. Den här artikeln innehåller allmän information om planer. Mer information om initiativ finns i [Översikt över initiativ i  [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

Du kan definiera de arbetsresurser och ekonomiska resurser som behövs för att slutföra arbetet som identifieras i planen. Ni kan också se vilka arbetsresurser och ekonomiska resurser som krävs för att initiativen i planen ska kunna slutföras.

Du kan beräkna och granska följande information för varje plan:

* Uppskatta typen och antalet jobbroller som är tillgängliga för att genomföra planen.
* Beräkna den budget ditt företag behöver för att slutföra planen.
* Granska utnyttjandeprocenten för varje jobbroll mot de obligatoriska jobbrollerna som är kopplade till initiativen.
* Granska utnyttjandeprocenten för din plans budget mot kostnaderna för initiativen.
* Granska planens nettovärde vid en given tidpunkt.
* Information på plannivå ändras när du väljer olika scenarier. Varje scenario har olika budget- och personinformation.

Mer information om hur du skapar planer finns i artikeln [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Mer information om att skapa scenarier finns i [Skapa och jämföra planscenarier i  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

## Överväganden om planer

Tänk på följande när du skapar planer:

* Du kan skapa planer för ett team, en hel avdelning eller till och med hela företaget. Planer är stora planeringsenheter som skisserar ett företags strategi på hög nivå.
* Den kortaste planen kan ha en varaktighet på ett år. Den längsta planen kan ha en varaktighet på 5 år.
* Du kan inte utföra verkligt arbete på en plan. Du kan grovt uppskatta om du har de resurser och den budget som krävs för att starta planeringsarbetet. Om ditt företag till exempel vill expandera och förvärva ett nytt kontor på en ny plats, måste du vidta de åtgärder som kan anges först i en plan på den övre ledningsnivån.
* Du kan skapa flera scenarier för samma plan. När din ursprungliga plan innehåller för många motstridiga initiativ vill du skapa flera scenarier där du kan redigera initiativ eller budgetar och kostnader för att se vad som är den idealiska situationen för att genomföra planen. Initiativ kan vara i konflikt med varandra när de försöker använda samma resurser under samma tidsperiod. Du kan sedan jämföra scenarier för att se vad som är mest meningsfullt och vilket som ska användas av företaget innan de börjar lägga till det verkliga arbetet för att uppnå det. Mer information om hur du skapar scenarier finns i artikeln [Skapa och jämföra planscenarier i  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
* Du kan lägga till flera initiativ i en plan för att ange hur mindre planeringsenheter kommer att bidra till att planen slutförs. Om du t.ex. planerar att expandera till en viss marknad kan du ha flera initiativ på avdelningsnivå som i slutänden bidrar till att expandera på alla nivåer i organisationen. Mer information om hur du skapar initiativ finns i artikeln [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).
* När du skapar en plan är du den enda personen som kan visa den. Du måste ansluta till planen med andra användare och de kan komma åt den om de har minst Visa åtkomst till [!DNL Scenario Planner] på åtkomstnivån.

## Jobbrollsinformation för planer

Du kan granska allmän information om jobbroller för planer som anger antalet lediga roller som är tillgängliga för planen samt mängden jobbroller som krävs för att initiativen ska slutföras. Du kan visa den här informationen i rutan [!UICONTROL Job Roles] i planens huvud.

![Jobbrollruta i plan](assets/job-role-box-on-plan-not-expanded-fte-350x141.png)

Du kan visa följande i rutan Jobbroll:

| Information | Beskrivning |
|---|---|
| Indikator för heltidsekvivalenter/timmar | Indikatorn ([!UICONTROL FTE]) eller ([!UICONTROL Hours]) bredvid titeln [!UICONTROL Job Role] anger om planen var konfigurerad att använda FTE eller timmar när den skapades. Planen, alla scenarier och initiativ använder den här enheten. |
| [!UICONTROL Available] | Antalet FTE eller timmar för jobbroll som är tillgängliga för det aktuella scenariot. |
| Obligatoriskt | Antal heltidsanställda eller timmar för jobbroller som krävs för alla initiativ i det aktuella scenariot så att de kan slutföras. |

Mer information om hur du får åtkomst till en plan och visar detaljerad information om jobbroller finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Finansiell information om planer

Du kan granska ekonomisk information om en plan, särskilt dess planerade budget, hur den budgeten används och vad planens nettovärde är. Nettovärdet för en plan baseras på nettovärdet av dess initiativ. Du kan visa den här informationen i rutorna [!UICONTROL Financial] och [!UICONTROL Summary] i planens sidhuvud.

![Rutor för budget och nettovärde](assets/budget-net-value-boxes-on-plan-not-expanded-350x86.png)

Du kan visa följande i rutorna [!UICONTROL Financial] och [!UICONTROL Summary] i planen:

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
   <td> <p>Detta är den totala kostnaden för alla initiativ i planen. Workfront beräknar kostnaderna för planen enligt följande formel:</p> <p><code>Plan Costs = SUM(Initiative Costs)</code> </p> <p>Mer information om hur initialkostnader beräknas finns i <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Skapa och redigera initiativ i [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">UTIL (budgetutnyttjandeprocent)</td> 
   <td> <p>Detta är en beräknad procentandel mellan kostnaderna i samband med initiativ och den budget som definierats för planen. </p> <p>[!DNL Workfront] beräknar budgetutnyttjandeprocenten för en plan med hjälp av följande formel: </p> <p><code>Utilization percentage = (Plan Costs* 100))/ Plan Budget</code> </p> <p>Kostnaderna beräknas med följande formel:</p> <p><code>Plan Costs = SUM(Initiatives People Costs, Initiatives Fixed Costs)</code> </p> <p>Tips! Procentsatsen för användning är avrundad och har en decimal. </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader"> <p role="rowheader">[!UICONTROL Net Value] området <span>i [!UICONTROL Summary]-rutan</span></p> <p role="rowheader"> </p> </td> 
   <td> <p>Detta är en beräkning av alla nettovärden för alla initiativ i planen. </p> <p>Workfront beräknar nettovärdet för planen enligt följande formel: </p> <p><code>Plan Net Value = SUM(Initiative Planned Benefit - People Costs)</code> </p> <p>eller</p> <p><code>Plan Net Value = SUM(Initiative Net Value)</code> </p> <p>Mer information om de initiativa nettovärdena finns i artikeln <a href="../scenario-planner/initiatives-overview.md" class="MCXref xref">Översikt över initiativen i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om hur du får tillgång till en plan och visar detaljerad ekonomisk information om den finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).


