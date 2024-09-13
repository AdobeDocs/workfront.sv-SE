---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Lös initialkonflikter i scenarioplanen
description: När satsningarna hamnar i konflikt med varandra konkurrerar de om samma resurser. Resurserna som är tillgängliga för ett scenario räcker inte till för att täcka alla resurser som krävs för alla initiativ i scenariot.
author: Alina
feature: Workfront Scenario Planner
exl-id: d3a3e177-bece-4e03-89d7-9cee6127bc55
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '2071'
ht-degree: 0%

---

# Lös initialkonflikter i [!DNL Scenario Planner]

När satsningarna hamnar i konflikt med varandra konkurrerar de om samma resurser. Resurserna som är tillgängliga för ett scenario räcker inte till för att täcka alla resurser som krävs för alla initiativ i scenariot.

Detta kan inträffa i följande fall:

* Antalet arbetsroller som krävs för initiativet är större än antalet roller som har budgeterats för planen.
* Kostnaderna för initiativet är större än det tillgängliga budgetbeloppet för planen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>Nytt: Ultimate </p></li>
   <p>Scenarioplanen är inte tillgänglig för de nya Workfront Select- eller Workfront Prime-planerna. </p>
   <li><p>Aktuell: [!UICONTROL Business] eller högre</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens*</p> </td> 
   <td> <p>Nytt: Ljus eller högre</p> 
   <p>Aktuell: [!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> <ul><li><p>För nya Workfront-planer:</p><p> Adobe Workfront</li></p>
   <li><p>För nuvarande Workfront-planer: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>

<p>Mer information finns i <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Åtkomstnivå </td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Översikt över att lösa konflikter

* En konflikt tolkas också som en överallokering av jobbrollerna eller budgeten för ett scenario.
* När [!DNL Workfront] upptäcker en konflikt visas fältet som motsvarar den konfliktskapande månaden under initieringens varaktighet i rött. Detta kan inträffa i följande fall:

   * Antalet jobbroller som krävs varje månad för ett initiativ är större än antalet roller som har budgeterats för planen efter att alla tidigare initiativ har använt de resurser som har budgeterats för planen.
   * Månadskostnaderna för initiativet är större än den tillgängliga budgeten för planen efter att alla tidigare initiativ har använt programmets budget för att täcka sina kostnader.

>[!TIP]
>
>Som standard antar [!DNL Scenario Planner] att du har budgeterat för 0 jobbroller och $0 eller motsvarande $0 i systemets valuta för ett scenario, om du inte har angett något annat. Antalet jobbroller anger antalet heltidsanställda (heltidsmotsvarigheter) eller timmar som budgeterats för jobbrollen.
>
>För alla beräkningar i Scenarioplaneraren använder Workfront följande värde: 1 FTE = 8 timmar.
>
>Mer information om hur du uppdaterar tillgängliga roller för en plan och en budget finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

* Du kan lösa en konflikt genom att göra något av följande:

   * Lägga till de saknade nödvändiga resurserna automatiskt från satsningarna i scenariot. I den här artikeln beskrivs hur du löser konflikter med det här alternativet.
   * Justera jobbrollen och budgetresurserna för scenariot genom att redigera planen. Mer information finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

## Lös konflikter mellan initiativ

1. Gå till en plan som du vill lösa konflikter för.

   Mer information om hur du skapar planer finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

   Mer information om hur du skapar initiativ finns i [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Valfritt) Välj det scenario som du vill granska i listrutan **[!DNL Initial scenario]**.

   >[!TIP]
   >
   >En plan kan ha flera scenarier. När du tittar på planens konflikter refererar [!DNL Workfront] till de resurser som är tillgängliga för det valda scenariot och de som krävs för det scenariots initiativ. Mer information om scenarier finns i [Skapa och jämföra planscenarier i  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. Kontrollera att **[!UICONTROL Show conflicts]** är aktiverat. Den är aktiverad som standard.

   ![](assets/show-scenarios-toggle-on.png)

   I det första motstridiga initiativet visas de månader som har röda konflikter och en varningsikon visas bredvid initieringsnamnet.

   Bakgrunden till alla initiativ som börjar med den första motstridiga visas i rött i planens diagram.

   När en konflikt uppstår i ett projekt innebär det att antalet jobbroller för minst en specifik roll, de kostnader som uppstått eller båda överstiger antalet jobbroller eller den budget som definierats för planen för en viss månad.

   ![](assets/initiatives-on-plan-with-conflicts-350x126.png)

1. Gör något av följande om du vill veta mer om de konflikter som kan uppstå:

   * Håll muspekaren över varningsikonen bredvid initialnamnet för att se om du har en jobbroll eller en budgetkonflikt.

     ![](assets/budget-job-role-conflict-tooltip-on-warning-icon-350x109.png)

     Beroende på om du har övertilldelat roller eller överskattat kostnaderna för ditt initiativ kan du se något av följande alternativ när du håller pekaren över varningsikonen:

      * Visa information om jobbrollskonflikter
      * Visa detaljer om budgetkonflikt
      * Visa jobbroll och budgetinformation

   * När du visar planen per månad håller du över en månad i tidslinjen för planen för att visa de resurser som krävs för den månaden och om månadskonflikterna är människor eller kostnadsrelaterade.

     ![](assets/details-of-conflicts-on-monthly-plan-timeline-pop-up-350x178.png)

     Granska följande månadsinformation på plannivå:

      * Antalet tillgängliga, obligatoriska och överallokerade jobbroller för månaden för alla initiativ som planeras för den månaden
      * Tillgängliga, nödvändiga och överfördelade kostnader för månaden för alla planerade initiativ för den månaden

        >[!TIP]
        >
        >Kostnaderna för [!UICONTROL Available] är scenariots budget för den månaden.

   * Håll muspekaren över ett dokuments röda fält i en månad för att visa ytterligare informationsruta om konflikten som inträffar den månaden.

     ![](assets/details-of-conflicts-on-initiative-timeline-pop-up-350x113.png)

     Granska följande fält i den extra informationsrutan på initialnivå:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader">Månad när konflikten inträffar</td> 
        <td>Visar i rubriken för den extra informationsrutan.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">Initiativets namn</td> 
        <td>Visar i rubriken för den extra informationsrutan.</td> 
       </tr> 
       <tr> 
        <td role="rowheader">[!UICONTROL Job Roles]</td> 
        <td> <p>De jobbroller som är associerade med det här initiativet och som har övertilldelats för den valda månaden. I följande kolumner visas information för varje jobbroll som krävs för den valda månaden och som står i konflikt med antalet jobbroller som är tillgängliga för den månaden:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: Antalet tillgängliga jobbroller från scenariot för den valda månaden.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: Antalet arbetsroller som krävs för initiativet för den valda månaden.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> Skillnaden mellan det antal som krävs för initiativet och det antal som är tillgängligt från scenariot. </p> </li> 
         </ul> <p>Tips! Ibland matchar eller är antalet [!UICONTROL Available]-roller högre än antalet [!UICONTROL Required]-roller, men [!DNL Scenario Planner] visar fortfarande en överallokering. Det innebär att det finns högre rankningsinitiativ som redan har använt de jobbroller som är tillgängliga i planen för samma månad. </p> </td> 
       </tr> 
       <tr> 
        <td role="rowheader">Kostnader</td> 
        <td> <p>Initiativets kostnader för den valda månaden. I följande kolumner visas information om vilka kostnader som krävs och vilken budget som är tillgänglig för den valda månaden:</p> 
         <ul> 
          <li> <p><strong>[!UICONTROL Available]</strong>: Budgeten som är tillgänglig från planen för den valda månaden.</p> </li> 
          <li> <p><strong>[!UICONTROL Required]</strong>: Kostnaderna för det här initiativet för den valda månaden.</p> </li> 
          <li> <p style="font-weight: normal;"><strong>[!UICONTROL Overallocated]:</strong> Skillnaden mellan initialkostnaderna och den tillgängliga budgeten från planen. </p> </li> 
         </ul> <p>Tips! Ibland matchar kostnaderna för [!UICONTROL Available] eller är högre än initialkostnaden för [!UICONTROL Required] för den valda månaden och [!DNL Scenario Planner] visar fortfarande en överbeläggning av kostnaden. Det innebär att det finns större initiativ som redan använder den tillgängliga budgeten för planen för samma månad. </p> </td> 
       </tr> 
      </tbody> 
     </table>

1. Gör något av följande för att öppna panelen med information om initiativ och visa mer information om var konflikterna inträffar och för att lösa dem:

   * Klicka på varningsikonen bredvid initieringens namn.
   * Klicka på ett initiativ.
   * Klicka på ikonen **[!UICONTROL More]** ![](assets/more-icon.png) till höger om initieringens namn och klicka sedan på **[!UICONTROL Edit]**.

     Panelen Initiativinformation visas till höger.

     Om du inte har tillräckligt med personal eller budget för ditt initiativ visas en röd varningsikon bredvid följande avsnitt:

   * [!UICONTROL Required Job Roles]
   * [!UICONTROL Costs]

1. (Villkorligt) För initiativ som har jobbrollskonflikter går du till avsnittet **[!UICONTROL Required Job Roles]** för att visa alla jobbroller som krävs för ditt initiativ. Identifiera vilka jobbroller som kan bli överallokerade. Granska antalet heltidsanställda eller timmar som behövs för varje jobbroll för varje månad i initiativet. Rutan med antalet heltidsanställda eller timmar för månader med överbeläggningar visas i en röd ram.

   ![](assets/details-panel-overallocated-roles-350x275.png)

1. (Valfritt) Klicka på högerpilen bredvid månaderna på initieringens tidslinje för att se vilka ytterligare månader som står i konflikt med jobbrollerna.

   ![](assets/right-arrow-initiative-months-inside-details-box-highlighted-350x145.png)

1. (Valfritt) Klicka på **[!UICONTROL Show details]** under jobbrollen som visar en konflikt för att se var konflikterna förekommer och för att markera de månader som står i konflikt i planens diagramområde. Ytterligare information visas för varje jobbroll.

   Följande fält visas för varje jobbroll:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Antalet jobbroller som är tillgängliga från planen för varje månad. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>Antalet jobbroller som redan har tilldelats från planens budget till initiativ med högre rankning för en viss månad. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>Skillnaden mellan antalet obligatoriska jobbroller i initiativet och antalet tillgängliga från planen efter högre rankningsinitiativ har också utnyttjat vissa av rollerna. Workfront beräknar antalet [!UICONTROL Overallocated] jobbroller med följande formel:</p> <p><code>Overallocated roles = (Roles Previously Allocated to higher initiatives + Required roles for current initiative) - Monthly available roles from the plan</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >I planens diagram visar de månader där jobbrollerna fördelas namn och antal roller som behövs för varje initiativ där de behövs. Du måste välja vyn [!UICONTROL Month] för att kunna se namnet på jobbrollerna

   ![](assets/conflicting-job-role-months-on-plan-after-clicking-show-details-350x158.png)

1. Gör något av följande för att lösa jobbrollskonflikter:

   * Justera manuellt antalet jobbroller för varje månad i initiativet till ett lägre antal.
   * Håll muspekaren över namnet på jobbrollen och klicka på ikonen **[!UICONTROL delete]** ![](assets/delete.png) för att ta bort jobbrollen från initiativet.
   * Välj **[!UICONTROL Add roles to the scenario's available resources]** och klicka sedan på **[!UICONTROL Apply]**.

     Det här lägger till antalet saknade FTE:er eller timmar för jobbroller i scenariots [!UICONTROL Available]-fält.

     >[!NOTE]
     >
     >De roller du lägger till för att lösa konflikterna ändrar jobbrollerna [!UICONTROL Available] för det valda scenariot och inte för alla scenarier i planen.

     En uppåtriktad grön pil ![](assets/upward-green-arrow.png) visas för månaden i tidslinjen i planen för att ange att fler resurser har lagts till i planen den månaden. Du måste markera vyn [!UICONTROL Month] för att kunna se den här indikatorn.

   * (Villkorligt) Stäng panelen Detaljer och ge initiativet en högre prioritet att ta emot budgetresurser från planen först, om det är möjligt. Mer information om att uppdatera prioritet för initiativ finns i [Uppdatera prioritet för initiativ i scenarioplanen](../scenario-planner/prioritize-initiatives.md).

1. (Valfritt) Klicka på **[!UICONTROL Hide details]** för att stänga den ytterligare informationsrutan och klicka sedan på **[!UICONTROL Apply]** för att spara ändringarna du gör i jobbroller.

1. (Villkorligt) För initiativ med kostnadskonflikter går du till avsnittet **[!UICONTROL Costs]** i panelen Initiativinformation och granskar kostnaderna för varje månad som initieringens varaktighet varar. Identifiera vilka månader som kanske inte har tillräckligt med pengar i planens budget för att täcka kostnaderna för det valda initiativet. Rutan med otillräcklig budget visas i en röd ram.
1. (Valfritt) Klicka på den högerriktade pilen bredvid månaderna i tidslinjen för initiativet för att se ytterligare månader som inte har tillräcklig budget för att täcka kostnaderna.

   ![](assets/details-panel-insufficient-costs-350x239.png)

1. (Valfritt) Klicka på **[!UICONTROL Show details]** under kostnadsinformationen för att se var konflikten förekommer och för att markera de månader som står i konflikt i planens diagram. Följande ytterligare fält visas för varje typ av kostnad:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Available]</td> 
      <td> <p>Kostnaderna som är tillgängliga från planens budget för varje månad. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Previously allocated]</td> 
      <td>Det belopp som redan anslagits från planens budget till initiativ med högre rankning. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Overallocated]</td> 
      <td> <p>Den månatliga skillnaden mellan de kostnader som krävs för initiativet och de pengar som är tillgängliga från planens budget efter större rankningsinitiativ har också utnyttjat en del av den tillgängliga budgeten. [!DNL Workfront] beräknar antalet överfördelade kostnader med följande formel:</p> <p><code>Overallocated costs = (Costs Previously Allocated to higher initiatives + Required costs for the current initiative) - Monthly available budget from the plan</code> </p> <p>[!DNL Workfront] Beräknar de obligatoriska kostnaderna för det aktuella initiativet för varje månad med hjälp av följande formel:</p> <p><code>Required initiative costs = Initiative Fixed Costs + Initiative People Costs</code> </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >I planens diagram visar de månader där kostnaderna är otillräckliga namn och antal roller som fortfarande behövs för initiativet. Du måste välja månadsvyn för att visa kostnadsbeloppen.

   ![](assets/conflicting-costs-months-on-plan-after-clicking-show-details-350x139.png)

   >[!NOTE]
   >
   >Om du inaktiverade [!UICONTROL Include people cost]-inställningen för planens [!UICONTROL Budget]-ruta när du skapade planen visas inte [!UICONTROL People Costs]-raden för några initiativ i något scenario. I det här fallet tar Workfront inte personkostnader med i beräkningar för att fastställa kostnadskonflikter. Mer information om hur du skapar en plan finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

