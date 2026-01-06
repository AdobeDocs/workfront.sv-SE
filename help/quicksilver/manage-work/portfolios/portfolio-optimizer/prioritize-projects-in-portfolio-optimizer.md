---
title: Prioritera projekt i Portfolio Optimizer
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Du kan prioritera dina projekt i Portfolio Optimizer för att fastställa i vilken ordning de ska slutföras.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: 714e6e09f1429f0382c36d17d3f2aca95edcfbc6
workflow-type: tm+mt
source-wordcount: '421'
ht-degree: 0%

---

# Prioritera projekt i [!UICONTROL Portfolio Optimizer]

Du kan prioritera dina projekt i [!UICONTROL Portfolio Optimizer] för att fastställa i vilken ordning de ska slutföras.

Tänk på följande när du använder [!UICONTROL Portfolio Optimizer]:

* Projekten högst upp i [!UICONTROL Portfolio Optimizer] anses viktigare än de som listas längst ned. Du måste slutföra projekten i prioritetsordning i [!UICONTROL Portfolio Optimizer] för att Portfolio ska kunna optimeras.
* Prioriteten för projekt i [!UICONTROL Portfolio Optimizer] är inte relaterad till fältet [!UICONTROL Priority] på fliken [!UICONTROL Project Details] i ett projekt.

  Fältet [!UICONTROL Priority] på fliken [!UICONTROL Project Details] är en visuell flagga som du anger manuellt för att förstå hur viktigt ett projekt ska vara.

* Prioriteten för projekt i Portfolio Optimizer visas i [!DNL Resource Planner], om den är aktiverad där. I [!DNL Resource Planner] får projekt resurser i den ordning de har [!UICONTROL Resource Planner] och inte i den ordning de har [!UICONTROL Portfolio Priority].

  Mer information om hur du prioriterar projekt i [!UICONTROL Resource Planner] finns i artikeln [Prioritera projekt i [!UICONTROL Resource Planner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* Under **[!UICONTROL Project Prioritization]** i [!UICONTROL Portfolio Optimizer] visas projekt i ordningen [!UICONTROL Planned Start Dates] och [!UICONTROL Net Value] som standard.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln. 

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

<!--Old:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td> <p>Any </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront licenses*</td> 
   <td> <p>New: Standard</p>
   <p>Current: Plan</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Access level configurations*</td> 
   <td> <p>[!UICONTROL Edit] access to Projects and Portfolios</p></td> 
  </tr> 
  <tr> 
   <td role="rowheader">Object permissions</td> 
   <td> <p>[!UICONTROL Manage] permissions to the portfolio</p> <p>Contribute or higher permissions to the projects</p> 
   <p>You must have Manage permissions to all the projects in the list to be able to use <b>Set project priority</b>.</p>
    </td> 
  </tr> 
 </tbody> 
</table>-->

## Ändra prioritet för projekten i [!UICONTROL Portfolio Optimizer]

{{step1-to-portfolios}}

1. (Valfritt) Välj rätt filter i listrutan **[!UICONTROL Filter]** för att visa rätt lista över portföljer.
1. Klicka på namnet på en portfölj för att öppna den.
1. Klicka på **[!UICONTROL Portfolio Optimization]** i den vänstra panelen.
1. I området [!UICONTROL project optization] ändrar du prioriteten för dina projekt genom att dra projekten i prioritetsordning och sedan släppa till önskad visningsposition.

   ![Portfolio-optimering med projekt](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Klicka på **[!UICONTROL Set Priority]** i projektoptimeringsområdet när du är klar med att ordna om dina projekt. Projekten får ett nytt nummer baserat på den nya ordern.

1. Klicka på **[!UICONTROL Save]** om du vill spara den nya projektprioriteten i [!UICONTROL Portfolio Optimizer]. Prioriteten listas som ett tal i kolumnen **#**.

   >[!TIP]
   >
   >Detta ändrar inte nödvändigtvis ordningen på projekten i [!UICONTROL Portfolio Optimizer], eftersom listan med projekt kan sorteras efter en annan kolumn än kolumnen **#**. Klicka på kolumnrubriken **#** för att sortera listan efter projektprioritet.

   Du kan se projektets prioritet så som den visas i [!UICONTROL Portfolio Optimizer] i resursplaneraren genom att aktivera inställningen **[!UICONTROL Display Portfolio Priorities]** i resursplaneraren.

   Mer information om hur du prioriterar projekt i [!UICONTROL Resource Planner] finns i artikeln [Prioritera projekt i [!UICONTROL Resource Planner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
