---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Skapa och redigera planer i scenarioplaneraren
description: Du kan skapa planer som en del av att använda Workfront Scenarioplan när du prioriterar företagets strategi på en högre nivå. Mer information om planer finns i Planer - översikt i Scenarioplaneraren.
author: Alina
feature: Workfront Scenario Planner
exl-id: 15c0e519-0164-449d-84f3-470d0d4eb795
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '2285'
ht-degree: 0%

---

# Skapa och redigera planer i [!DNL Scenario Planner]

Du kan skapa planer som en del av att använda [!DNL Workfront Scenario Planner] när du prioriterar ditt företags strategi på en högre nivå. Mer information om planer finns i [Planöversikt i  [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

<!--
<div data-mc-conditions="QuicksilverOrClassic.Draft mode">
<p>(NOTE: talk about:</p>
<p>- Show people conflicts >> this impacts the conflicts calculation for initiatives>> link to the conflicts article</p>
<p>- explain what hovering over the green upward-pointing arrow does, with screen shot)</p>
</div>
-->

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
   <p>Scenarioplanen är inte tillgänglig för nya Workfront Select- eller Workfront Prime-planer. </p>
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

## Skapa eller redigera planer

Du kan skapa en helt ny plan eller redigera en befintlig plan som delats med dig.

>[!NOTE]
>
>När du har skapat en plan betraktas du som planskapare och ägare. När en användare inaktiveras har planen ingen ägare och är inte synlig för någon om den inte tidigare delats med en länk.

I den här artikeln beskrivs hur du kan skapa en plan från grunden eller redigera en befintlig plan.

Alla överväganden om planer, inklusive information som är tillgänglig för en plan, finns i [Översikt över planer i  [!DNL Scenario Planner]](../scenario-planner/plans-overview.md).

Mer information om hur du tar bort planer finns i [Ta bort planer i  [!DNL Scenario Planner]](../scenario-planner/delete-plans.md).

Så här skapar eller redigerar du en plan:

{{step1-to-scenario-planner}}

En lista över befintliga planer som du har skapat visas i [!DNL Workfront Scenario Planner].

1. (Valfritt) Klicka på ikonen **[!UICONTROL Filter]** ![Filter &#x200B;](assets/filter-icon-34x37.png) i det övre högra hörnet av planlistan och välj något av följande:

   | Filter | Beskrivning |
   |---|---|
   | [!UICONTROL All] | Visar alla planer som du har skapat eller som har delats med dig. |
   | [!UICONTROL My plans] | Visar planer som du har skapat. |
   | [!UICONTROL Shared with me] | Visar planer som delas med dig. |

   ![Listrutealternativ för planfilter](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Search]** ![&#x200B; Sök &#x200B;](assets/search-icon.png) om du vill skriva ett nyckelord och snabbt hitta en plan i listan.

1. Klicka på namnet på en befintlig plan för att redigera den och fortsätt med steg 7.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate) </p>
   -->

   eller

   Klicka på **[!UICONTROL New Plan]** i det övre vänstra hörnet för att skapa en plan och fortsätta med steg 5.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: is the step still accurate)</p>
   -->

   ![Knappen Ny plan](assets/new-plan-button.png)

   Rutan [!UICONTROL New Plan] visas.

   ![Ny planruta](assets/new-plan-ui-adding-a-new-plan-350x306.png)

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
      <td> <p><span>Välj ett av följande alternativ för att ange hur du vill beräkna jobbrollsinformation för den här planen:</span> </p> 
       <ul> 
      <li> <p><span><strong>FTE</strong>. Det här är standardvärdet </span> </p> 
      <p><b>VIKTIGT</b></p>  
      <p>För alla beräkningar i [!DNL Scenario Planner] använder [!DNL Workfront] följande värde: 1 FTE = 8 timmar. </p> </li> 
      <li> <p><strong>[!UICONTROL Hours]</strong> </p> </li> 
       </ul> <p><b>VIKTIGT</b></p>

   Det alternativ du väljer här avgör hur information om jobbroll visas för planen, planens scenarier och initiativ</p> </td>
   </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Start date]</td> 
      <td> <p>Välj den månad och det år då du vill att planen ska starta. I det här fältet kan du bara välja månader. [!DNL Workfront] antar att startdatumet för planen är den första dagen i den valda månaden och att slutdatumet är den sista dagen i slutet av månaden. </p> </td> 
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

<!--for table above - how FTE is calcualted: NOTE: snippet below: this is per Ani; it does NOT look at the system FTE.) </p>-->

