---
product-area: enterprise-scenario-planner-product-area
keywords: publicera,planer,projekt,scenario,scenarier
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Uppdatera eller skapa projekt genom att publicera initiativ i Scenarioplanen
description: Du kan skapa projekt från befintliga initiativ och uppdatera projekt som tidigare länkats till initiativ genom att publicera scenarier i Adobe Workfront Scenarioplan.
author: Alina
feature: Workfront Scenario Planner
exl-id: 46d3666a-4454-4a84-8c02-a79f3947a18f
source-git-commit: 7cfe82eb703e2a043c264cf86c0e5424d1e33d78
workflow-type: tm+mt
source-wordcount: '1616'
ht-degree: 0%

---

# Uppdatera eller skapa projekt genom att publicera initiativ i [!DNL Scenario Planner]

Publicering av ett scenario från [!DNL Adobe Workfront Scenario Planner] ger följande:

* Skapar projekt från satsningarna på scenariot och länkar samman dem.
* Uppdaterar projekt som redan är kopplade till initiativ i scenariot med information från det länkade initiativet. Projekt kan också länkas till initiativ när du importerar dem till en plan. Mer information finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md)

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
   <td> <p>[!UICONTROL Edit] åtkomst för [!DNL Scenario Planner] och [!UICONTROL Projects]</p></td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td>  <ul> 
     <li>[!UICONTROL Manage] behörigheter för planen </li> 
     <li>[!UICONTROL Manage] behörigheter för publicerade projekt</li> 
    </ul> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md" class="MCXref xref">Begär åtkomst till en plan i [!DNL Scenario Planner]</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Förutsättningar

Innan du börjar:

* Du måste skapa och spara en plan innan du kan publicera initiativ från den.
* Tillåt användare att skapa projekt utan att använda en mallinställning måste vara aktiverat under Projektinställningar i Konfigurera. Mer information finns i [Konfigurera systemomfattande projektinställningar](/help/quicksilver/administration-and-setup/set-up-workfront/configure-system-defaults/set-project-preferences.md).

## Att tänka på när det gäller att publicera projekt

* Du kan bara publicera ett scenario från en plan.
* Ett initiativ kan bara kopplas till ett projekt.
* Ett projekt kan vara kopplat till mer än ett initiativ när initiativen tillhör olika planer.

  >[!TIP]
  >
  >När det finns ett projekt på flera planer och du publicerar information till projektet från alla planer, skriver den senaste publiceringen över befintlig [!DNL Scenario Planner]-information i projektet.

* Om initiativ skapades på planen genom att projekt importerades till planen uppdateras även de länkade projekten med initiativinformation när man publicerar initiativet.

  >[!TIP]
  >
  >Du kan importera samma projekt till flera planer. Publicering kan skriva över initialinformation i ett projekt som är kopplat till flera initiativ.

  Mer information om hur du skapar initiativ genom att importera projekt finns i [Importera projekt till planer i  [!DNL Scenario Planner]](../scenario-planner/import-projects-to-plans.md).

* Ändringar som görs i projektet överförs inte till det kopplade initiativet.



## Publicera initiativ

>[!IMPORTANT]
>
>Om du ändrar några initiativ i planen, inklusive löser konflikter, måste du publicera om initiativet för att den nya informationen ska synas i projektet. Den här informationen visas endast i projekt som är kopplade till initiativ när du publicerar motsvarande initiativ. Mer information om hur du löser konflikter mellan initiativ finns i [Lös initialkonflikter i  [!DNL Scenario Planner]](../scenario-planner/resolve-conflicts-in-sp.md)

{{step1-to-scenario-planner}}

1. (Valfritt och villkorligt) Om du vill publicera från en befintlig plan klickar du på **[!UICONTROL Filter]**-ikonen ![Filterikonen](assets/filter-nwepng.png) i planens övre högra hörn och väljer något av följande alternativ:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL All]</td> 
      <td>Visar alla planer som du äger eller delar med dig. Det här är standardinställningen. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL My plans]</td> 
      <td>Visar planer som du har skapat.</td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Shared with me]</td> 
      <td> <p>Visar planer som du inte har skapat men som delas med dig.</p> <p>Viktigt! Du måste ha [!UICONTROL Manage] behörigheter till planer som delas med dig för att kunna publicera dem. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   ![Alternativ i listrutan Filter](assets/plans-filters-dropdown-options-scenario-planer.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Search]** ![sök](assets/search-icon.png) och börja skriva namnet på en plan för att snabbt hitta den i listan.
1. (Villkorligt) Skapa en plan om du vill publicera från en ny plan.

   Mer information om hur du skapar planer finns i [Skapa och redigera planer i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-plans.md) .

1. (Valfritt) Klicka på namnet på en befintlig plan och skapa nya scenarier för planen.

   Mer information om hur du skapar scenarier för en plan finns i [Skapa och jämföra planscenarier i  [!DNL Scenario Planner]](../scenario-planner/create-and-compare-scenarios-for-a-plan.md).

