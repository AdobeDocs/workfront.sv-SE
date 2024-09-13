---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visa rolltilldelning för projekt och initiativ i Utjämning av arbetsbelastning
description: När du har kopplat projekt och initiativ kan du hantera deras resurstilldelning sida vid sida för att säkerställa att de
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: bbc3ac852dae3d9a503b4585dfc229d43c9aed28
workflow-type: tm+mt
source-wordcount: '741'
ht-degree: 0%

---

# Visa rollallokering för projekt och initiativ i [!UICONTROL Workload Balancer]

<!--Audited: 07/2024-->

När du har kopplat projekt och initiativ kan du hantera deras resurstilldelning sida vid sida för att säkerställa att de matchar. På så sätt undviker du att överallokera eller underutnyttja dem.

I den här artikeln beskrivs hur du kan stämma av resurser med hjälp av panelen [!UICONTROL Role Allocation] i [!UICONTROL Workload Balancer] för ett projekt.

Allmän information om hur du förenar resurser mellan projekt och initiativ, inklusive förutsättningar, finns i [Översikt över att stämma av resursallokeringar mellan projekt och initiativ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

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
   <td> <p>Visa eller öka åtkomsten till projekt.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p> Visa eller ge högre behörighet till ett projekt.</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa rollallokering för projekt och initiativ i [!UICONTROL Workload Balancer]

Om ditt företag har köpt en [!DNL Workfront Scenario Planner]-licens kan du stämma av resursallokeringarna mellan initiativet och det projekt som är länkat till det på projektnivå [!UICONTROL Workload Balancer].

1. (Villkorligt) Koppla ett projekt till ett projekt med en av de metoder som beskrivs i följande artiklar:

   * [Importera projekt till planer i  [!DNL Adobe Workfront Scenario Planner]](import-projects-to-plans.md).
   * [Uppdatera eller skapa projekt genom att publicera initiativ i  [!DNL Adobe Workfront Scenario Planner]](publish-scenarios-update-projects.md).

   >[!IMPORTANT]
   >
   >Om ni ändrar resurser i initiativet måste ni på nytt publicera det scenario som initiativet hör till för att få den senaste resursinformationen från initiativet som ska uppdateras i projektet.

1. Gå till det projekt där du vill granska fördelningen av jobbroller för projektet samt för det associerade initiativet.
1. Klicka på [!UICONTROL Workload Balancer] i den vänstra panelen.

   Du kan behöva klicka på **[!UICONTROL Scheduling]** och sedan på **[!UICONTROL Switch to Workload Balancer]**.

1. Gör något av följande:

   * Klicka på **[!UICONTROL Month]** om du vill visa arbetsbelastningsutjämnaren per månad, klicka på listrutan bredvid en månad i tidslinjen ![](assets/drop-down-next-to-month-month-view-wb.png) och klicka sedan på **[!UICONTROL More]**.
   * Klicka på ikonen **[!UICONTROL Show role allocation]** ![](assets/show-role-allocation-icon.png) i det övre högra hörnet av verktygsfältet.

   Panelen [!UICONTROL Role Allocation] visas.

   ![](assets/role-allocation-panel-months-collapsed-350x319.png)

   >[!CAUTION]
   >
   >Även om du kan visa panelen [!UICONTROL Role Allocation] även om din organisation inte har köpt någon [!DNL Workfront Scenario Planner]-licens, kan du inte visa information om satsningarnas jobbroller.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Granska följande information i området **[!UICONTROL Project Totals]** på panelen Rollallokering:

   <table style="table-layout:auto"> 
    <col> 
    <col> 
    <tbody> 
     <tr> 
      <td role="rowheader">[!UICONTROL Job Role]</td> 
      <td> <p>Namnen på de jobbroller som är associerade med något av följande:</p> 
       <ul> 
        <li> <p>uppgifter i projektet</p> </li> 
        <li> <p>frågor om projektet</p> </li> 
        <li> <p>initiativ som är kopplat till projektet</p> </li> 
       </ul> </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Initiative Hours]</td> 
      <td>Antalet timmar som krävs för varje arbetsroll i initiativet under hela den tid som initiativet pågår. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Planned Hours]</td> 
      <td>Antal planerade timmar som associeras med varje jobbroll i aktiviteterna eller utleveranser i projektet under projektets totala längd. </td> 
     </tr> 
     <tr> 
      <td role="rowheader">[!UICONTROL Variance]</td> 
      <td> <p>Skillnaden mellan de timmar som krävs för initiativet och de planerade timmarna i samband med arbete i projektet. [!DNL Workfront] beräknar [!UICONTROL Variance] med den här formeln:</p> <p><code>Role Allocation Variance = Initiative Hours - Planned Hours</code> </p> <p>När resurser planeras för fler timmar än vad som krävs för initiativet, är [!UICONTROL Variance] negativ och visas i rött. Det innebär att era resurser är överallokerade. </p> </td> 
     </tr> 
    </tbody> 
   </table>

   >[!TIP]
   >
   >Planerade timmar från projektet visas inte i följande scenarier:
   >
   >   
   >   
   >   * När uppgifter eller utgåvor inte har tilldelats till jobbroller, eller användare med en jobbroll som är kopplad till dem.
   >   * När aktiviteter eller utgåvor har [!UICONTROL Duration] som är noll.
   >   
   >

1. (Valfritt) Om kolumnen [!UICONTROL Variance] visar att dina resurser är överallokerade justerar du något av följande:

   * Minska antalet planerade timmar för en jobbroll som visar överallokerade eller lägg till fler resurser för aktiviteterna och distribuera fler planerade timmar till de nya resurserna. Du kan uppdatera uppdrag eller antalet planerade timmar för uppgifter eller problem när du redigerar dem. Mer information finns i följande artiklar:

      * [Redigera uppgifter](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Redigera problem](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Du måste ha ytterligare åtkomst och behörigheter för att kunna redigera uppgifter och problem.

   * Öka antalet timmar som krävs för en roll som visar överallokeringen för initiativet. Mer information finns i [Skapa och redigera initiativ i  [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Du måste ha ytterligare åtkomst och behörigheter för att kunna redigera planer.

1. (Valfritt) Klicka på listruteikonen för att utöka en av månaderna på panelen [!UICONTROL Role Allocation] eller på tidslinjen i [!UICONTROL Workload Balancer].

   ![](assets/month-expanded-highlighted-role-allocation-panel-wb-350x145.png)

   Samma typ av information som visas i området [!UICONTROL Project Totals] visas också för varje månad.

   >[!TIP]
   >
   >Månaderna som visas på panelen [!UICONTROL Role Allocation] är de månader i tidslinjen som visas på skärmen i [!UICONTROL Workload Balancer]. Rulla bakåt och framåt på tidslinjen för att se ytterligare månader.

   <!--
   <li value="8" data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p> </p> </li>
   -->


