---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Skapa och redigera planer i scenarioplaneraren
description: Du kan skapa planer som en del av att använda Workfront Scenarioplan när du prioriterar företagets strategi på en högre nivå. Mer information om planer finns i Planer - översikt i Scenarioplaneraren.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '2244'
ht-degree: 0%

---

# Skapa och redigera planer i [!DNL Scenario Planner]

Du kan skapa planer som en del av [!DNL Workfront Scenario Planner]när ni prioriterar er strategi på en högre nivå. Mer information om planer finns i [Planer - översikt i [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

## Åtkomstkrav

Du måste ha följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td>[!UICONTROL Business] eller högre</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens*</p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt</td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du får [!UICONTROL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!UICONTROL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationer på åtkomstnivå* </td> 
   <td> <p>[!UICONTROL Edit] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Obs! Om du fortfarande inte har åtkomst frågar du Workfront-administratören om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!DNL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Skapa eller redigera planer

Du kan skapa en helt ny plan eller redigera en befintlig plan som delats med dig.

>[!NOTE]
>
>När du har skapat en plan betraktas du som planskapare och ägare. När en användare inaktiveras har planen ingen ägare och är inte synlig för någon om den inte tidigare delats med en länk.

I den här artikeln beskrivs hur du kan skapa en plan från grunden eller redigera en befintlig plan.

Om du vill ha mer information om planer, inklusive information om en plan, kan du läsa [Planer - översikt i [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Mer information om hur du tar bort planer finns i [Ta bort planer i [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Så här skapar eller redigerar du en plan:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png)och sedan klicka [!UICONTROL Scenarios].

   En lista över befintliga planer som du har skapat visas i [!DNL Workfront Scenario Planner].

1. (Valfritt) Klicka på **[!UICONTROL Filter]** icon ![](assets/filter-icon-34x37.png)i planlistans övre högra hörn och välj något av följande:

   | Filter | Beskrivning |
   |---|---|
   | [!UICONTROL All] | Visar alla planer som du har skapat eller som har delats med dig. |
   | [!UICONTROL My plans] | Visar planer som du har skapat. |
   | [!UICONTROL Shared with me] | Visar planer som delas med dig. |

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Valfritt) Klicka på **[!UICONTROL Search]** icon ![](assets/search-icon.png) om du vill skriva ett nyckelord och snabbt hitta en plan i listan.

1. Klicka på namnet på en befintlig plan för att redigera den och fortsätt med steg 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   eller

   Klicka **[!UICONTROL New Plan]** i det övre vänstra hörnet för att skapa en plan och fortsätta med steg 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![](assets/new-plan-button.png)

   The [!UICONTROL New Plan] visas.

   ![](assets/new-plan-ui-adding-a-new-plan-350x306.png)

1. (Villkorligt) Ange följande information när du skapar en ny plan:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Name]</td> 
      <td>Ange ett namn för planen. Detta är ett obligatoriskt fält.</td> 
     </tr> 
     <tr> 
      <td role="rowheader" colspan="2"> <p>Viktigt: <span style="font-weight: normal;">Du kan inte ändra följande val när du har skapat och sparat planen.</span> </p> </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader"><span>FTE ([!UICONTROL Full Time Equivalent]) eller [!UICONTROL Hours]</span> </td> 
      <td> <p><span>Välj något av följande alternativ för att ange hur du vill beräkna jobbrollsinformation för den här planen:</span> </p> 
       <ul> 
        <li> <p><span><strong>FTE</strong>. Detta är standardinställningen </span> </p> <!--
          <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>
         --> <p>För alla beräkningar i [!DNL Scenario Planner], [!DNL Workfront] använder följande värde: 1 heltidsanställd = 8 timmar. </p> </li> 
        <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p>Viktigt: <span>Det alternativ du väljer här avgör hur information om jobbroller visas för planen, planens scenarier och initiativ.</span> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start date]</td> 
      <td> <p>Välj den månad och det år då du vill att planen ska starta. I det här fältet kan du bara välja månader. [!DNL Workfront] förutsätter att startdatumet för planen är den första dagen i den valda månaden och att slutdatumet är den sista dagen i slutet av månaden. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Duration]</td> 
      <td> <p>I listrutan väljer du bland följande varaktigheter:</p> 
       <ul> 
        <li>1 år. Detta är standardlängden. </li> 
        <li>3 år</li> 
        <li> <p>5 år</p> </li> 
       </ul> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Villkorligt) Klicka **[!UICONTROL Next]**.

   Tidslinjen för planen visas som **[!UICONTROL Initial scenario]**.

   Mer information om hur du skapar ytterligare scenarier finns i [Skapa och jämföra planscenarier i [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Valfritt) I listrutan Tidslinje väljer du ett av alternativen i följande tabell för att ändra hur du visar tidslinjen för planen.

   ![](assets/month-dropdown-with-all-options.png)

   | Nedrullningsbart menyalternativ | Beskrivning |
   |---|---|
   | [!UICONTROL Month] | Visar tidslinjen per månad. Detta är standardinställningen och det enda alternativet för en ettårsplan. |
   | [!UICONTROL Quarter] | Visar tidslinjen per kvartal. Det här alternativet är bara tillgängligt när [!UICONTROL Duration] för planen är 3 eller 5 år. Det här är standardalternativet för en 3-årsplan. |
   | [!UICONTROL Year] | Visar tidslinjen per år. Det här alternativet är bara tillgängligt när [!UICONTROL Duration] av planen är fem år. Det här är standardalternativet för en femårsplan. |

1. (Valfritt) Bläddra från vänster till höger för att visa hela planens varaktighet.
1. (Valfritt) Klicka på **[!UICONTROL Today]** indikatorrad som ska återgå till den aktuella dagen.

   ![](assets/today-indicator-350x160.png)

1. Klicka på **[!UICONTROL Job Roles]** i planens huvud för att lägga till jobbroller som är tillgängliga för att genomföra planen.

   Information om [!UICONTROL Job Roles] visas.

   >[!TIP]
   >
   >Rollallokeringsenheten (FTE eller timmar) som [!DNL Workfront] för den här planen visas inom parentes i rutans rubrik.

   ![](assets/adding-people-to-plan-350x206.png)

1. Klicka på **[!UICONTROL Start typing job role]** och välj en roll i listan eller börja skriva namnet på en aktiv jobbroll.

   Alla aktiva jobbroller i systemet visas när du klickar på det här fältet.

   Detta lägger till jobbrollen i kolumnen Jobbroller.

1. Uppdatera eller granska följande information för jobbrollen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (för heltidsanställda) </p> <p role="rowheader">eller </p> <p role="rowheader"><span>[!UICONTROL Total available] (i timmar)</span> </p> </td> 
      <td> <p><span>Beroende på om du valt att använda timmar eller heltidsanställd för din plan kan du skriva</span> antalet heltidsanställda jobbroller <span>eller timmar</span> som är tillgängliga för att utföra arbete på planen i följande fält: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total available]</strong> (i timmar): Ange det totala antalet timmar för alla månader under scenariots varaktighet. Som standard [!DNL Workfront] dividerar det totala tillgängliga antalet jämnt över alla månader i scenariots varaktighet. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om du anger 1 200 timmar för en Designer innebär det att Designer är tillgängligt i 100 timmar för varje månad under planens giltighetstid, när planen [!UICONTROL Duration] är ett år. </p> </li> 
        <li> <p><b>[!UICONTROL Max available]</b> (för heltidsanställda): Ange antalet heltidsanställda som jobbrollen är tillgänglig för varje månad under planens varaktighet. Som standard <strong>Workfront</strong> tilldelar [!UICONTROL Max available] till varje månad under scenariot.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om du anger 1 heltidsanställd för en konsult innebär detta att konsulten är tillgänglig för 1 heltidsanställd för varje månad under planens löptid. </p> <p>Du kan ange ett tal som är lägre än 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>En arbetsuppgift för 0.5-konsulter innebär att en konsult skulle ägna hälften av sin heltidsanställda (vanligtvis 4 timmar, där 8 timmar är 1 heltidsanställd) åt att arbeta med planen. För alla beräkningar i Scenarioplaneraren använder Workfront följande värde: 1 heltidsanställd = 8 timmar. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max required] (för heltidsanställda)</p> <p role="rowheader">eller </p> <p role="rowheader"><span>[!UICONTROL Total required] (i timmar)</span> </p> </td> 
      <td> <p><span>Beroende på om du valt att använda timmar eller heltidsanställd för din plan kan du granska</span> antalet heltidsanställda jobbroller <span>eller timmar</span> som krävs för att slutföra satsningarna i scenariot. Granska följande fält:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total required]</strong> (i timmar): Det totala antalet timmar som krävs för alla månader under planens varaktighet.</p> </li> 
        <li> <p><strong>[!UICONTROL Max required]</strong> (för heltidsanställda): Maximalt antal heltidsanställda som krävs för någon av månaderna under planens löptid. </p> </li> 
       </ul> <p>Tips: The <span>maximum</span> antal heltidsanställda <span>eller det totala antalet timmar</span> som krävs för den jobbrollen visas när du har börjat lägga till initiativ. Mer information om hur du lägger till initiativ i en plan finns i <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Skapa och redigera i [!DNL Scenario Planner]</a>.</p> </td> 
     </tr> <!--
      <tr data-mc-conditions="QuicksilverOrClassic.Draft mode"> 
       <td role="rowheader">[!UICONTROL Avg utilization]</td> 
       <td> <p>(NOTE: this field was removed in 21.2 - May 2021) </p> <p>[!DNL Workfront] calculates the average utilization for each job role using the job role FTEs associated with initiatives (required) and the job role FTEs associated with the plan (available). </p> <p> [!DNL Workfront] calculates the job role utilization percentage for a plan using the following formula: </p> <p><code>Job role utilization percentage = Sum [(Required job roles for each month of the plan *100)/ (Available job roles for each month of the plan)] / Number of months in the Duration of the plan</code> </p> 
        <div class="example" data-mc-autonum="<b>Example: </b>"> <span class="autonumber"><span><b>Example: </b></span></span> 
         <p>For example, if you have a plan with a duration of 12 months and an initiative with the duration of 2 months, where you use 1 Designer for your initiative (required job role) and there are 2 Designers available on the plan (available), the Utilization percentage for the Designer job role is calculated as follows:</p> 
         <p><code>Designer utilization percentage = [(1/2 + 1/2) * 100] / 12 = 100 / 12 = 8.3%</code> </p> 
        </div> <p>As you add job roles to the plan and indicate the Available amount for each one, the [!UICONTROL Utilization] value for each role also updates and [!DNL Workfront] calculates a utilization percentage for the plan. For information about how [!DNL Workfront] calculates the Job Role Utilization for a plan, see <a href="../scenario-planner/plans-overview.md" class="MCXref xref">Plans overview in the [!DNL Scenario Planner]</a>. </p> <p>Tip: The Utilization percentage is rounded and has one decimal. </p> </td> 
      </tr>
     --> 
     <tr> 
      <td role="rowheader">[!UICONTROL Hourly rate]</td> 
      <td> <p>Det här är [!UICONTROL Cost Hour] hastighet för jobbrollen. Timpriset visas i systemets valuta. Mer information om hur du ställer in valutakurser för ditt system finns i <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Ställ in valutakurser</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Håll muspekaren över namnet på en jobbroll eller klicka på fliken när du har uppdaterat rollinformationen och klicka sedan på knappen **[!UICONTROL trash can icon]** ![](assets/delete.png) för att ta bort den från planen.
