---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Skapa och redigera initiativ i Scenarioplaneraren
description: När du använder Adobe Workfront Scenarioplan kan du skapa initiativ i en plan som du har skapat eller som delats med dig. Genom att skapa initiativ kan du visa hur mindre organisationsenheter bidrar till att slutföra planen. Om din organisation till exempel har en plan för de kommande tre åren att expandera till en ny marknad, kan du skapa initiativ inom den här planen för varje avdelning för att uppskatta varje avdelnings behov av personal och budget för att kunna genomföra den här planen.
author: Alina
feature: Workfront Scenario Planner
exl-id: a811bad0-d3c0-4cba-8b78-d9a14ffc8482
source-git-commit: 6c5be4dccff46abbed104f1f1b3c958aaf74d629
workflow-type: tm+mt
source-wordcount: '1563'
ht-degree: 0%

---

# Skapa och redigera i [!DNL Scenario Planner]

När du använder [!UICONTROL Adobe Workfront Scenario Planner]kan du skapa initiativ i en plan som du har skapat eller som delats med dig. Genom att skapa initiativ kan du visa hur mindre organisationsenheter bidrar till att slutföra planen. Om din organisation till exempel har en plan för de kommande tre åren att expandera till en ny marknad, kan du skapa initiativ inom den här planen för varje avdelning för att uppskatta varje avdelnings behov av personal och budget för att kunna genomföra den här planen.

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
   <td> <p>[!DNL Adobe Workfront] licens* </p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln. </p> <p>Mer information om hur du får [!DNL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Konfigurationer på åtkomstnivå* </td> 
   <td> <p>[!UICONTROL Edit] åtkomst eller högre till [!DNL Scenario Planner]</p> <p>Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL Manage] behörigheter till en plan</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Kontakta [!DNL Workfront] administratör.

## Förutsättningar

Du måste skapa en plan, annars måste en annan användare dela en plan med dig innan du kan skapa ett initiativ i den planen. Mer information om att skapa planer finns i [Skapa och redigera planer i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md).

Mer information om vilka initiativ som är tillgängliga finns i [Översikt över initiativen i [!DNL Scenario Planner]](../scenario-planner/initiatives-overview.md).

## Skapa initiativ

Du kan skapa initiativ på följande sätt:

* Från scratch.
* Genom att importera projekt till en plan

   Mer information om hur du importerar projekt som initiativ i en plan finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Genom att kopiera befintliga initiativ.

   Mer information om kopieringsinitiativ finns i [Kopiera initiativ i [!DNL Scenario Planner]](../scenario-planner/copy-initiatives.md).

Så här skapar du helt nya initiativ:

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png)och sedan klicka [!UICONTROL Scenarios].

1. Klicka på namnet på den plan som du vill skapa ett initiativ för.
1. Klicka på **+ ikon** till vänster om **[!UICONTROL New initiative]**

   eller

   Klicka på **[!UICONTROL New initiative]** nedrullningsbar meny och välj antingen **[!UICONTROL New initiative]** eller **[!UICONTROL Import Projects].**

1. Skriv in ett namn på ditt initiativ i **[!UICONTROL Untitled Initiative]** och sedan trycka på Enter eller klicka någon annanstans på sidan.

   Initiativet visas på tidslinjen i planen, som ett blått fält. Som standard är ett initiativ en månad och börjar alltid på planens första månad.

1. (Valfritt) Dra separationsfältet mellan den vänstra panelen och tidslinjen för att ändra storlek på den vänstra panelen.

1. (Valfritt) Dra i slutet av initiativfältet för att förlänga det till mer än en månad och släpp det där du vill att initialets slutmånad ska vara.
1. (Valfritt och villkorligt) Om initiativets längd är kortare än planens drar och släpper du det i en annan position på tidslinjen i planen för att flytta det till en annan tidsram.

   ![](assets/move-initiative-back-and-forth-on-the-timeline-350x71.png)

   >[!IMPORTANT]
   >
   >Du kan bara välja en varaktighet i månader. Längden på ett initiativ som du skapar från grunden kan aldrig överstiga planens varaktighet.

1. (Valfritt) Från **[!UICONTROL Month]** väljer du något av följande alternativ för att ändra tidslinjen för planen:

   | Nedrullningsbart menyalternativ | Beskrivning |
   |---|---|
   | [!UICONTROL Month] | Visar tidslinjen per månad. Det här är standardalternativet för en ettårsplan. |
   | [!UICONTROL Quarter] | Visar tidslinjen per kvartal. Det här alternativet är bara tillgängligt när [!UICONTROL Duration] för planen är 3 eller 5 år. Det här är standardalternativet för en 3-årsplan. |
   | [!UICONTROL Year] | Visar tidslinjen per år. Det här alternativet är bara tillgängligt när [!UICONTROL Duration] av planen är fem år. Det här är standardalternativet för en femårsplan. |