1. (Villkorligt) Klicka på **[!UICONTROL Next]**.

   Tidslinjen för planen visas som **[!UICONTROL Initial scenario]**.

   Mer information om hur du skapar ytterligare scenarier finns i [Skapa och jämföra planscenarier i  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Valfritt) I listrutan Tidslinje väljer du ett av alternativen i följande tabell för att ändra hur du visar tidslinjen för planen.

   ![Månad-listrutan](assets/month-dropdown-with-all-options.png)

   | Nedrullningsbart menyalternativ | Beskrivning |
   |---|---|
   | [!UICONTROL Month] | Visar tidslinjen per månad. Detta är standardinställningen och det enda alternativet för en ettårsplan. |
   | [!UICONTROL Quarter] | Visar tidslinjen per kvartal. Det här alternativet är endast tillgängligt när [!UICONTROL Duration] för planen är 3 eller 5 år. Det här är standardalternativet för en 3-årsplan. |
   | [!UICONTROL Year] | Visar tidslinjen per år. Det här alternativet är endast tillgängligt när [!UICONTROL Duration] för planen är fem år. Det här är standardalternativet för en femårsplan. |

1. (Valfritt) Bläddra från vänster till höger för att visa hela planens varaktighet.
1. (Valfritt) Klicka på indikatorraden **[!UICONTROL Today]** om du vill återgå till den aktuella dagen.

   ![Aktuell indikator](assets/today-indicator-350x160.png)

1. Klicka på rutan **[!UICONTROL Job Roles]** i planens huvud för att lägga till jobbroller som är tillgängliga för att genomföra planen.

   Information om [!UICONTROL Job Roles]-rutevisningen.

   >[!TIP]
   >
   >Rollallokeringsenheten (FTE eller timmar) som [!DNL Workfront] använder för den här planen visas inom parentes i rutans rubrik.

   ![Lägger till personer i planen](assets/adding-people-to-plan-350x206.png)

1. Klicka på fältet **[!UICONTROL Start typing job role]** och välj en roll i listan eller börja skriva namnet på en aktiv jobbroll.

   Alla aktiva jobbroller i systemet visas när du klickar på det här fältet.

   Detta lägger till jobbrollen i kolumnen Jobbroller.

1. Uppdatera eller granska följande information för jobbrollen:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max available] (för heltidsanställda) </p> <p role="rowheader">eller </p> <p role="rowheader"><span>[!UICONTROL Total available] (i timmar)</span> </p> </td> 
      <td> <p><span>Beroende på om du har valt att använda timmar eller FTE för din plan skriver du</span> antalet FTE:er <span>eller timmar</span> för jobbrollen som är tillgängliga för att utföra arbete på planen i följande fält: </p> 
       <ul> 
        <li> <p style="font-weight: normal;"><strong>[!UICONTROL Total available]</strong> (för timmar): Ange det totala antalet timmar för alla månader under scenariots varaktighet. Som standard delar [!DNL Workfront] det totala tillgängliga antalet jämnt över alla månader i scenariots varaktighet. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om du anger 1 200 timmar för en Designer innebär det att Designer är tillgängligt i 100 timmar för varje månad under planens löptid, när planen [!UICONTROL Duration] är 1 år. </p> </li> 
        <li> <p><b>[!UICONTROL Max available]</b> (för heltidsanställda): Ange antalet heltidsanställda som jobbrollen är tillgänglig för varje månad under planens löptid. Som standard tilldelar <strong>Workfront</strong> talet [!UICONTROL Max available] till varje månad under scenariots varaktighet.</p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>Om du anger 1 heltidsanställd för en konsult innebär det att konsulten är tillgänglig för 1 heltidsanställd för varje månad under planens giltighetstid. </p> <p>Du kan ange ett tal som är lägre än 1 FTE. </p> <p class="example" data-mc-autonum="<b>Example: </b>"><span class="autonumber"><span><b>Exempel: </b></span></span>En jobbroll för 0,5-konsult innebär att en konsult skulle avsätta hälften av sin heltidsanställda (vanligtvis 4 timmar, där 8 timmar är 1 heltidsanställd) till att arbeta med den här planen. För alla beräkningar i Scenarioplaneraren använder Workfront följande värde: 1 FTE = 8 timmar. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Max required] (för heltidsanställda)</p> <p role="rowheader">eller </p> <p role="rowheader"><span>[!UICONTROL Total required] (i timmar)</span> </p> </td> 
      <td> <p><span>Beroende på om du valt att använda timmar eller heltidsanställd för din plan kan du granska</span> antalet heltidsanställda <span> eller timmar</span> som krävs för att slutföra initiativen i scenariot. Granska följande fält:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Total required]</strong> (för timmar): Det totala antalet timmar som krävs för alla månader under planens varaktighet.</p> </li> 
        <li> <p><strong>[!UICONTROL Max required]</strong> (för heltidsanställda): Det högsta antal heltidsanställda som krävs för någon av månaderna under planens löptid. </p> </li> 
       </ul> <p>Tips! Det <span>maximala</span> antalet FTE <span> eller det totala antalet timmar</span> som krävs för den jobbrollen visas när du har påbörjat tillägg av initiativ. Mer information om hur du lägger till initiativ i en plan finns i <a href="../scenario-planner/create-and-edit-initiatives.md" class="MCXref xref">Skapa och redigera initiativ i [!DNL Scenario Planner]</a>.</p> </td> 
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
      <td> <p>Detta är frekvensen [!UICONTROL Cost Hour] för jobbrollen. Timpriset visas i systemets valuta. Mer information om hur du konfigurerar valutakurser för ditt system finns i <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Konfigurera valutakurser</a>.</p> </td> 
     </tr> 
    </tbody> 
   </table>