1. Klicka på **[!UICONTROL Job role distribution]**.

   Panelen Jobbrollsfördelning visas för alla månader under scenariot.

   ![](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Skriv namnet på en jobbroll som ska läggas till i planen i **[!UICONTROL Start typing job role field]** klickar du sedan på Enter när den visas i listan. Detta lägger till jobbrollen i [!UICONTROL Job Roles] kolumn.
1. Uppdatera eller granska följande information för varje månad i scenariot:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Roles] (heltidsekvivalenter eller timmar)</td> 
      <td>Både den jobbroll som är tillgänglig för scenariot och den som krävs för initiativen i scenariot visas på panelen för jobbrollsfördelning. Det finns en indikation på om uppskattningar av jobbroller finns i heltidsanställda eller timmar i kolumnrubriken. </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p>[!UICONTROL Available] (max &lt;number of="" ftes=""&gt;) </p> 
       <div> 
        <p>eller</p> 
        <p>[!UICONTROL Available] (totalt &lt;number of="" hours=""&gt;) </p> 
       </div> </td> 
      <td> <p><span>Beroende på om du valt att använda timmar eller heltidsanställd för din plan, granska eller uppdatera</span> månadsantalet heltidsanställda befattningar <span>eller timmar</span> är tillgängliga för scenariot i följande fält:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Available] (max &lt;number of="" ftes=""&gt;)</strong>: Antalet inom parentes visar det maximala antalet roller som är tillgängliga för en av månaderna för scenariot. Granska eller uppdatera antalet heltidsanställda för varje månad i scenariot. Om du ändrar månadstilldelningen kan antalet heltidsanställda uppdateras inom parenteserna. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Available] (totalt &lt;number of="" hours=""&gt;)</strong>: Antalet inom parentes visar det totala antalet tillgängliga timmar för alla månader i scenariot. Granska eller uppdatera antalet timmar för varje månad i scenariot. Om du ändrar den månatliga tilldelningen uppdateras antalet timmar inom parenteserna.</span> </p> </li> 
       </ul> <p>Manuell uppdatering av de månatliga jobbrollallokeringarna är ett annat sätt att lösa jobbrollskonflikter mellan initiativ i scenariot. </p> <p>Tips:   <p><span>Om du vill uppdatera den månatliga rolltillgängligheten för flera månader skriver du antalet timmar eller heltidsanställda i [!UICONTROL Available] i valfri månad och dra sedan fältets hörn över de angränsande månaderna för att kopiera samma värde för varje månad. Släpp det för att uppdatera alla månader.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Required] (max &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">eller</p> 
        <p role="rowheader">[!UICONTROL Required] (totalt &lt;number&gt;)</p> 
       </div> </td> 
      <td> <p><span>Beroende på om du valt att använda timmar eller heltidsanställd för din plan kan du granska</span> Månadsantalet FTE eller timmar för jobbroll som krävs för scenariot i följande fält: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Required] (max &lt;number of="" ftes=""&gt;)</strong>: Antalet inom parentes visar det maximala antalet roller som krävs för någon av månaderna för scenariot. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Required] (totalt &lt;number of="" hours=""&gt;)</strong>: Antalet inom parentes visar det totala antalet timmar som krävs för alla månader i scenariot.</span> </p> </li> 
       </ul> <p>Tips: Du kan inte ändra antalet FTE som krävs <span>eller timmar</span> för jobbrollen. Det här numret fyller i scenariot när du har börjat lägga till initiativ och deras krav på jobbroll. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>Den månatliga skillnaden mellan mängden obligatoriska och tillgängliga jobbroller för scenariot. [!DNL Workfront] beräknar skillnaden för varje jobbroll för varje månad med hjälp av följande formel:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (i heltidsekvivalenter eller timmar) </p> 
        <p>Tips: När skillnaden visar ett negativt tal, kräver scenariot fler jobbroller än vad som finns tillgängligt i planen. Dina resurser är överallokerade. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Utilization] %</td> 
      <td> 
       <div> 
        <p>I procent av användningen visas hur många av de tillgängliga jobbrollerna som faktiskt används (eller krävs) för initiativen i scenariot. </p> 
        <p>[!DNL Workfront] beräknar utnyttjandegraden per jobbroll per månad med hjälp av följande formel: </p> 
        <p><code>Monthly role utilization % = Monthly required roles / Monthly available roles * 100</code> </p> 
        <p>Den procentuella användningen kan visas i följande färger, beroende på resurstilldelningen:</p> 
        <ul> 
         <li> <p><b>Grön</b>: Antalet tillgängliga och obligatoriska jobbroller matchar. Resurserna är helt fördelade och utnyttjandeprocenten är 100 %. </p> </li> 
         <li> <p><b>Röd</b>: Det finns fler obligatoriska jobbroller än vad som är tillgängligt i planen. Resurserna är överallokerade och utnyttjandeprocenten är högre än 100 %.</p> </li> 
         <li> <p><b>Blå</b>: Det finns fler tillgängliga jobbroller än vad de behöver. Resurserna är underallokerade och utnyttjandeprocenten är lägre än 100 %. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka **[!UICONTROL Apply]** för att spara den månatliga fördelningen av jobbroller

   eller

   Klicka **[!UICONTROL Cancel]** för att stänga distributionslistan för jobbroller och återgå till scenariot.

