---
product-area: portfolios
navigation-topic: portfolios-overview
title: Navigera i en portfölj
description: Navigera i en portfölj
author: Alina
feature: Work Management, Strategic Planning
exl-id: 6c1795ab-422f-419c-b5e9-1f1323800b39
source-git-commit: b7387af018b1814c387ba3f0000fcdf7e0bf5067
workflow-type: tm+mt
source-wordcount: '555'
ht-degree: 0%

---

# Navigera i en portfölj

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">(NOTE: This article will need to be further revised and maybe merged into Understanding Portfolios?! (other?!).)</p>
-->

I [!DNL Adobe Workfront] representerar en portfölj en samling projekt som konkurrerar om samma resurser, budget, schema och prioritet. Det främsta syftet med portföljen är att hjälpa chefer och projektledare att välja att arbeta med projekt som ger mest nytta för en organisation.

Mer information om portföljer finns i [Översikt över Portfolio i [!DNL Adobe Workfront]](../../../manage-work/portfolios/portfolios-overview/portfolio-overview.md).

## Åtkomstkrav


+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens*</td> 
   <td> <p>Nytt: [!UICONTROL Standard] </p>
   <p>Aktuell: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] tillgång till projekt och portföljer</p>  </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen</p> <p>Visa eller högre behörigheter för projekten</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav i Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

## Navigera i en portfölj

1. Klicka på ikonen **[!UICONTROL Main Menu]** ![Huvudmeny](assets/main-menu-icon.png) i det övre högra hörnet av [!DNL Adobe Workfront].

1. Klicka på [!UICONTROL Portfolios].
1. Välj följande i listrutan **[!UICONTROL Filter]**:

   * **[!UICONTROL Portfolios I Own]**: Innehåller en lista över portföljer som du har utsetts till [!UICONTROL Portfolio Manager] för.
   * **[!UICONTROL All]**: Inkluderar alla portföljer som du har åtminstone åtkomst till Visa för.

     Mer information om åtkomst till portföljer finns i [Översikt över åtkomstnivåer](../../../administration-and-setup/add-users/access-levels-and-object-permissions/access-levels-overview.md).
Mer information om behörigheter till portföljer finns i [Dela en portfölj](../../../workfront-basics/grant-and-request-access-to-objects/share-a-portfolio.md).

     Mer information om hur du lägger till nya portföljer finns i [Skapa en portfölj](../../../manage-work/portfolios/create-and-manage-portfolios/create-portfolios.md).

1. Klicka på namnet på en portfölj för att komma åt den.
Följande portföljresultatmått visas i området [!UICONTROL Portfolio Details] i en portfölj:

   * Om portföljen är [!UICONTROL On Time]
   * Om portföljen är [!UICONTROL On Budget]
   * [!UICONTROL Return on Investment] (ROI)
   * Portföljen [!UICONTROL Alignment]
   * Portföljen [!UICONTROL Net Value]

1. (Valfritt)   Klicka på **[!UICONTROL Projects]** i den vänstra panelen för att visa projekt som är kopplade till den valda portföljen och välj sedan något av följande filter i listrutan **[!UICONTROL Filter]**:

   * **[!UICONTROL Active]**: Inkluderar alla projekt som är associerade med den valda portföljen och som har följande status:

      * [!UICONTROL Planning]
      * [!UICONTROL Approved]
      * [!UICONTROL Current]
   * **[!UICONTROL Requested]**: Inkluderar projekt som är associerade med den valda portföljen med statusen **[!UICONTROL Requested]**.

     Mer information om hur du granskar begärda projekt finns i [Granska begärda projekt](../../../manage-work/portfolios/create-and-manage-portfolios/review-requested-projects.md).

   * **[!UICONTROL All]**: Inkluderar alla projekt som är associerade med den valda portföljen.

     >[!NOTE]
     >
     >Om du bara vill visa specifika projekt kan du skapa ett projektfilter i listrutan **[!UICONTROL Filter]** högst upp i listan med projekt för att minska antalet projekt som visas.

     Mer information om hur du skapar filter finns i [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md).


1. Klicka på **[!UICONTROL Programs]** i den vänstra panelen för att skapa program i portföljen eller hantera befintliga program.
Mer information om program finns i avsnittet [Skapa och hantera program](../../../manage-work/portfolios/create-and-manage-programs/create-and-manage-programs.md).

1. (Valfritt) Expandera området **[!UICONTROL Portfolio Details]** i den vänstra panelen och klicka sedan på **[!UICONTROL Overview]** eller **[!UICONTROL Custom Forms]** för att redigera information om portföljen.

1. (Valfritt) Klicka på **[!UICONTROL Portfolio Optimization]** i den vänstra panelen för att optimera portföljens prestanda.

   ![Portfolio-optimering med projekt](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   >[!IMPORTANT]
   >
   >Ditt företag måste ha en [!UICONTROL Business]-plan eller en senare [!DNL Workfront]-plan för att få tillgång till [!UICONTROL Portfolio Optimizer].

   Mer information om hur du använder Portfolio Optimizer finns i avsnittet [Hantera projekt i Portfolio Optimizer](../../../manage-work/portfolios/portfolio-optimizer/manage-projects-in-portfolio-optimizer.md).

1. (Valfritt) Klicka på **Dokument** i den vänstra panelen för att bifoga dokument till portföljen.
1. (Valfritt) Klicka på **[!UICONTROL Updates]** i den vänstra panelen för att lägga till kommentarer i portföljens uppdateringsström. Mer information finns i [Uppdatera arbete](../../../workfront-basics/updating-work-items-and-viewing-updates/update-work.md).
1. (Valfritt) Klicka på **[!UICONTROL More]-menyn** ![Mer-menyn](assets/qs-more-icon-on-an-object.png) om du vill göra något av följande:

   * Inaktivera portföljen. När en portfölj inaktiveras kan du inte längre koppla den till projekt på projektnivå.
   * Ta bort portföljen.

     >[!IMPORTANT]
     >
     >Detta tar inte bort projekt som är kopplade till portföljen. Detta tar bort namnet på portföljen från de projekt som är kopplade till den.

   * Dela portföljen med andra användare.

1. (Valfritt) Klicka på ikonen **Stjärna** ![Stjärna &#x200B;](assets/qs-star-icon-favorites-39x38.png) till höger om portföljnamnet för att lägga till portföljen i din favoritlista.
