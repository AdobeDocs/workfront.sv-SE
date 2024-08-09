---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa, redigera och dela standardfilter, vyer och grupperingar
description: Du kan skapa standardfilter, -vyer och -grupperingar och sedan göra dem tillgängliga för användare i organisationen.
author: Lisa
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: f036fbfc203f942fa5a22070860c3a20035a183b
workflow-type: tm+mt
source-wordcount: '776'
ht-degree: 0%

---

# Skapa, redigera och dela standardfilter, vyer och grupperingar

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Du kan skapa standardfilter, -vyer och -grupperingar och sedan göra dem tillgängliga för användare i organisationen.

När du skapar standardfilter, vyer och grupperingar enligt beskrivningen i den här artikeln kan användare som du delar dem med utnyttja dem när de visar sina listor. Användare kan skapa egna filter, vyer och grupperingar baserat på de som du skapar, men de kan inte ändra direkt på dem som du skapar.

## Åtkomstkrav

+++ Expandera om du vill visa åtkomstkrav för funktionerna i den här artikeln.

Du måste ha följande åtkomst för att kunna utföra stegen i den här artikeln:

<table style="table-layout:auto"> 
 <col> 
 <col> 
 <tbody> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] plan</td> 
   <td>Alla</td> 
  </tr> 
  <tr> 
   <td role="rowheader">[!DNL Adobe Workfront] licens</td> 
   <td>[!UICONTROL Plan]</td> 
  </tr> 
  <tr> 
   <td role="rowheader">Konfigurationer på åtkomstnivå</td> 
   <td> <p>Du måste vara en [!DNL Workfront]-administratör.</p> <p><b>Obs!</b> Om du fortfarande inte har åtkomst frågar du [!DNL Workfront]-administratören om de anger ytterligare begränsningar för din åtkomstnivå. Mer information om hur en [!DNL Workfront]-administratör kan ändra din åtkomstnivå finns i <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

+++

## Skapa standardfilter, vyer eller grupperingar

{{step-1-to-setup}}

1. Gör något av följande, beroende på om du skapar eller redigerar ett filter, en vy eller en gruppering:

   * Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Filters]**.

   * Klicka på **[!UICONTROL Interface]>** **[!UICONTROL Views]**.

   * Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**.

1. Om du skapar ett filter, en vy eller en gruppering klickar du på **[!UICONTROL Add Filter]**, **[!UICONTROL Add View]** eller **[!UICONTROL Add Grouping]** och väljer sedan den objekttyp som du vill associera det nya filtret, den nya vyn eller grupperingen med.

   eller

   Om du redigerar ett befintligt filter, en befintlig vy eller en befintlig gruppering markerar du det och klickar sedan på ikonen **[!UICONTROL Edit]** ![Redigera ](assets/edit-icon.png) .

1. Konfigurera filter, vy eller gruppering.

   Mer information om tillgängliga alternativ finns i följande artiklar:

   * [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Vyöversikt i [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Översikt över grupperingar i [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Klicka på **[!UICONTROL Save]** nära det nedre vänstra hörnet.

Du kan göra filtret, visningen eller grupperingen tillgänglig för användare i systemet. Mer information om att dela filter, vyer och grupperingar med andra användare finns i avsnittet [Gör filter, vyer och grupperingar tillgängliga för användare](#make-filters-views-or-groupings-available-to-users) i den här artikeln.


## Visa eller dölj filter, vyer eller grupperingar som är tillgängliga från layoutmallen

Du kan välja att visa eller dölja filter, vyer eller grupperingar i layoutmallen. Synliga filter är tillgängliga för alla användare i hela systemet. Du kan använda en layoutmall för att dölja synliga filter för specifika användare eller grupper.

>[!NOTE]
>
>Om en användare aktivt använder ett filter, en vy eller en gruppering och sedan en administratör inaktiverar den, har användaren fortfarande åtkomst tills han eller hon väljer ett nytt filter, en ny vy eller en ny gruppering. När de har valt ett nytt filter, en ny vy eller en ny gruppering kan de inte längre återgå till det dolda filtret, den dolda vyn eller grupperingen.

Så här visar eller döljer du filter, vyer eller grupperingar som är tillgängliga från layoutmallen:

1. Klicka på **[!UICONTROL Interface]** och sedan på något av följande: **[!UICONTROL Filters]**, **[!UICONTROL Views]** eller **[!UICONTROL Groupings]**.

1. (Villkorligt) Markera det filter, den vy eller den gruppering som du vill göra tillgänglig för användarna och klicka sedan på **[!UICONTROL Enable system-wide]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Om du vill att filtret, vyn eller grupperingen ska vara tillgänglig för de flesta användare, men dölja den för andra, kan du använda layoutmallen. Mer information finns i [Anpassa filter, vyer och grupperingar med hjälp av en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Villkorligt) Markera det filter, den vy eller den gruppering som du vill dölja för användarna och klicka sedan på **[!UICONTROL Disable system-wide]**. När det är inaktiverat döljs filtret, vyn eller grupperingen från layoutmallen samt användare i hela systemet.


## Göra filter, vyer och grupperingar tillgängliga för alla användare {#make-filters-views-or-groupings-available-to-users}

I de här stegen beskrivs hur du gör filter, vyer och grupperingar tillgängliga i dialogrutan [!UICONTROL Share] i området [!UICONTROL Interface] i [!UICONTROL Setup]. Den här inställningen fungerar som en på/av-switch för hela systemet, inklusive layoutmallen.

{{step-1-to-setup}}

1. Klicka på **[!UICONTROL Interface]** och sedan på något av följande: **[!UICONTROL Filters]**, **[!UICONTROL Views]** eller **[!UICONTROL Groupings]**.

1. Markera det filter, den vy eller den gruppering som du vill göra tillgänglig för användarna och klicka sedan på ikonen **[!UICONTROL Share]** ![Dela ](assets/share-icon.png) för att öppna formuläret [!UICONTROL Filter Access], [!UICONTROL View Access] eller [!UICONTROL Grouping Access].
1. (Villkorligt) Om du vill göra filtret, vyn eller grupperingen tillgänglig för alla användare i systemet klickar du på den nedrullningsbara menyn **[!UICONTROL Gear]** ![](assets/gear-menu-for-sharing-items.png) och sedan på **[!UICONTROL Make this visible system-wide]**. Alla användare i systemet kan nu se filtret, vyn eller grupperingen.

   eller

   Börja skriva namnet på specifika användare, team, roller, grupper eller företag som filtret, vyn eller grupperingen ska delas med och klicka sedan på namnet i listrutan.

   Mer information om delning finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicka på **[!UICONTROL Save]**.

   Användare som du har angett kan nu se standardfiltret, vyn eller grupperingen när du visar den objekttyp som du har associerat den med.

## Ta bort filter, vyer och grupperingar

{{step-1-to-setup}}

1. Gör något av följande, beroende på om du tar bort ett filter, en vy eller en gruppering:

   * Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Filters]**

   * Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Views]**

   * Klicka på **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**

1. Markera ett eller flera objekt i listan och klicka sedan på ikonen **[!UICONTROL Delete]** ![Ta bort](assets/delete.png) .
1. I någon av följande artiklar finns detaljerad information om hur du konfigurerar ett filter, en vy eller en gruppering.

   * [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Översikt över vyer i  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Översikt över grupperingar i  [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
