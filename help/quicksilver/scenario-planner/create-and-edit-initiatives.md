---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Skapa och redigera initiativ i scenarioplaneraren
description: När du använder Adobe Workfront Scenarioplan kan du skapa initiativ i en plan som du har skapat eller som delats med dig. Genom att skapa initiativ kan du visa hur mindre organisationsenheter bidrar till att slutföra planen. Om din organisation till exempel har en plan för de kommande tre åren att expandera till en ny marknad, kan du skapa initiativ inom den här planen för varje avdelning för att uppskatta varje avdelnings behov av personal och budget för att kunna genomföra den här planen.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: aa2e9a012a60ab10e2d027dedae520b5e06686c7
workflow-type: tm+mt
source-wordcount: '1547'
ht-degree: 0%

---

# Skapa och redigera initiativ i [!DNL Scenario Planner]

<!--Audited: 07/2024-->

När du använder [!UICONTROL Adobe Workfront Scenario Planner] kan du skapa initiativ i en plan som du har skapat eller som delats med dig. Genom att skapa initiativ kan du visa hur mindre organisationsenheter bidrar till att slutföra planen. Om din organisation till exempel har en plan för de kommande tre åren att expandera till en ny marknad, kan du skapa initiativ inom den här planen för varje avdelning för att uppskatta varje avdelnings behov av personal och budget för att kunna genomföra den här planen.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] package</p> </td> 
   <td> 
   <p>Workfront Ultimate</p>
<p><b>ANMÄRKNING</b></p>
<p>Kontakta Workfront om du har ett annat Workfront-paket.</p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens</p> </td> 
   <td> <p>[!UICONTROL Light] eller högre</p> 
   <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
    <tr> 
   <td>Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> </td> 
  </tr> 
 </tbody> 
</table>