1. Klicka på **[!UICONTROL Financial]** i planens huvud för att lägga till budgeten för den här planen.

   Information om [!UICONTROL Financial] visas.

   >[!TIP]
   >
   >Valutan som [!DNL Workfront] för den här planen visas inom parentes i rutans rubrik.

1. Ange **[!UICONTROL Yearly budget]**.

   >[!NOTE]
   >
   >Om din plan sträcker sig över flera år måste du ange ett budgetbelopp för varje år.

1. Tryck på Retur för att spara den årliga budgeten och sedan [!UICONTROL Tab] för att gå över till nästa år.

   Den årliga budgeten fördelas automatiskt jämnt för varje månad under det valda året.

1. Klicka **[!UICONTROL Advanced]** för att se den månatliga budgetfördelningen. De årliga och månadsvisa budgetarna är alltid avrundade tal. När budgetbeloppet inte kan fördelas jämnt på alla månader inom ett år på grund av decimaler a **[!UICONTROL Remaining]** indikator visas under den årliga budgetfördelningen.

   ![](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Justera månadsbudgeten manuellt för att eliminera de belopp som överskrider gränsen.

   När summan av alla månadsbudgetbelopp är större än den årliga budgeten, kan **[!UICONTROL Exceeding]** varningsindikator visas under den årliga budgetfördelningen. Justera månadsbudgetbeloppen manuellt tills de är lika med eller lägre än den tillgängliga budgeten för planen.

   ![](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Inaktivera **[!UICONTROL Include people costs]** Inställning för att utesluta kostnader som är kopplade till jobbroller från att räknas mot planens totala kostnad. Fasta kostnader räknas alltid in i planens totala kostnad. Den här inställningen är aktiverad som standard och påverkar alla scenarier i planen.
1. Klicka var som helst utanför [!UICONTROL Financial] för att stänga den. Informationen som du angav sparas automatiskt.

   Nu kan du börja skapa initiativ för planen och lägga till scenarier.

1. (Rekommenderas) Klicka på **[!UICONTROL New initiative]** att lägga till ett nytt initiativ.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Mer information om hur du lägger till initiativ finns i artikeln [Skapa och redigera i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Valfritt) Skapa en kopia av det befintliga scenariot för att skapa ett nytt scenario för samma plan. Mer information om hur du skapar och arbetar med flera scenarier finns i [Skapa och jämföra planscenarier i [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Klicka på **[!UICONTROL Save Plan]**.

   Din plan skapas eller uppdateras.

1. (Valfritt) Klicka på **[!UICONTROL Favorites icon]** ![](assets/favorites-icon-small.png) till höger om namnet på planen om du vill lägga till planen i listan Favoriter.

1. (Valfritt) Kopiera URL:en för planen och skicka den till andra användare som kan behöva granska eller uppdatera den. De måste åtminstone ha [!UICONTROL View] behörighet på åtkomstnivå för att kunna se planen. De måste ha [!UICONTROL Edit] behörighet att redigera det. Om de måste granska ekonomisk information om planen, som budgetar, kostnader och jobbrollstariffer, måste de också ha tillgång till [!UICONTROL Financial Data] på deras åtkomstnivå. Mer information om åtkomsten som krävs för [!DNL Scenario Planner], se [Åtkomst krävs för att använda [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