1. (Valfritt) Uppdatera initiativen för en befintlig eller ny plan eller skapa nya.

   Mer information om hur du skapar initiativ finns i [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).

1. Klicka på **[!UICONTROL Save plan]**.
1. Välj det scenario som du vill publicera i listrutan **[!UICONTROL Initial scenario]** och klicka sedan på **[!UICONTROL Go to Publish]** ![Gå till publicering](assets/go-to-publish-button-icon.png) i det övre högra hörnet.

   eller

   Klicka på **[!UICONTROL Compare scenarios]**, hovra över det scenariokort som du vill publicera från och klicka sedan på **[!UICONTROL Go to Publish]** ![Gå till publicering](assets/go-to-publish-button-icon.png).

   Sidan [!UICONTROL Publish initiatives] visas med en lista över alla initiativ i scenariot. Om någon av initiativen har publicerats tidigare visas projektikonen ![Projektikon](assets/project-icon-sp.png) efter deras namn och datumet **[!UICONTROL Last published]** i listan.

   >[!TIP]
   >
   >Initiativ som har skapats genom import av projekt visas också med projektikonen ![Projektikon](assets/project-icon-sp.png) till höger om namnet

   ![Projektikon och det senast publicerade datumet](assets/project-icons-and-last-published-date-in-publish-initiative-page-350x63.png)

1. (Valfritt och villkorligt) Om du vill publicera från en befintlig plan klickar du på **[!UICONTROL Filter]**-ikonen ![Filterikonen](assets/filter-nwepng.png) i planens övre högra hörn och väljer något av följande alternativ:

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

   ![Initiativfilter](assets/initiatives-fitler-in-publishing-screen-scenario-planner.png)

