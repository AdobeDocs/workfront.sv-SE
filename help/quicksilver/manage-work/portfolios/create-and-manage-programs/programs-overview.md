---
content-type: overview
product-area: portfolios
navigation-topic: create and manage programs
title: Programöversikt
description: Ett program är en samling projekt som har enhetliga egenskaper. Dessa projekt konkurrerar vanligtvis om samma resurser, budget eller tidskortplats. Programmen är en undergrupp av portföljer. Du kan associera projekt med program innan de läggs till i en portfölj.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 1c64fe00-12e3-49f6-b864-b8f89ed9140d
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '483'
ht-degree: 0%

---

# Programöversikt

<!-- Audited: 08/2025 -->

I Adobe Workfront är ett program en samling projekt som har enhetliga egenskaper. De kan till exempel konkurrera om samma budget, resurser eller tidsram. Programmen är en undergrupp av portföljer.

Den här artikeln innehåller allmän information om program i Workfront.


## Åtkomst krävs för att skapa program

<!--leave the table uncollapsed as this article is about access-->

Du måste ha följande åtkomst för att skapa och hantera portföljer:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Alla</p>
   <p>[!UICONTROL Business] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!UICONTROL Portfolios] och [!UICONTROL Programs]</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>Hantera behörigheter för att redigera ett program eller lägga till projekt i det</p>
   <p>Hantera behörigheter för den portfölj som programmet tillhör </p>
   <p>Visa behörigheter till ett program för att visa det</p>
   <p>När du har skapat ett program har du som standard behörigheten Hantera</p> 
    </td> 
  </tr> 
 </tbody> 
</table>

Mer information finns i [Åtkomstkrav i Workfront-dokumentationen](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

<!--Old:
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>New: Any</p>
   <p>Current: [!UICONTROL Business] or higher</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] license</td> 
   <td> <p>New: [!UICONTROL Standard]</p>
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations</td> 
   <td> <p>[!UICONTROL Edit] access to Portfolios and Programs</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>Manage permissions to edit a program or add projects to it</p>
   <p>Manage permissions to the portfolio that the program belongs to </p>
   <p>View permissions to a program to view it</p>
   <p>After you create a program, you have Manage permissions to it, by default</p> 
    </td> 
  </tr> 
 </tbody> 
</table>-->


## Att tänka på när du arbetar med program

* Du kan använda både portföljer och program för att ordna projekt. Genom att organisera projekt kan du jämföra liknande projekt och avgöra var resurser ska användas bäst.

* Programmen är en undergrupp av portföljer. Om en portfölj innehåller för många projekt kan du dela upp den i flera program och ordna projekten först efter program och sedan efter portfölj.

  Du kan till exempel ha en Marketing 2024-portfolio som är uppdelad i fyra kvartalsprogram.

* Projekt som tillhör samma program konkurrerar vanligtvis om samma resurser, budget eller tidsrymd.

* Du måste först skapa en portfölj och sedan kan du skapa flera program i samma portfölj.

  Mer information om hur du använder program finns i [Skapa ett program](../../../manage-work/portfolios/create-and-manage-programs/create-program.md).

* Du måste först skapa en portfölj, sedan ett program, innan du kan koppla ett projekt till ett program och en portfölj.

* När du skapar projekt, program och portfolior bör du tänka på följande:

   * Ett projekt kan vara oberoende utan att vara kopplat till ett program eller en portfölj.
   * Ett projekt kan associeras med en portfölj, men behöver inte associeras med ett program.
   * Ett program måste alltid associeras med en portfölj. Den kan aldrig finnas utanför en portfölj.
   * Ett projekt som är associerat med ett program är alltid associerat med programmets portfölj.
   * Ett program kan bara associeras med en portfölj.
   * Ett projekt kan bara associeras med ett program och programmets portfölj i taget.
   * En portfölj kan ha flera program och projekt.
   * Ett program kan ha flera projekt.

  Mer information om hur du skapar projekt och portföljer finns i följande artiklar:
   * [Skapa ett projekt](/help/quicksilver/manage-work/projects/create-projects/create-project.md)
   * [Skapa en portfölj](/help/quicksilver/manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md)


* Du kan använda portföljoptimeraren för att analysera prestanda för alla projekt i en portfölj. Du kan inte jämföra prestanda för flera projekt i ett och samma program. Du måste analysera projektresultaten på portföljnivå.

  Mer information finns i [Optimera projekt i Portfolio Optimizer](/help/quicksilver/manage-work/portfolios/portfolio-optimizer/optimize-projects-in-portfolio-optimizer.md).
