---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visa rolltilldelning för projekt och initiativ i Utjämning av arbetsbelastning
description: När du har kopplat projekt och initiativ kan du hantera deras resurstilldelning sida vid sida för att säkerställa att de
author: Alina
feature: Workfront Scenario Planner
exl-id: cdc3a1b0-7021-4853-9b51-c3682fd55430
source-git-commit: 9c0160dc5e43f36b65d9f2d4a3498a9c5f39f6f1
workflow-type: tm+mt
source-wordcount: '812'
ht-degree: 0%

---

# Visa rollallokering för projekt och initiativ i [!UICONTROL Workload Balancer]

>[!IMPORTANT]
>
>Din organisation måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] så att du kan visa initialinformation för ett projekt. Mer information om hur du hämtar [!DNL Workfront Scenario Planner] finns i [Åtkomst som behövs för att använda  [!DNL Scenario Planner]](../scenario-planner/access-needed-to-use-sp.md).

När du har kopplat projekt och initiativ kan du hantera deras resurstilldelning sida vid sida för att säkerställa att de matchar. På så sätt undviker du att överallokera eller underutnyttja dem.

I den här artikeln beskrivs hur du kan stämma av resurser med hjälp av panelen [!UICONTROL Role Allocation] i [!UICONTROL Workload Balancer] för ett projekt.

Allmän information om hur du förenar resurser mellan projekt och initiativ, inklusive förutsättningar, finns i [Översikt över att stämma av resursallokeringar mellan projekt och initiativ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Åtkomstkrav

Du måste göra följande:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> plan*</b> </p> </td> 
   <td>[!UICONTROL Business] eller högre</td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront]<b> licens*</b> </p> </td> 
   <td> <p>[!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td><b>Produkt</b> </td> 
   <td> <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till de funktioner som beskrivs i den här artikeln.</p> <p>Mer information om hur du hämtar [!DNL Workfront Scenario Planner] finns i <a href="../scenario-planner/access-needed-to-use-sp.md">Åtkomst som behövs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td><strong>Åtkomstnivåkonfigurationer*</strong> </td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till projekt </p> <p>Obs! Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p><strong>Objektbehörigheter</strong> </p> </td> 
   <td> <p>[!UICONTROL View] eller högre behörighet till projektet</p> <p>Mer information om hur du begär ytterligare åtkomst till en plan finns i <a href="../scenario-planner/request-access-to-plan.md">[!UICONTROL Request]-åtkomst till en plan i [!DNL Workfront Scenario Planner]</a>.</p> <p>Mer information om hur du begär ytterligare åtkomst till ett projekt finns i <a href="../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>. </p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront]-administratören om du vill ta reda på vilken plan, licenstyp eller åtkomst du har.

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