1. (Valfritt) Klicka på ikonen **[!UICONTROL Search]** ![&#x200B; Sök &#x200B;](assets/search-icon.png) och börja skriva namnet på ett initiativ för att snabbt hitta det i listan.
1. Välj en eller flera initiativ att publicera och skapa eller uppdatera projekt från dem och klicka sedan på **[!UICONTROL Publish initiatives]**.

   Detta skapar ett nytt projekt från varje vald initiativ eller uppdaterar befintliga kopplade projekt, om de publicerade initiativen redan var kopplade till ett projekt.

   >[!TIP]
   >
   >Nya projekt har samma namn som de publicerade initiativen.

1. (Villkorligt) Gör något av följande:

   * Om du har publicerat ett initiativ klickar du på **[!UICONTROL See associated project]** för att öppna projektet som har skapats eller uppdaterats från det.
   * Om du har publicerat mer än ett initiativ klickar du på **[!UICONTROL See associated projects]** för att öppna en lista över projekt som publicerats från initiativ. [!DNL Workfront] använder filtret [!DNL Scenario Planner] Projekt på listan med projekt som standard. De senast publicerade projekten visas högst upp i listan.

     ![Scenarioplanering efter publiceringsinitiativ](assets/scenario-planner-filter-after-publishing-initiatives-350x81.png)

1. Gå till följande områden om du vill se information om projektet:

   * **Avsnittet [!UICONTROL Updates]**: En uppdatering publiceras som anger att projektet skapades eller uppdaterades från initiativet. Uppdateringen innehåller namnet på det initiativ som skapade eller uppdaterade projektet och det länkade namnet på den plan som innehåller initiativet. Du kan klicka på namnet på planen i uppdateringen för att öppna planen i [!DNL Scenario Planner].

     ![Uppdatera bekräftelse av publiceringsström](assets/update-stream-confirmation-of-publish-on-project-350x65.png)

   * **Området [!UICONTROL Overview] i [!UICONTROL Project Details] avsnittet**: Ett nytt [!DNL Scenario Planner]-avsnitt skapas i det här området som innehåller information från det länkade initiativet.

     ![Scenarioplanering för projektinformation](assets/scenario-planner-on-project-details-350x135.png)

     Följande initialinformation publiceras i området [!DNL Scenario Planner] i avsnittet [!UICONTROL Project Details]:

     <table style="table-layout:auto"> 
      <col> 
      <col> 
      <tbody> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Duration]</span> </td> 
        <td><span>Det motsvarande initiativets varaktighet när projektet är kopplat till ett initiativ. Det här fältet kan inte redigeras.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Last Published Date]</span> </td> 
        <td><span>Datumet då projektet senast publicerades från ett motsvarande initiativ.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Start Date]</span> </td> 
        <td><span>Den första dagen i startmånaden för initiativet, när projektet är kopplat till ett initiativ.</span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative End Date]</span> </td> 
        <td><span>Den sista dagen i initialets slutmånad, när projektet är kopplat till ett initiativ. </span> </td> 
       </tr> 
       <tr> 
        <td role="rowheader"><span>[!UICONTROL Initiative Job Roles in FTEs and Hours]</span> </td> 
        <td> <p>Information om de associerade jobbrollerna och deras tidsfördelningar för initiativet. Detta omfattar följande:</p> 
         <ul> 
          <li>Jobbrollsnamn</li> 
          <li>Antal heltidsanställda</li> 
          <li> <p>Antal timmar för alla heltidsanställda</p> <p>Du kan beräkna antalet jobbroller som behövs för din plan eller ditt initiativ med hjälp av timmar eller heltidsanställda.</p> <p>Mer information finns i <a href="../scenario-planner/create-and-edit-plans.md" class="MCXref xref">Skapa och redigera planer i scenarioplanen</a>. </p> </li> 
         </ul> 
      <p><b>TIPS</b>

     Om antalet befattningar är olika för varje månad i initiativet visas det maximala antalet roller som krävs för initiativet i det här fältet. Om du till exempel behöver en konsult för januari och 2 för februari, visar kolumnen 2 heltidsanställda och motsvarande antal timmar för 2 heltidsanställda för alla månader.</p> </td>
     </tr> 
      </tbody> 
     </table>

     >[!NOTE]
     >
     >Alla användare med [!UICONTROL View]-åtkomst till projektet kan se avsnittet [!DNL Scenario Planner] i området [!UICONTROL Overview]. Du kan styra om det här området ska visas i avsnittet [!UICONTROL Details] med hjälp av en layoutmall. Om användarna inte har någon associerad layoutmall visas det här området som standard.
     >
     >   
     >   
     >   * Mer information om hur du lägger till eller tar bort områden i avsnittet [!UICONTROL Details] med hjälp av en layoutmall finns i [Anpassa vyn [!UICONTROL Details] med hjälp av en layoutmall](../administration-and-setup/customize-workfront/use-layout-templates/customize-details-view-layout-template.md).
     >   * Mer information om hur du visar information i området [!UICONTROL Overview] i [!UICONTROL Project Details] finns i [[!UICONTROL Manage] -information i projektområdet [!UICONTROL Overview] &#x200B;](../manage-work/projects/manage-projects/understand-project-overview-area.md).
     >   
     >

   * **Panelen [!UICONTROL Role Allocation] i [!UICONTROL Workload Balancer] eller aktivitetslistan för projektet**: Information om rollallokering för initiativet fylls i i det här området, förutom rollallokeringar för projektet.

     Mer information finns i [Översikt över att stämma av resursallokeringar mellan projekt och initiativ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

     ![Rollallokeringspanelen](assets/role-allocation-panel-350x174.png)

     Ändringar av datum eller resurser för projektet påverkar inte motsvarande initiativ eller något av de områden i projektet som innehåller initiativinformation.

   * **Området [!UICONTROL Resource Budgeting] i [!UICONTROL Business Case] projektet**: Ett nytt alternativ för att hantera projektresurser med hjälp av [!DNL Scenario Planner]-information läggs till i [!UICONTROL Resource Budgeting]-området i [!UICONTROL Business Case] för projektet.

     Mer information finns i [Budgetresurser i [!UICONTROL Business Case] med  [!DNL Scenario Planner]](../manage-work/projects/define-a-business-case/budget-resources-in-business-case-use-scenario-planner.md).

     ![Scenarioplanering i affärsfall](assets/sp-in-business-case-selected-350x110.png)

1. (Valfritt) Granska följande information i [!DNL Scenario Planner] när du har publicerat ett scenario:

   * Det publicerade scenariot blir det första när du har publicerat initiativ från det.
   * Du kan inte publicera från något annat scenario efter att du har publicerat ett scenario minst en gång.
   * Alternativet [!UICONTROL Go to Publish] tas bort från alla andra scenarier efter att minst ett initiativ har publicerats från ett scenario.
   * En grön indikator visas bredvid de publicerade initialernas projektikoner i planen.

     ![Indikator för publicerat initiativ](assets/indicator-for-published-initiative-icon-350x119.png)

   * En grön&quot;publicerad&quot; indikator visas högst upp i scenariot och på scenariokortet och fältet Publicerad fylls i på scenariokortet som anger antalet initiativ i scenariot som har publicerats.

     ![Publicerat scenario](assets/published-scenario-highlighted-350x632.png)

     >[!TIP]
     >
     >Om alla projekt som publiceras från scenariots initiativ tas bort, tas indikationen på att scenariot har publicerats bort. Mer information finns i [Ta bort projekt](../manage-work/projects/manage-projects/delete-projects.md).

1. (Valfritt) Uppdatera information om initiativet och upprepa den process som beskrivs ovan för att publicera initiativet på nytt och uppdatera information om det länkade projektet.

   Mer information om redigeringsinitiativ finns i [Skapa och redigera initiativ i  [!DNL Scenario Planner]](../scenario-planner/create-and-edit-initiatives.md).