Mer information om åtkomst till scenarioplanen finns i [Åtkomst krävs för att använda  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

Mer information om Workfront åtkomstkrav finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <ul></li>
   <li><p>New: Ultimate </p></li>
   <p>The Scenario Planner is not available for the new Workfront Select or Workfront Prime plans. </p>
   <li><p>Current: [!UICONTROL Business] or higher</p></ul>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] license*</p> </td> 
   <td> <p>New: Light or higher</p> 
   <p>Current: [!UICONTROL Review] or higher</p> </td> 
  </tr> 
  <tr> 
   <td>Product* </td> 
   <td> <ul><li><p>For the new Workfront plans:</p><p> Adobe Workfront</li></p>
   <li><p>For the current Workfront plans: </p>
   <p>Adobe Workfront</p> <p>Adobe Workfront Scenario Planner</p></li></ul>
   
   <p>For more information, see <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Access needed to use the [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Access level </td> 
   <td> <p>[!UICONTROL Edit] access to the [!DNL Scenario Planner]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Object permissions </p> </td> 
   <td> <p>[!UICONTROL Manage] permissions to a plan</p> <p>For information on requesting additional access to a plan, see <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Request access to a plan in the [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>-->

## Förutsättningar

Du måste skapa en plan, annars måste en annan användare dela en plan med dig innan du kan skapa ett initiativ i den planen. Mer information om hur du skapar planer finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Mer information om vilka initiativ som är tillgängliga finns i [Översikt över initiativ i  [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Skapa initiativ

Du kan skapa initiativ på följande sätt:

* Från scratch.
* Genom att importera projekt till en plan

  Mer information om hur du importerar projekt som initiativ i en plan finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Genom att kopiera befintliga initiativ.

  Mer information om kopieringsinitiativ finns i [Kopiera initiativ i  [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Så här skapar du helt nya initiativ:

{{step1-to-scenario-planner}}

1. Klicka på namnet på den plan som du vill skapa ett initiativ för.
1. Klicka på ikonen **+** till vänster om **[!UICONTROL New initiative]**

   eller

   Klicka på listrutan **[!UICONTROL New initiative]** och välj antingen **[!UICONTROL New initiative]** eller **[!UICONTROL Import Projects].**

1. Skriv in ett namn för din initiativ i fältet **[!UICONTROL Untitled Initiative]** och tryck sedan på Retur eller klicka någon annanstans på sidan.

   Initiativet visas på tidslinjen i planen, som ett blått fält. Som standard är ett initiativ en månad och börjar alltid på planens första månad.

1. (Valfritt) Dra separationsfältet mellan den vänstra panelen och tidslinjen för att ändra storlek på den vänstra panelen.

1. (Valfritt) Dra i slutet av initiativfältet för att förlänga det till mer än en månad och släpp det där du vill att initialets slutmånad ska vara.
1. (Valfritt och villkorligt) Om initiativets längd är kortare än planens drar och släpper du det i en annan position på tidslinjen i planen för att flytta det till en annan tidsram.

   ![Flytta initiativ på tidslinjen](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Du kan bara välja en varaktighet i månader. Längden på ett initiativ som du skapar från grunden kan aldrig överstiga planens varaktighet.

1. (Valfritt) Välj något av följande alternativ i listrutan **[!UICONTROL Month]** för att ändra tidslinjen för planen:

   | Nedrullningsbart menyalternativ | Beskrivning |
   |---|---|
   | [!UICONTROL Month] | Visar tidslinjen per månad. Det här är standardalternativet för en ettårsplan. |
   | [!UICONTROL Quarter] | Visar tidslinjen per kvartal. Det här alternativet är endast tillgängligt när [!UICONTROL Duration] för planen är 3 eller 5 år. Det här är standardalternativet för en 3-årsplan. |
   | [!UICONTROL Year] | Visar tidslinjen per år. Det här alternativet är endast tillgängligt när [!UICONTROL Duration] för planen är fem år. Det här är standardalternativet för en femårsplan. |


1. (Valfritt) Rulla från vänster till höger för att se hela tiden för initiativet.
1. (Valfritt) Klicka på indikatorraden **[!UICONTROL Today]** om du vill återgå till det aktuella datumet.

   ![Aktuell indikator](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Om din plan finns i framtiden eller tidigare och inte innehåller aktuellt datum visas inte Dagsindikatorn.

1. Klicka på ett initiativ. Panelen Initiativinformation öppnas till höger.

   ![Panelen Initiativinformation](assets/initiative-details-panel-multiple-months-350x626.png)

   Ange eller granska följande information:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Initiativvaraktighet</td> 
      <td>Initiativets längd i månader. </td> 
     </tr> 
     <tr data-mc-conditions=""> 
      <td role="rowheader">Start- och slutdatum</td> 
      <td>Initiativets start- och slutdatum.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">Sektion för obligatoriska jobbroller </td> 
      <td> <p>Klicka på fältet <strong>[!UICONTROL Start typing job role]</strong> och välj en roll i listan eller börja skriva namnet på en <span>n aktiv</span>-jobbroll. </p> <p><span>Beroende på om planen är inställd på att använda heltidsanställda eller timmar, </span> lägger du till antalet jobbroller som krävs för det här initiativet i <span><span>FTE eller timmar</span></span><span> för varje månad i initiativet</span>. <span>De tre första månaderna av initialvisningen som standard.</span></p> <p><span>Om du uppdaterar jobbrollsinformationen för initiativet uppdateras även den obligatoriska jobbrollsinformationen för planen.</span> </p> <p>Mer information om hur du konfigurerar planen för att använda FTE eller timmar finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i [!DNL Scenario Planner]</a>. </p>
      <p><b>VIKTIGT</b></p>  
      <p>För alla beräkningar i [!DNL Scenario Planner] använder [!DNL Workfront] följande värde: 1 FTE = 8 timmar. </p>

   <p><b>TIPS</b></p>

   <ul> 
       <li> <p><span>Använd tangenten [!UICONTROL Tab] för att gå till nästa månad.</span> </p> </li> 
      <li> <p> Alla <span>aktiva</span> jobbroller i systemet visas när du klickar på det här fältet. </p> </li> 
       <li> <p>De jobbroller som redan har lagts till i tillgängliga jobbroller för planen visas först. Mer information om hur du lägger till tillgängliga jobbroller i en plan finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplanen</a>. </p> </li> 
       <li> <p>[!DNL Workfront] heltidsmotsvarigheten är 160 timmar per månad. </p> <p>För alla beräkningar i Scenarioplaneraren använder Workfront följande värde: 1 FTE = 8 timmar. </p></li> 
      </ul> </p> <p>Du kan ange ett tal som är lägre än 1 FTE eller decimaltal för FTE <span> eller</span> <span>hours</span>. Till exempel innebär en konsult på 0,5 timmar att en konsult skulle ägna hälften av sin heltidsanställd (vanligtvis 4 timmar, där 8 timmar är 1 heltidsanställd) åt att arbeta med detta initiativ. </p>  </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Kostnadssektion</td> 
      <td> <p>De totala kostnaderna för den initiala visningen till höger om avsnittet [!UICONTROL Costs]. [!DNL Workfront] beräknar kostnaderna för ett initiativ med hjälp av följande formel:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>I fältet <strong>[!UICONTROL Fixed Costs]</strong> anger du manuellt en grov uppskattning av vad du tror kommer att kosta att slutföra det här initiativet. Detta ska inte omfatta kostnader i samband med de roller som initiativet beräknas ha.</p> <p><span>Ange ett belopp för varje månad i initiativet genom att gå från en månad till nästa när du använder tabbtangenten.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Beroende på om planen är konfigurerad att använda FTE eller timmar, använder [!UICONTROL Workfront] följande formler för att beräkna [!UICONTROL People Cost]:</p> 
        <ul> 
         <li> <p>När FTE används: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, där 160 är det totala antalet arbetstimmar per månad. </p> </li> 
         <li> <p style="font-weight: normal;">Vid användning av timmar: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Mer information om hur du konfigurerar planen för att använda timmar eller heltidsanställda finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplanen</a>.</p> </li> 
        </ul> 
        <p>Personkostnader beräknas i den basvaluta som har valts i inställningarna för valutakurser. Mer information om valutakurser finns i <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Konfigurera valutakurser</a>.</p> 
        <p>Om du uppdaterar kostnadsinformationen för ett initiativ uppdateras även området [!UICONTROL Costs] för planen. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">När du har definierat den jobbroll och de kostnadsvärden som krävs för ditt initiativ och du har ändrat dess varaktighet kan ett av följande scenarier inträffa:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Om du förkortar initiativet tar [!DNL Workfront] bort den mängd resurser som krävs och de kostnader som är associerade med den tid som tagits bort från planen. Jobbrollerna finns kvar i planen, men de har ingen nödvändig FTE eller <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">timmar</span>. De tillgängliga resurserna för planen och budgeten förblir oförändrade.<br>Mer information om planen finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Om du tar initiativet längre måste du ange antalet nya roller och kostnader för de nya månaderna i initiativet. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] section</td> 
      <td>I avsnittet <strong>[!DNL Net Value]</strong> anger du manuellt ett grovt uppskattningsbelopp i fältet <strong>[!UICONTROL Planned Benefit]</strong>. Detta är vad ni tror att fördelarna med att uppnå detta initiativ kommer att vara. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Om du redan har definierat antalet jobbroller och budgeten för din plan, antalet jobbroller och kostnaderna för det initiativ du redigerar och för alla initiativ ovan, och alla överstiger de belopp som du har angett för planen, kan [!DNL Workfront] upptäcka att du inte har tillräckligt med resurser för att slutföra initiativet. [!DNL Workfront] markerar detta som en konflikt när det försöker genomföra det här initiativet och visar det som ett rött fält. Alla initiativ som följer det motstridiga initiativet visas i röd bakgrund. Du kan behöva justera en del av behoven i dina satsningar, från den första som inte har tillräckliga resurser. Mer information om hur du justerar initiativ som står i konflikt finns i [Lös initialkonflikter i  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Valfritt) Hovra över namnet på en jobbroll och klicka sedan på ikonen **[!UICONTROL trash can icon]** ![Ta bort](assets/delete.png) för att ta bort den från initiativet.

1. (Villkorligt) Klicka på **[!UICONTROL Apply]** om du har gjort ändringar i initiativet.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Villkorligt) Om du inte har gjort några ändringar klickar du på ikonen **X** i det övre högra hörnet av panelen med initialinformation för att stänga den.
1. (Valfritt) Uppdatera prioriteten för dina initiativ.

   Mer information om hur du prioriterar initiativ finns i [Uppdatera initialprioriteringar i scenarioplanen](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Initiativ som listas först i listan har högre prioritet och får resurser före initiativen som listas nedan.

1. Klicka på **[!UICONTROL Save plan]**.

   Initiativet ingår nu i din plan.

   Mer information om hur du tar bort initiativ från en plan finns i [Ta bort initiativ i  [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