1. Gör något av följande för att lösa kostnadskonflikter:

   * Justera manuellt antalet [!UICONTROL Fixed Costs] för varje månad i initiativet till ett lägre antal.
   * I avsnittet **[!UICONTROL Required Job Roles]** justerar du om möjligt antalet jobbroller för månaden med en personkostnadsbudget. Detta minskar antalet personkostnader.

     >[!TIP]
     >
     >Du kan inte justera personkostnader manuellt.

   * Välj **[!UICONTROL Add amount to the scenario's budget]** och klicka sedan på **[!UICONTROL Apply]**.

     Detta adderar det otillräckliga beloppet till scenariots budget för de månader där det saknades, vilket även uppdaterar den övergripande scenariobudgeten.

     >[!NOTE]
     >
     >Det belopp som du lägger till för att lösa kostnadskonflikterna ändrar budgeten för det valda scenariot och inte för alla scenarier i planen.

   * (Villkorligt) Stäng panelen Detaljer och ge initiativet en högre prioritet att ta emot budgetresurser från planen först, om det är möjligt. Mer information om uppdatering av prioritet för initiativ finns i [Uppdatera prioritet för initiativ i  [!DNL Scenario Planner]](../scenario-planner/prioritize-initiatives.md).

1. Klicka på **[!UICONTROL Apply]** när du gör några ändringar i avsnittet Kostnader.
1. Klicka på **[!UICONTROL Save plan]** om du vill spara ändringarna.