1. (Valfritt) Håll muspekaren över namnet på en jobbroll eller klicka på fliken efter att du har uppdaterat rollinformationen och klicka sedan på ikonen **[!UICONTROL trash can icon]** ![Ta bort](assets/delete.png) för att ta bort den från planen.
1. Klicka på **[!UICONTROL Job role distribution]**.

   Panelen Jobbrollsfördelning visas för alla månader under scenariot.

   ![Månadsdistribution av jobbroll](assets/job-role-monthly-distribution-box-fte-350x144.png)

1. Skriv namnet på en jobbroll som du vill lägga till den i planen i **[!UICONTROL Start typing job role field]** och klicka sedan på Enter när den visas i listan. Detta lägger till jobbrollen i kolumnen [!UICONTROL Job Roles].
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
      <td role="rowheader"> <p>[!UICONTROL Available] (max &lt;antal heltidsanställda&gt;) </p> 
       <div> 
        <p>eller</p> 
        <p>[!UICONTROL Available] (totalt &lt;antal timmar&gt;) </p> 
       </div> </td> 
      <td> <p><span>Beroende på om du har valt att använda timmar eller FTE för din plan kan du granska eller uppdatera</span> det månadsvisa antalet FTE <span>eller timmar</span> för jobbrollen som är tillgängligt för scenariot i följande fält:</p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Available] (max &lt;antal FTE&gt;)</strong>: Antalet inom parentes visar det maximala antalet roller som är tillgängliga för en av månaderna för scenariot. Granska eller uppdatera antalet heltidsanställda för varje månad i scenariot. Om du ändrar månadstilldelningen kan antalet heltidsanställda uppdateras inom parenteserna. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Available] (totalt &lt;antal timmar&gt;)</strong>: Antalet inom parentes visar det totala antalet tillgängliga timmar för alla månader i scenariot. Granska eller uppdatera antalet timmar för varje månad i scenariot. Om du ändrar den månatliga allokeringen uppdateras antalet timmar inom parenteserna.</span> </p> </li> 
       </ul> <p>Manuell uppdatering av de månatliga jobbrollallokeringarna är ett annat sätt att lösa jobbrollskonflikter mellan initiativ i scenariot. </p> <p>Tips:   <p><span>Om du vill uppdatera den månatliga rolltillgängligheten för flera månader skriver du antalet timmar eller heltidsanställda i fältet [!UICONTROL Available] för en månad och drar sedan fältets hörn över de angränsande månaderna för att kopiera samma värde för varje månad. Släpp det för att uppdatera alla månader.</span> </p> <p> <img src="assets/job-role-distribution-draggable-corner-highlighted-350x83.png" style="width: 350;height: 83;"> </p> </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader"> <p role="rowheader">[!UICONTROL Required] (max &lt;number&gt;)</p> 
       <div> 
        <p role="rowheader">eller</p> 
        <p role="rowheader">[!UICONTROL Required] (totalt &lt;tal&gt;)</p> 
       </div> </td> 
      <td> <p><span>Beroende på om du har valt att använda timmar eller heltidsanställd för din plan kan du granska</span> det månadsvisa antalet heltidsanställda eller timmar för jobbroller som krävs för scenariot i följande fält: </p> 
       <ul> 
        <li> <p><strong>[!UICONTROL Required] (max &lt;antal FTE&gt;)</strong>: Antalet inom parentes visar det maximala antalet roller som krävs för någon av månaderna för scenariot. </p> </li> 
        <li> <p><span><strong>[!UICONTROL Required] (totalt &lt;antal timmar&gt;)</strong>: Antalet inom parentes visar det totala antalet timmar som krävs för alla månader i scenariot.</span> </p> </li> 
       </ul> <p>Tips! Du kan inte ändra antalet FTE <span> eller timmar </span> som krävs för jobbrollen. Det här numret fyller i scenariot när du har börjat lägga till initiativ och deras krav på jobbroll. </p> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Difference]</td> 
      <td> 
       <div> 
        <p>Den månatliga skillnaden mellan mängden obligatoriska och tillgängliga jobbroller för scenariot. [!DNL Workfront] beräknar skillnaden för varje jobbroll för varje månad med följande formel:</p> 
        <p><code>Monthly role difference = Monthly required roles - Monthly available roles</code> (i heltidsekvivalenter eller timmar) </p> 
        <p>Tips! När skillnaden visar ett negativt tal kräver scenariot fler jobbroller än vad planen har tillgängligt. Dina resurser är överallokerade. </p> 
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
         <li> <p><b>Röd</b>: Det finns fler obligatoriska jobbroller än vad som finns i planen. Resurserna är överallokerade och utnyttjandeprocenten är högre än 100 %.</p> </li> 
         <li> <p><b>Blå</b>: Det finns fler tillgängliga jobbroller än de som krävs. Resurserna är underallokerade och utnyttjandeprocenten är lägre än 100 %. </p> </li> 
        </ul> 
       </div> <p> <img src="assets/utilization-percent-colors-sp-350x61.png" style="width: 350;height: 61;"> </p> </td> 
     </tr> 
    </tbody> 
   </table>

