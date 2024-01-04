---
user-type: administrator
product-area: system-administration
navigation-topic: configure-system-defaults
title: Skapa, redigera och dela standardfilter, vyer och grupperingar
description: Du kan skapa standardfilter, -vyer och -grupperingar och sedan göra dem tillgängliga för användare i organisationen.
author: Caroline
feature: System Setup and Administration
role: Admin
exl-id: 32eb825c-ba50-4820-a659-adc924a6ae52
source-git-commit: 548e713700fda79070f59f3dc3457410d2c50133
workflow-type: tm+mt
source-wordcount: '765'
ht-degree: 0%

---

# Skapa, redigera och dela standardfilter, vyer och grupperingar

<!--
<p data-mc-conditions="QuicksilverOrClassic.Draft mode">***DON'T DELETE, DRAFT OR HIDE THIS ARTICLE. IT IS LINKED TO THE PRODUCT, THROUGH THE CONTEXT SENSITIVE HELP LINKS. **</p>
-->

Du kan skapa standardfilter, -vyer och -grupperingar och sedan göra dem tillgängliga för användare i organisationen.

När du skapar standardfilter, vyer och grupperingar enligt beskrivningen i den här artikeln kan användare som du delar dem med utnyttja dem när de visar sina listor. Användare kan skapa egna filter, vyer och grupperingar baserat på de som du skapar, men de kan inte ändra direkt på dem som du skapar.

## Åtkomstkrav

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
   <td> <p>Du måste vara en [!DNL Workfront] administratör.</p> <p><b>ANMÄRKNING</b>: Om du fortfarande inte har åtkomst frågar du [!DNL Workfront] om de anger ytterligare begränsningar för din åtkomstnivå. För information om hur en [!DNL Workfront] kan administratören ändra din åtkomstnivå, se <a href="../../../administration-and-setup/add-users/configure-and-grant-access/create-modify-access-levels.md" class="MCXref xref">Skapa eller ändra anpassade åtkomstnivåer</a>.</p> </td> 
  </tr> 
 </tbody> 
</table>

## Skapa standardfilter, vyer eller grupperingar

{{step-1-to-setup}}

1. Gör något av följande, beroende på om du skapar eller redigerar ett filter, en vy eller en gruppering:

   * Klicka **[!UICONTROL Interface]** > **[!UICONTROL Filters]**.

   * Klicka **[!UICONTROL Interface]>** **[!UICONTROL Views]**.

   * Klicka **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**.

1. Om du skapar ett filter, en vy eller en gruppering klickar du på **[!UICONTROL Add Filter]**, **[!UICONTROL Add View]**, eller **[!UICONTROL Add Grouping]** markerar du sedan den objekttyp som du vill associera det nya filtret, den nya vyn eller grupperingen med.

   eller

   Om du redigerar ett befintligt filter, en befintlig vy eller en befintlig gruppering markerar du det och klickar sedan på knappen **[!UICONTROL Edit]** icon ![Ikonen Redigera](assets/edit-icon.png).

