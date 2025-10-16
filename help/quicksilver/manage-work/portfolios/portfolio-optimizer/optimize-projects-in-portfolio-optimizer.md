---
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
title: Optimera projekt i Portfolio Optimizer
description: Du kan använda [!UICONTROL Portfolio Optimizer] för att prioritera dina projekt baserat på deras resultat och andra värden. Optimeraren tar hänsyn till viktig projektinformation, som kostnad, justering, risk och avkastning, för att prioritera projekten efter vad som är viktigast för dig.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 25debc5b-5d7d-453f-ab0a-9bf3fba05693
source-git-commit: d7600a55b3dffb242957234de9d85a0deb1ad2e3
workflow-type: tm+mt
source-wordcount: '407'
ht-degree: 0%

---

# Optimera projekt i [!UICONTROL Portfolio Optimizer]

Du kan använda [!UICONTROL Portfolio Optimizer] för att prioritera dina projekt baserat på deras resultat och andra värden. [!UICONTROL Optimizer] tar hänsyn till viktig projektinformation, som kostnad, justering, risk och avkastning, för att prioritera projekten enligt vad som är viktigast för dig.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] package</td> 
   <td> <p>Workfront Prime eller senare</p>
      <p>Arbetsflöde Prime eller senare</p>
    </td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td> <p>[!UICONTROL Standard]</p>
   <p>[!UICONTROL Plan]</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>[!UICONTROL Edit] åtkomst till [!UICONTROL Portfolios] och [!UICONTROL Projects]</p>  </td>
</tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen</p>  </td> 
  </tr> 
 </tbody> 
</table>

*Mer information finns i [Åtkomstkrav för Workfront-dokumentation](/help/quicksilver/administration-and-setup/add-users/access-levels-and-object-permissions/access-level-requirements-in-documentation.md).

+++

<!--Old
<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> Any</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: [!UICONTROL Standard] </p>
   <p>Current: [!UICONTROL Plan] </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Optimera projekt i Portfolio Optimizer

1. Öppna en Portfolio och klicka sedan på **[!UICONTROL Portfolio Optimization]** i den vänstra panelen.

   [!UICONTROL Portfolio Optimizer] visas.

1. Klicka på ikonen **[!UICONTROL Optimize]** .

   ![Ikonen Optimera](assets/optimize-icon-portfolio-optimizer.png)

   Kategorierna som ett projekt kan poängsättas med visas till vänster om ikonen [!UICONTROL Optimize].

1. Använd skjutcirkeln för att ändra optimeringen av någon av följande kategorier:

   * **[!UICONTROL Low Cost]**: Flytta reglaget åt höger om du vill visa projekt med det lägsta [!UICONTROL Planned Cost].
   * **[!UICONTROL High Alignment]**: Flytta reglaget åt höger om du vill visa projekt med den högsta justeringen baserat på [!UICONTROL Scorecard].
   * **[!UICONTROL High Value]**: Flytta skjutreglaget åt höger om du vill visa projekt med ett högre [!UICONTROL Net Value] poäng.
   * **[!UICONTROL Low Risk to Benefit]**: Flytta reglaget åt höger om du vill visa projekt med lägst risk-till-nytta-förhållande.
   * **[!UICONTROL High ROI]**: Flytta reglaget åt höger om du vill visa projekt med högre avkastning på investeringen.

1. Klicka på ikonen **x** för att stänga optimeringskategorierna.

   Detta uppdaterar [!UICONTROL Score]-värdena för varje projekt i kolumnen **[!UICONTROL Score]**.

   Mer information om bakgrundsmusiken [!UICONTROL Portfolio Optimizer] finns i [Översikt över bakgrundsmusiken [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/portfolio-optimizer-score.md).

1. När rätt vikter har angetts för kolumnen **[!UICONTROL Score]** klickar du på rubriken för kolumnen **[!UICONTROL Score]** för att sortera efter den här kolumnen. Det projekt som har högst poäng visas högst upp i listan.

1. (Valfritt) Dra och släpp projekt i den ordning du prioriterar.
Detta ändrar ordningen för projekten i [!UICONTROL Portfolio Optimizer].
1. (Valfritt) Klicka på **[!UICONTROL Set Priority]** om du vill spara den nya prioriteten för projekten.

   >[!NOTE]
   >
   >   Du måste ha behörigheten Hantera för alla projekt i listan för att kunna använda **Ange projektprioritet**.

   Mer information om hur du prioriterar projekt i [!UICONTROL Portfolio Optimizer] finns i artikeln [Prioritera projekt i [!UICONTROL Portfolio Optimizer]](../../../manage-work/portfolios/portfolio-optimizer/prioritize-projects-in-portfolio-optimizer.md).

1. Klicka på **[!UICONTROL Save]** om du vill spara [!UICONTROL Portfolio Optimizer].