1. Klicka på **[!UICONTROL Apply]** för att spara den månatliga fördelningen av jobbroller

   eller

   Klicka på **[!UICONTROL Cancel]** för att stänga listan över jobbrollsdistribution och återgå till scenariot.

1. Klicka på rutan **[!UICONTROL Financial]** i planens huvud för att lägga till budgeten för den här planen.

   Information om [!UICONTROL Financial]-rutevisningen.

   >[!TIP]
   >
   >Valutan som [!DNL Workfront] använder för den här planen visas inom parentes i rutans namn.

1. Ange **[!UICONTROL Yearly budget]**.

   >[!NOTE]
   >
   >Om din plan sträcker sig över flera år måste du ange ett budgetbelopp för varje år.

1. Tryck på Retur för att spara den årliga budgeten och sedan [!UICONTROL Tab] för att gå till nästa år.

   Den årliga budgeten fördelas automatiskt jämnt för varje månad under det valda året.

1. Klicka på **[!UICONTROL Advanced]** för att visa den månatliga budgetfördelningen. De årliga och månadsvisa budgetarna är alltid avrundade tal. När budgetbeloppet inte kan fördelas jämnt på alla månader inom ett år på grund av decimaler visas en **[!UICONTROL Remaining]**-indikator under den årliga budgetfördelningen.

   ![Avancerade och återstående länkar](assets/adanced-and-remaining-links-on-plan-budget-350x507.png)

1. Justera månadsbudgeten manuellt för att eliminera de belopp som överskrider gränsen.

   När summan av alla månadsbudgetbelopp är större än den årliga budgeten visas en **[!UICONTROL Exceeding]**-varningsindikator under den årliga budgetfördelningen. Justera månadsbudgetbeloppen manuellt tills de är lika med eller lägre än den tillgängliga budgeten för planen.

   ![Budgetvarning överskrids](assets/exceeding-budget-warning-on-plan-350x483.png)

1. Inaktivera inställningen **[!UICONTROL Include people costs]** för att exkludera kostnader som är associerade med jobbroller från att räknas mot planens totala kostnad. Fasta kostnader räknas alltid in i planens totala kostnad. Den här inställningen är aktiverad som standard och påverkar alla scenarier i planen.
1. Klicka var som helst utanför rutan [!UICONTROL Financial] för att stänga den. Informationen som du angav sparas automatiskt.

   Nu kan du börja skapa initiativ för planen och lägga till scenarier.

1. (Rekommenderas) Klicka på **[!UICONTROL New initiative]** om du vill lägga till ett nytt initiativ.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: Should this include information on how to create scenarios - see also information about scenarios in Manage Plans?)</p>
   -->

   Mer information om hur du lägger till initiativ finns i artikeln [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. (Valfritt) Skapa en kopia av det befintliga scenariot för att skapa ett nytt scenario för samma plan. Mer information om hur du skapar och arbetar med flera scenarier finns i [Skapa och jämföra planscenarier i  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).
1. Klicka på **[!UICONTROL Save Plan]**.

   Din plan skapas eller uppdateras.

1. (Valfritt) Klicka på ikonen **[!UICONTROL Favorites icon]** ![Favoriter](assets/favorites-icon-small.png) till höger om plannamnet för att lägga till planen i din favoritlista.

1. (Valfritt) Kopiera URL:en för planen och skicka den till andra användare som kan behöva granska eller uppdatera den. De måste ha minst [!UICONTROL View] åtkomst på åtkomstnivån för att kunna visa planen. De måste ha [!UICONTROL Edit]-åtkomst för att kunna redigera det. Om de måste granska ekonomisk information om planen, som budgetar, kostnader och jobbrollstariffer, måste de också ha tillgång till [!UICONTROL Financial Data] på sin åtkomstnivå. Mer information om åtkomsten som krävs för [!DNL Scenario Planner] finns i [Åtkomst som behövs för att använda  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).