1. (Valfritt) Rulla från vänster till höger för att se hela tiden för initiativet.
1. (Valfritt) Klicka på **[!UICONTROL Today]** indikatorrad som återgår till aktuellt datum.

   ![](assets/today-indicator-350x160.png)

   >[!TIP]
   >
   >Om din plan finns i framtiden eller tidigare och inte innehåller aktuellt datum visas inte Dagsindikatorn.

1. Klicka på ett initiativ. Panelen Initiativinformation öppnas till höger.

   ![](assets/initiative-details-panel-multiple-months-350x626.png)

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
      <td> <p>Klicka på <strong>[!UICONTROL Start typing job role]</strong> och välj en roll i listan eller börja skriva namnet på en<span>n aktiv</span> jobbroll. </p> <p><span>Beroende på om planen är konfigurerad för att använda heltidsanställda eller timmar,</span> lägg till antalet jobbroller som krävs för det här initiativet i heltidsanställda <span><span>eller timmar</span></span><span> för varje månad i initiativet</span>. <span>Initiativets första tre månader visas som standard.</span></p> <p><span>Om du uppdaterar jobbrollsinformationen för initiativet uppdateras även den obligatoriska jobbrollsinformationen för planen.</span> </p> <p>Information om hur du konfigurerar planen för att använda heltidsanställda eller timmar finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i [!DNL Scenario Planner]</a>. </p> <p>Tips:  
        <ul> 
         <li> <p><span>Använd [!UICONTROL Tab] till nästa månad.</span> </p> </li> 
         <li> <p> Alla <span>aktiv</span> jobbroller i systemet visas när du klickar på det här fältet. </p> </li> 
         <li> <p>De jobbroller som redan har lagts till i tillgängliga jobbroller för planen visas först. Mer information om hur du lägger till tillgängliga jobbroller i en plan finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplaneraren</a>. </p> </li> 
         <li> <p>[!DNL Workfront] Parlamentet anser att en heltidsekvivalent är 160 timmar för en månad. </p> </li> 
        </ul> </p> <p>Du kan ange ett tal som är lägre än 1 FTE eller decimaltal för FTE <span>eller</span> <span data-mc-edit-date="2021-04-22T16:51:21.5923499-04:00" data-mc-editor="alinawilson" data-mc-comment=" yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:00.3159349-04:00">timmar</span>. Till exempel innebär en konsult på 0,5 timmar att en konsult skulle ägna hälften av sin heltidsanställd (vanligtvis 4 timmar, där 8 timmar är 1 heltidsanställd) åt att arbeta med detta initiativ. </p> <p>För alla beräkningar i Scenarioplaneraren använder Workfront följande värde: 1 heltidsanställd = 8 timmar. </p> </td> 
     </tr> 
     <tr> 
      <td rowspan="3" role="rowheader">Kostnadssektion</td> 
      <td> <p>De totala kostnaderna för det initiativ som visas till höger om [!UICONTROL Costs] -avsnitt. [!DNL Workfront] beräknar kostnaderna för ett initiativ med hjälp av följande formel:</p> <p><code>[!UICONTROL Initiative Costs] = [!UICONTROL Fixed Costs] + [!UICONTROL People] Costs</code> </p> </td> 
     </tr> 
     <tr> 
      <td> <p>I <strong>[!UICONTROL Fixed Costs]</strong> anger du manuellt en ungefärlig uppskattning av vad det kommer att kosta att slutföra det här initiativet. Detta ska inte omfatta kostnader i samband med de roller som initiativet beräknas ha.</p> <p><span>Ange ett belopp för varje månad i initiativet genom att gå från en månad till nästa när du använder tabbtangenten.</span> </p> </td> 
     </tr> 
     <tr> 
      <td> 
       <div> 
        <p>Beroende på om planen är konfigurerad för att använda heltidsanställda eller timmar, [!UICONTROL Workfront] använder följande formler för att beräkna [!UICONTROL People Cost]:</p> 
        <ul> 
         <li> <p>När FTE används: </p> <p><code>[!UICONTROL People Costs] = SUM(Job role hourly rate * Number of months in the Duration * 160 * Number of FTEs)</code>, där 160 är det totala antalet arbetstimmar per månad. </p> </li> 
         <li> <p style="font-weight: normal;">Vid användning av timmar: </p> <p style="font-weight: normal;"><code>Monthly People Costs = SUM(Job role hourly rate * Number of hours estimated for an initiative)</code> </p> <p style="font-weight: normal;">Mer information om hur du konfigurerar planen för att använda timmar eller heltidsanställda finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplaneraren</a>.</p> </li> 
        </ul> 
        <p>Personkostnader beräknas i den basvaluta som har valts i inställningarna för valutakurser. Mer information om valutakurser finns i <a href="../administration-and-setup/manage-workfront/exchange-rates/set-up-exchange-rates.md" class="MCXref xref">Ställ in valutakurser</a>.</p> 
        <p>Uppdateringen av kostnadsinformationen för ett initiativ uppdaterar också [!UICONTROL Costs] planens yta. </p> 
       </div> </td> 
     </tr> 
     <tr> 
      <td colspan="2" role="rowheader"> <p style="font-weight: normal;">När du har definierat den jobbroll och de kostnadsvärden som krävs för ditt initiativ och du har ändrat dess varaktighet kan ett av följande scenarier inträffa:</p> 
       <ul> 
        <li> <p style="font-weight: normal;">Om du förkortar initiativet, [!DNL Workfront] tar bort nödvändiga resurser och kostnader i samband med den tid som tagits bort från planen. Jobbrollerna finns kvar i planen, men de har inget FTE eller <span data-mc-edit-date="2021-04-19T13:46:01.5004065-04:00" data-mc-editor="alinawilson" data-mc-comment="drafted, yellow" data-mc-initials="AL" data-mc-creator="alinawilson" data-mc-create-date="2021-04-19T13:45:58.7938344-04:00">timmar</span>. De tillgängliga resurserna för planen och budgeten förblir oförändrade.<br>Information om hur du uppdaterar planen finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i [!DNL Scenario Planner]</a>. </p> </li> 
        <li> <p style="font-weight: normal;">Om du tar initiativet längre måste du ange antalet roller och kostnader för de nya månaderna i initiativet. </p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!DNL Net Value] section</td> 
      <td>I <strong>[!DNL Net Value]</strong> avsnitt, ange ett grovt uppskattningsbelopp manuellt i <strong>[!UICONTROL Planned Benefit]</strong> fält. Detta är vad ni tror att fördelarna med att uppnå detta initiativ kommer att vara. </td> 
     </tr> 
    </tbody> 
   </table>

   >[!NOTE]
   >
   >Om du redan har definierat antalet befattningar och budgeten för din plan, antalet befattningar och kostnaderna för det initiativ du redigerar och för alla initiativ ovan, och de överstiger alla de belopp du har angett för planen, [!DNL Workfront] kanske inte har tillräckligt med resurser för att slutföra initiativet. [!DNL Workfront] markerar detta som en konflikt när man försöker genomföra det här initiativet och visar det som ett rött fält. Alla initiativ som följer det motstridiga initiativet visas i röd bakgrund. Du kan behöva justera en del av behoven i dina initiativ, från den första som har otillräckliga resurser. Mer information om hur du justerar initiativ som orsakar konflikter finns i [Lös initialkonflikter i [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md).

1. (Valfritt) Håll muspekaren över namnet på en jobbroll och klicka sedan på knappen **[!UICONTROL trash can icon]** ![](assets/delete.png) att ta bort det från initiativet.

1. (Villkorligt) Om du har ändrat i initiativet klickar du på **[!UICONTROL Apply]**.

   <!--
   <MadCap:conditionalText data-mc-conditions="QuicksilverOrClassic.Draft mode">
   (NOTE: Add more steps here as you can do more in the Initiative box over time)
   </MadCap:conditionalText>
   -->

1. (Villkorligt) Om du inte har gjort några ändringar klickar du på **X** ikonen i det övre högra hörnet av panelen med information om initiativ för att stänga den.
1. (Valfritt) Uppdatera prioriteten för dina initiativ.

   Mer information om att prioritera initiativ finns i [Uppdatera initiala prioriteringar i scenarioplanen](../scenario-planner/prioritize-initiatives.md).

   >[!TIP]
   >
   >Initiativ som listas först i listan har högre prioritet och får resurser före initiativen som listas nedan.

1. Klicka på **[!UICONTROL Save plan]**.

   Initiativet ingår nu i din plan.

   Mer information om hur du tar bort initiativ från en plan finns i [Ta bort initiativ i [!DNL Scenario Planner]](../scenario-planner/delete-initiatives.md).
