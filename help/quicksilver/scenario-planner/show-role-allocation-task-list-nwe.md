---
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Visa rolltilldelning för projekt och initiativ i uppgiftslistan
description: När du har kopplat projekt och initiativ kan du hantera deras resurstilldelning sida vid sida för att säkerställa att de matchar. På så sätt undviker du att överallokera eller underutnyttja dem.
author: Alina
feature: Workfront Scenario Planner
exl-id: 77152e46-0b7b-4937-9d16-1a20c2a7fdf1
source-git-commit: 2ff32ba11f9ef214f16b11323386223792b0877e
workflow-type: tm+mt
source-wordcount: '624'
ht-degree: 0%

---

# Visa rolltilldelning för projekt och initiativ i uppgiftslistan

<!--Audited: 07/2024-->

När du har kopplat projekt och initiativ kan du hantera deras resurstilldelning sida vid sida för att säkerställa att de matchar. På så sätt undviker du att överallokera eller underutnyttja dem.

I den här artikeln beskrivs hur du kan synkronisera resurser med hjälp av panelen [!UICONTROL Role Allocation] i uppgiftslistan för ett projekt.

Allmän information om hur du förenar resurser mellan projekt och initiativ, inklusive förutsättningar, finns i [Översikt över att stämma av resursallokeringar mellan projekt och initiativ](../scenario-planner/overview-reconcile-allocations-between-projects-initiatives.md).

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] plan*</p> </td> 
   <td> <p>Aktuell: [!UICONTROL Business] eller högre</p>
   <p>Nytt: Ultimate </p>
   </td> 
  </tr> 
  <tr> 
   <td> <p>[!DNL Adobe Workfront] licens*</p> </td> 
   <td> <p>Nytt: Ljus eller högre</p> 
   <p>Aktuell: [!UICONTROL Review] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td>Produkt* </td> 
   <td> 
   <p>För nuvarande Workfront-planer: </p>
   <p>Du måste köpa ytterligare en licens för [!DNL Adobe Workfront Scenario Planner] för att få tillgång till de funktioner som beskrivs i den här artikeln.</p> <p>Mer information om åtkomst och behörigheter för [!DNL Workfront Scenario Planner] finns i <a href="../scenario-planner/access-needed-to-use-sp.md" class="MCXref xref">Åtkomst som behövs för att använda [!DNL Scenario Planner]</a>. </p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td>Åtkomstnivå </td> 
   <td> <p>[!UICONTROL View] eller högre åtkomst till [!UICONTROL Projects]</p> </td> 
  </tr> 
  <tr data-mc-conditions=""> 
   <td> <p>Objektbehörigheter </p> </td> 
   <td> <p>[!UICONTROL View] behörigheter till ett projekt</p> </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Visa rolltilldelning för projekt och initiativ i uppgiftslistan

Om ditt företag har köpt en [!DNL Workfront Scenario Planner]-licens kan du stämma av resursallokeringarna mellan initiativet och det projekt som är länkat till det i projektavsnittet [!UICONTROL Tasks].

1. (Villkorligt) Anslut ett projekt till ett projekt med en av de metoder som beskrivs i [Visa rolltilldelning för projekt och initiativ i uppgiftslistan](#Connect) i den här artikeln.

   >[!IMPORTANT]
   >
   >Om ni ändrar resurser i initiativet måste ni på nytt publicera det scenario som initiativet hör till för att få den senaste resursinformationen från initiativet som ska uppdateras i projektet.

1. Gå till det projekt där du vill granska fördelningen av jobbroller för projektet samt för det associerade initiativet.
1. Klicka på **[!UICONTROL Tasks]** i den vänstra panelen.
1. Klicka på ikonen **[!UICONTROL Show role allocation]** ![](assets/show-role-allocation-icon.png) i det övre högra hörnet av verktygsfältet.

   Panelen [!UICONTROL Role Allocation] visas.

   <!--
   <p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: ensure this step stays 5 to match the mention of it in the section below)</p>
   -->

1. Granska följande information i området **[!UICONTROL Project Totals]** på panelen [!UICONTROL Role Allocation]:

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
   >   * När aktiviteter eller utgåvor har varaktigheten noll.
   >   
   >



1. (Valfritt) Om kolumnen [!UICONTROL Variance] visar att dina resurser är överallokerade justerar du något av följande:

   * Minska antalet planerade timmar för en jobbroll som visar överallokerade eller lägg till fler resurser för aktiviteterna och distribuera fler planerade timmar till de nya resurserna. Du kan uppdatera uppdrag eller antalet planerade timmar för uppgifter eller problem när du redigerar dem. Mer information finns i följande artiklar:

      * [Redigera uppgifter](../manage-work/tasks/manage-tasks/edit-tasks.md)
      * [Redigera problem](../manage-work/issues/manage-issues/edit-issues.md)

     >[!NOTE]
     >
     >Du måste ha ytterligare åtkomst och behörigheter för att kunna redigera uppgifter och problem.

   * Öka antalet timmar som krävs för rollen som visar överallokeringen för initiativet. Mer information finns i [Skapa och redigera initiativ i  [!DNL Adobe Workfront Scenario Planner]](create-and-edit-initiatives.md).

     >[!NOTE]
     >
     >Du måste ha ytterligare åtkomst och behörigheter för att kunna redigera planer.


