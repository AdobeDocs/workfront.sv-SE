---
product-area: enterprise-scenario-planner-product-area
keywords: publicera,planer,projekt,scenario,scenarier
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Uppdatera eller skapa projekt genom att publicera initiativ i Scenarioplanen
description: Du kan skapa projekt från befintliga initiativ och uppdatera projekt som tidigare länkats till initiativ genom att publicera scenarier i Adobe Workfront Scenarioplan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: e152c20e7b987f4bef7ffd6ee534c059f7b9bf45
workflow-type: tm+mt
source-wordcount: '1580'
ht-degree: 0%

---

# Uppdatera eller skapa projekt genom att publicera i [!DNL Scenario Planner]

Publicera ett scenario från [!DNL Adobe Workfront Scenario Planner] innebär följande:

* Skapar projekt från satsningarna på scenariot och länkar samman dem.
* Uppdaterar projekt som redan är kopplade till initiativ i scenariot med information från det länkade initiativet. Projekt kan också länkas till initiativ när du importerar dem till en plan. Mer information finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

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
   <td>Produkt </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du får [!DNL Workfront Scenario Planner], se <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst krävs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p></p> <p>Åtkomstnivå*</p> </td> 
   <td> 
    <ul> 
    <li>[!UICONTROL Edit] behörighet för [!DNL Scenario Planner] och projekt</li></ul>

<p><b>ANMÄRKNING</b>

Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] administratören kan ändra din åtkomstnivå, se <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td>
</tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter</p> </td> 
   <td> 
    <ul> 
     <li>[!UICONTROL Manage] behörigheter för planen </li> 
     <li>[!UICONTROL Manage] behörigheter för publicerade projekt</li> 
    </ul> <p>Mer information om hur du begär ytterligare åtkomst till projekt finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