1. Konfigurera filter, vy eller gruppering.

   Mer information om tillgängliga alternativ finns i följande artiklar:

   * [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Översikt över vyer i [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Översikt över grupperingar i [!UICONTROL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)

1. Klicka **[!UICONTROL Save]** nära det nedre vänstra hörnet.

Du kan göra filtret, visningen eller grupperingen tillgänglig för användare i systemet. Mer information om hur du delar filter, vyer och grupper med andra användare finns i avsnittet [Göra filter, vyer och grupperingar tillgängliga för användarna](#make-filters-views-or-groupings-available-to-users) i den här artikeln.


## Visa eller dölj filter, vyer eller grupperingar som är tillgängliga från layoutmallen

Du kan välja att visa eller dölja filter, vyer eller grupperingar i layoutmallen. Synliga filter är tillgängliga för alla användare i hela systemet. Du kan använda en layoutmall för att dölja synliga filter för specifika användare eller grupper.

>[!NOTE]
>
>Om en användare aktivt använder ett filter, en vy eller en gruppering och sedan en administratör inaktiverar den, har användaren fortfarande åtkomst tills han eller hon väljer ett nytt filter, en ny vy eller en ny gruppering. När de har valt ett nytt filter, en ny vy eller en ny gruppering kan de inte längre återgå till det dolda filtret, den dolda vyn eller grupperingen.

Så här visar eller döljer du filter, vyer eller grupperingar som är tillgängliga från layoutmallen:

1. Klicka **[!UICONTROL Interface]** klickar du sedan på något av följande: **[!UICONTROL Filters]**, **[!UICONTROL Views]**, eller **[!UICONTROL Groupings]**.

1. (Villkorligt) Markera det filter, den vy eller den gruppering som du vill göra tillgänglig för användarna och klicka sedan på **[!UICONTROL Enable system-wide]**.

   ![](assets/enable-system-wide-fvg.png)

   >[!TIP]
   >
   >Om du vill att filtret, vyn eller grupperingen ska vara tillgänglig för de flesta användare, men dölja den för andra, kan du använda layoutmallen. Mer information finns i [Anpassa filter, vyer och grupperingar med en layoutmall](/help/quicksilver/administration-and-setup/customize-workfront/use-layout-templates/customize-fvg-list-controls-layout-template.md).

1. (Villkorligt) Markera det filter, den vy eller gruppering som du vill dölja för användarna och klicka sedan på **[!UICONTROL Disable system-wide]**. När det är inaktiverat döljs filtret, vyn eller grupperingen från layoutmallen samt användare i hela systemet.


## Göra filter, vyer och grupperingar tillgängliga för alla användare {#make-filters-views-or-groupings-available-to-users}

I de här stegen beskrivs hur du gör filter, vyer och grupperingar tillgängliga i [!UICONTROL Share] i dialogrutan [!UICONTROL Interface] område i [!UICONTROL Setup]. Den här inställningen fungerar som en på/av-switch för hela systemet, inklusive layoutmallen.

{{step-1-to-setup}}

1. Klicka **[!UICONTROL Interface]** klickar du sedan på något av följande: **[!UICONTROL Filters]**, **[!UICONTROL Views]**, eller **[!UICONTROL Groupings]**.

1. Markera det filter, den vy eller den gruppering som du vill göra tillgänglig för användarna och klicka sedan på **[!UICONTROL Share]** icon ![Delningsikon](assets/share-icon.png) för att öppna [!UICONTROL Filter Access], [!UICONTROL View Access], eller [!UICONTROL Grouping Access] formulär.
1. (Villkorligt) Om du vill göra filtret, vyn eller grupperingen tillgänglig för alla användare i systemet klickar du på **[!UICONTROL Gear]** nedrullningsbar meny ![](assets/gear-menu-for-sharing-items.png)och sedan klicka **[!UICONTROL Make this visible system-wide]**. Alla användare i systemet kan nu se filtret, vyn eller grupperingen.

   eller

   Börja skriva namnet på specifika användare, team, roller, grupper eller företag som filtret, vyn eller grupperingen ska delas med och klicka sedan på namnet i listrutan.

   Mer information om delning finns i [Översikt över delningsbehörigheter för objekt](../../../workfront-basics/grant-and-request-access-to-objects/sharing-permissions-on-objects-overview.md).

1. Klicka på **[!UICONTROL Save]**.

   Användare som du har angett kan nu se standardfiltret, vyn eller grupperingen när du visar den objekttyp som du har associerat den med.

## Ta bort filter, vyer och grupperingar

{{step-1-to-setup}}

1. Gör något av följande, beroende på om du tar bort ett filter, en vy eller en gruppering:

   * Klicka **[!UICONTROL Interface]** > **[!UICONTROL Filters]**

   * Klicka **[!UICONTROL Interface]** > **[!UICONTROL Views]**

   * Klicka **[!UICONTROL Interface]** > **[!UICONTROL Groupings]**

1. Markera ett eller flera objekt i listan och klicka sedan på **[!UICONTROL Delete]** icon ![Ikonen Ta bort](assets/delete.png).
1. I någon av följande artiklar finns detaljerad information om hur du konfigurerar ett filter, en vy eller en gruppering.

   * [Översikt över filter](../../../reports-and-dashboards/reports/reporting-elements/filters-overview.md)
   * [Översikt över vyer i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/views-overview.md)
   * [Översikt över grupperingar i [!DNL Adobe Workfront]](../../../reports-and-dashboards/reports/reporting-elements/groupings-overview.md)
