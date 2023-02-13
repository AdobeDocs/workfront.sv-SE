---
title: Prioritera projekt i Portfolio-optimering
product-area: portfolios;projects
navigation-topic: portfolio-optimizer
description: Du kan prioritera dina projekt i Portfolio Optimizer för att fastställa i vilken ordning de ska slutföras.
author: Alina
feature: Work Management, Strategic Planning
exl-id: 54e33746-5995-49de-8e21-bf973f0694a6
source-git-commit: b6defd7dba91a06feb365ead74bd9c48f5165c77
workflow-type: tm+mt
source-wordcount: '490'
ht-degree: 0%

---

# Prioritera projekt i [!UICONTROL Portfolio Optimizer]

Du kan prioritera dina projekt i [!UICONTROL Portfolio Optimizer], för att fastställa i vilken ordning de ska fyllas i.

Tänk på följande när du använder [!UICONTROL Portfolio Optimizer]:

* Projekten högst upp i [!UICONTROL Portfolio Optimizer] anses viktigare än de som anges längst ned. Du måste slutföra projekten efter deras prioritet i [!UICONTROL Portfolio Optimizer] för att optimera Portfolio.
* Prioriteten för projekt i [!UICONTROL Portfolio Optimizer] är inte relaterat till [!UICONTROL Priority] fältet som finns på [!UICONTROL Project Details] -fliken i ett projekt.

   The [!UICONTROL Priority] på [!UICONTROL Project Details] -fliken är en visuell flagga som du anger manuellt för att förstå hur viktigt ett projekt ska vara.

* Prioriteten för projekt i optimeraren för Portfolio visas i dialogrutan [!DNL Resource Planner], om det är aktiverat där. I [!DNL Resource Planner], får projekten resurser i den ordning de är [!UICONTROL Resource Planner] och inte prioriteringen för [!UICONTROL Portfolio Priority].

   Mer information om hur du prioriterar projekt i [!UICONTROL Resource Planner], se artikeln [Prioritera projekt i [!UICONTROL Resource Planner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).

* The **[!UICONTROL Project Prioritization]** området på [!UICONTROL Portfolio Optimizer] visar projekt i den ordning [!UICONTROL Planned Start Dates] och [!UICONTROL Net Value], som standard.

## Åtkomstkrav

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan*</td> 
   <td> <p>Alla </p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Adobe Workfront-licenser*</td> 
   <td> <p>[!UICONTROL Business] eller högre</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå*</td> 
   <td> <p>[!UICONTROL Edit] behörighet till projekt och Portfolio</p> <p>Obs! Om du fortfarande inte har åtkomst kan du fråga [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
  <tr> 
   <td role="rowheader">Objektbehörigheter</td> 
   <td> <p>[!UICONTROL Manage] behörighet till portföljen</p> <p>Contribute eller högre behörigheter för projekten</p> <p>Mer information om hur du begär ytterligare åtkomst finns i <a href="../../../workfront-basics/grant-and-request-access-to-objects/request-access.md" class="MCXref xref">Begär åtkomst till objekt </a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

&#42;Kontakta [!DNL Workfront] administratör.

## Ändra prioritet för projekten i [!UICONTROL Portfolio Optimizer]

1. Klicka på **[!UICONTROL Main Menu]** icon ![](assets/main-menu-icon.png) i det övre högra hörnet av Adobe Workfront.

1. Klicka på **[!UICONTROL Portfolios]**.
1. (Valfritt) Välj rätt filter i dialogrutan **[!UICONTROL Filter]** för att visa rätt lista över portföljer.
1. Klicka på namnet på en portfölj för att öppna den.
1. Klicka **[!UICONTROL Portfolio Optimization]** i den vänstra panelen.
1. I [!UICONTROL project optization] ändrar du prioriteten för dina projekt genom att dra projekten i prioritetsordning och sedan släppa dem till önskad visningsposition.

   ![](assets/portfolio-optimizer-with-projects-nwe-350x89.png)

   Klicka **[!UICONTROL Set Priority]** i projektoptimeringsområdet när du är klar med att ordna om projekten. Projekten får ett nytt nummer baserat på den nya ordern.

1. Klicka **[!UICONTROL Save]** för att spara den nya projektprioriteten i [!UICONTROL Portfolio Optimizer]. Prioriteten anges som ett nummer i numret **#** kolumn.

   >[!TIP]
   >
   >Detta ändrar inte nödvändigtvis ordningen på projekten i [!UICONTROL Portfolio Optimizer], eftersom listan med projekt kan sorteras efter en annan kolumn än **#** kolumn. Klicka på **#** kolumnrubrik för att sortera listan efter projektprioritet.

   Du kan se projektets prioritet så som den visas i dialogrutan [!UICONTROL Portfolio Optimizer] i resursplaneraren genom att aktivera **[!UICONTROL Display Portfolio Priorities]** i resursplaneraren.

   Mer information om hur du prioriterar projekt i [!UICONTROL Resource Planner], se artikeln [Prioritera projekt i [!UICONTROL Resource Planner]](../../../resource-mgmt/resource-planning/prioritize-projects-resource-planner.md).