Mer information om åtkomst till [!DNL Workfront Scenario Planner], se [Åtkomst krävs för att använda [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

## Förutsättningar

Innan du börjar:

* Du måste skapa och spara en plan innan du kan publicera initiativ från den.

## Att tänka på när det gäller att publicera projekt

* Du kan bara publicera ett scenario från en plan.
* Ett initiativ kan bara kopplas till ett projekt.
* Ett projekt kan vara kopplat till mer än ett initiativ när initiativen tillhör olika planer.

   >[!TIP]
   >
   >När ett projekt finns på flera planer och du publicerar information till projektet från alla planer, skrivs den senaste publiceringen över [!DNL Scenario Planner] information om projektet.

* Om initiativ skapades på planen genom att projekt importerades till planen uppdateras även de länkade projekten med initiativinformation när man publicerar initiativet.

   >[!TIP]
   >
   >Du kan importera samma projekt till flera planer. Publicering kan skriva över initialinformation i ett projekt som är kopplat till flera initiativ.

   Mer information om hur du skapar initiativ genom att importera projekt finns i [Importera projekt till planer i [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Ändringar som görs i projektet överförs inte till det kopplade initiativet.



## Publicera initiativ

>[!IMPORTANT]
>
>Om du ändrar några initiativ i planen, inklusive löser konflikter, måste du publicera om initiativet för att den nya informationen ska synas i projektet. Den här informationen visas endast i projekt som är kopplade till initiativ när du publicerar motsvarande initiativ. Mer information om hur du löser konflikter mellan initiativ finns i [Lös initialkonflikter i [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Workfront och klicka sedan på **[!UICONTROL Scenarios]**
1. (Valfritt och villkorligt) Om du vill publicera från en befintlig plan klickar du på **[!UICONTROL Filter]** icon ![](assets/filter-nwepng.png) i planens övre högra hörn och välj något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Visar alla planer som du äger eller delar med dig. Detta är standardinställningen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>Visar planer som du har skapat.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>Visar planer som du inte har skapat men som delas med dig.</p> <p>Viktigt: Du måste ha [!UICONTROL Manage] behörigheter till planer som delas med dig för att kunna publicera dem. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Valfritt) Klicka på **[!UICONTROL Search]** icon ![](assets/search-icon.png) och börja skriva namnet på en plan för att snabbt hitta den i listan.
1. (Villkorligt) Skapa en plan om du vill publicera från en ny plan.

   Mer information om att skapa planer finns i [Skapa och redigera planer i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Valfritt) Klicka på namnet på en befintlig plan och skapa nya scenarier för planen.

   Mer information om hur du skapar scenarier för en plan finns i [Skapa och jämföra planscenarier i [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Valfritt) Uppdatera initiativen för en befintlig eller ny plan eller skapa nya.

   Mer information om hur du skapar initiativ finns i [Skapa och redigera i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Klicka på **[!UICONTROL Save plan]**.
1. Välj scenariot som du vill publicera i **[!UICONTROL Initial scenario]** nedrullningsbar meny och klicka sedan på **[!UICONTROL Go to Publish]** ![](assets/go-to-publish-button-icon.png) i det övre högra hörnet.

   eller

   Klicka **[!UICONTROL Compare scenarios]** hovra över det scenariokort du vill publicera från och klicka sedan på **[!UICONTROL Go to Publish]** ![](assets/go-to-publish-button-icon.png).

   The [!UICONTROL Publish initiatives] visas med en lista över alla initiativ i scenariot. Om något av initiativen redan har publicerats är projektikonen ![](assets/project-icon-sp.png) visas efter deras namn och **[!UICONTROL Last published]** datumet anges i listan.

   >[!TIP]
   >
   >Initiativ som har skapats genom att projekt har importerats visas också med en projektikon ![](assets/project-icon-sp.png) till höger om sitt namn

   ![](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Valfritt och villkorligt) Om du vill publicera från en befintlig plan klickar du på **[!UICONTROL Filter]** icon ![](assets/filter-nwepng.png) i planens övre högra hörn och välj något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Visar alla initiativ i det valda scenariot. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Published]</td> 
      <td>Visar initiativ som du eller en annan användare har publicerat tidigare. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Unpublished]</td> 
      <td> <p>Visar opublicerade initiativ. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Valfritt) Klicka på **[!UICONTROL Search]** icon ![](assets/search-icon.png) och börja skriva namnet på ett initiativ för att snabbt hitta det i listan.
1. Välj en eller flera initiativ att publicera och skapa eller uppdatera projekt från dem, och klicka sedan på **[!UICONTROL Publish initiatives]**.

   Detta skapar ett nytt projekt från varje vald initiativ eller uppdaterar befintliga kopplade projekt, om de publicerade initiativen redan var kopplade till ett projekt.

   >[!TIP]
   >
   >Nya projekt har samma namn som de publicerade initiativen.

1. (Villkorligt) Gör något av följande:

   * Om du har publicerat ett initiativ klickar du **[!UICONTROL See associated project]** att öppna det projekt som skapats eller uppdaterats från initiativet.
   * Om du har publicerat mer än ett initiativ klickar du **[!UICONTROL See associated projects]** för att öppna en lista över projekt som publicerats från initiativ. [!DNL Workfront] använder [!DNL Scenario Planner] Som standard filtreras projekt till listan med projekt. De senast publicerade projekten visas högst upp i listan.

      ![](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Gå till följande områden om du vill se information om projektet:

   * **The [!UICONTROL Updates] section**: En uppdatering publiceras som anger att projektet skapades eller uppdaterades från initiativet. Uppdateringen innehåller namnet på det initiativ som skapade eller uppdaterade projektet och det länkade namnet på den plan som innehåller initiativet. Du kan klicka på namnet på planen i uppdateringen för att öppna planen i [!DNL Scenario Planner].

      ![](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **The [!UICONTROL Overview] området på [!UICONTROL Project Details] section**: En ny [!DNL Scenario Planner] som innehåller information från det länkade initiativet.

      ![](assets/scenario-planner-on-project-details-350x135.png)

      Följande initiativinformation publiceras i [!DNL Scenario Planner] området på [!UICONTROL Project Details] avsnitt:

      <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>varaktigheten för motsvarande initiativ när projektet är kopplat till ett initiativ. Det här fältet kan inte redigeras.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span>Det datum då projektet senast offentliggjordes från ett motsvarande initiativ.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>Den första dagen i startmånaden för initiativet, när projektet är kopplat till ett initiativ.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>Den sista dagen i programmets slutmånad, när projektet är kopplat till ett initiativ. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Information om associerade jobbroller och deras tidsfördelningar för initiativet. Detta omfattar följande:</p> 
         <ul> 
          <li>Jobbrollsnamn</li> 
          <li>Antal heltidsanställda</li> 
          <li> <p>Antal timmar för alla heltidsanställda</p> <p>Du kan beräkna antalet jobbroller som behövs för din plan eller ditt initiativ med hjälp av timmar eller heltidsanställda.</p> <p>Mer information finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplaneraren</a>. </p> </li> 
         </ul> 
      <p><b>TIPS</b>

      Om antalet befattningar är olika för varje månad i initiativet visas det maximala antalet roller som krävs för initiativet i det här fältet. Om du till exempel behöver en konsult för januari och 2 för februari, visar kolumnen 2 heltidsanställda och motsvarande antal timmar för 2 heltidsanställda för alla månader.</p> </td>
      </tr> 
      </tbody> 
     </table>

      >[!NOTE]
      >
      >Alla användare med [!UICONTROL View] åtkomst till projektet kan se [!DNL Scenario Planner] i [!UICONTROL Overview] område. Du kan styra om det här området ska visas i dialogrutan [!UICONTROL Details] med hjälp av en layoutmall. Om användarna inte har någon associerad layoutmall visas det här området som standard.
      >
      >   
      >   
      >   * Mer information om hur du lägger till eller tar bort områden i [!UICONTROL Details] avsnitt med en layoutmall, se [Anpassa [!UICONTROL Details] visa med en layoutmall](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
      >   * Mer information finns i [!UICONTROL Overview] området på [!UICONTROL Project Details], se [[!UICONTROL Manage] information i projektet [!UICONTROL Overview] area](../manage-work/projects/manage-projects/understand-project-overview-area.md).


   * **The [!UICONTROL Role Allocation] i [!UICONTROL Workload Balancer] eller projektets uppgiftslista**: Information om rollfördelningen på initiativet fylls i på detta område, utöver rollfördelningen på projektet.

      Mer information finns i [Översikt över avstämning av resursallokeringar mellan projekt och initiativ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

      ![](assets/role-allocation-panel-350x174.png)

      Ändringar av datum eller resurser för projektet påverkar inte motsvarande initiativ eller något av de områden i projektet som innehåller initiativinformation.

   * **The [!UICONTROL Resource Budgeting] området på [!UICONTROL Business Case] projektet**: Ett nytt alternativ för hantering av projektresurser med [!DNL Scenario Planner] information läggs till i [!UICONTROL Resource Budgeting] området på [!UICONTROL Business Case] av projektet.

      Mer information finns i [Budgetresurser i [!UICONTROL Business Case] med [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

      ![](assets/sp-in-business-case-selected-350x110.png)

1. (Valfritt) Granska följande information i dialogrutan [!DNL Scenario Planner] efter att du har publicerat ett scenario:

   * Det publicerade scenariot blir det första när du har publicerat initiativ från det.
   * Du kan inte publicera från något annat scenario efter att du har publicerat ett scenario minst en gång.
   * The [!UICONTROL Go to Publish] Alternativet tas bort från alla andra scenarier efter att minst ett initiativ har publicerats från ett scenario.
   * En grön indikator visas bredvid de publicerade initialernas projektikoner i planen.

      ![](assets/indicator-for-published-initiative-icon-350x119.png)

   * En grön&quot;publicerad&quot; indikator visas högst upp i scenariot och på scenariokortet och fältet Publicerad fylls i på scenariokortet som anger antalet initiativ i scenariot som har publicerats.

      ![](assets/published-scenario-highlighted-350x632.png)

      >[!TIP]
      >
      >Om alla projekt som publiceras från scenariots initiativ tas bort, tas indikationen på att scenariot har publicerats bort. Mer information finns i [Ta bort projekt](../manage-work/projects/manage-projects/delete-projects.md).

1. (Valfritt) Uppdatera information om initiativet och upprepa den process som beskrivs ovan för att publicera initiativet på nytt och uppdatera information om det länkade projektet.

   Mer information om redigeringsinitiativ finns i [Skapa och redigera i [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


