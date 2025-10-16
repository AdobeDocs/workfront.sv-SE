---
content-type: reference
product-area: enterprise-scenario-planner-product-area
navigation-topic: enterprise-scenario-planner-navigation-topic
title: Åtkomst krävs för att använda scenarioplaneraren
description: Scenarioplaneraren kräver en separat licens från Adobe Workfront och ytterligare åtkomst.
author: Alina
feature: Workfront Scenario Planner
exl-id: d7f3c7fa-81aa-40c9-b506-fe1fe346e9ea
source-git-commit: 1b06589a705cf218239ff1273b865c05e4ceb96f
workflow-type: tm+mt
source-wordcount: '387'
ht-degree: 0%

---

# Åtkomst krävs för att använda [!DNL Scenario Planner]

<!--Audited: 04/2024-->

<!--The [!DNL Scenario Planner] has additional license requirements. For information about the [!DNL Workfront Scenario Planner], see [The [!DNL Scenario Planner] overview](../scenario-planner/scenario-planner-overview.md).-->

<!--
might need to add information about the permissions to plans/ initiatives if those will be coming later?
-->

Utan rätt åtkomst eller behörigheter kanske du inte kan visa [!UICONTROL Scenarios]-området för [!DNL &#x200B; Adobe Workfront] eller hantera planer eller initiativ för din organisation. I hanteringen av planer och initiativ ingår att skapa, redigera och ta bort dem.

## Åtkomst krävs för att visa och använda [!DNL Adobe Workfront Scenario Planner]

Du måste se till att alla följande villkor uppfylls innan du kan komma åt [!DNL Workfront Scenario Planner]:

1. Organisationen måste ha ett Workfront Ultimate-paket.

   Scenarioplaneraren är inte tillgänglig för Workfront Workflow-paket.

   Tala med din kontoansvarige på Workfront om du förnyar Workfront och du vill behålla scenarioplanen.

   Om du är ny kund är Scenarioplaneraren inte längre tillgänglig att köpa.

   <!--Old: 
    Depending on whether you use the new or the current Workfront plan, your organization must have one of the following:
    * For the new plans, your organization must have the  [!UICONTROL Ultimate] [!DNL Workfront] plan. The Scenario Planner is included only in the [!UICONTROL Ultimate] plan. 
    * For the current Workfront plans, your organization must have both of the following: 
      * Your organization must purchase a [!DNL Workfront] [!UICONTROL Business] or higher [!DNL Workfront] plan. 
      
      * Your organization must purchase a [!DNL Workfront Scenario Planner] license, in addition to a [!DNL Workfront] license. Contact your [!DNL Workfront] Account Representative to learn about [!DNL Workfront Scenario Planner] licenses. -->

1. Du måste ha någon av följande Workfront-licenser:

   * [!UICONTROL Light] eller senare
   * [!UICONTROL Reviewer] eller senare

   <!--Old: 
      * For the current licenses: 
        * [!UICONTROL Plan]
        * [!UICONTROL Work]
        * [!UICONTROL Review]-->
   <!--Old: 
      >[!NOTE]
      > 
      >* When using the new licenses, users with a [!UICONTROL Contributor] or [!UICONTROL External] license type cannot access the [!DNL Scenario Planner].
      >
      >* When using the current licenses, users with a Request or External license type cannot access the Scenario Planner. -->

1. Din [!DNL Workfront]-administratör måste ge dig [!UICONTROL View] eller [!UICONTROL Edit] åtkomst till [!DNL Scenario Planner] på din åtkomstnivå.

   Mer information om att bevilja åtkomst till [!DNL Workfront Scenario Planner] finns i [Bevilja åtkomst till [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

1. (Valfritt och rekommenderas) Om du vill visa eller uppdatera ekonomisk information för dina planer och initiativ måste [!DNL Workfront]-administratören även ge dig åtkomst till [!UICONTROL Financial Data] på din åtkomstnivå. Mer information om att bevilja ekonomiska data på din åtkomstnivå finns i [Bevilja åtkomst till ekonomiska data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).


<!--1. (Optional) If you need to access plans you didn't create, a plan creator must give you the correct permissions to their plan to access it. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.-->

<!--this used to be true but not anymore:
  <li data-mc-conditions="QuicksilverOrClassic.Draft mode"> <p>(NOTE: this is no longer needed) </p> <p>Your Workfront administrator must assign you a layout template that includes the Scenarios area in the Main Menu. </p> <p>For information about customizing the Main Menu in a layout template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/customize-main-menu.md" class="MCXref xref" xrefformat="{para}">Customize the Main Menu using a layout template</a>. </p> <p>For information about assigning users to a Layout Template, see <a href="../administration-and-setup/customize-workfront/use-layout-templates/assign-users-to-layout-template.md" class="MCXref xref" xrefformat="{para}">Assign users to a layout template</a>.</p> </li>
  -->

<!--Repetitive from above?? 

## Access needed to view plans and initiatives

In addition to your company acquiring the correct license for the [!DNL Workfront Scenario Planner], your [!DNL Workfront] administrator must also assign you the following access and setup so you can view the [!DNL Workfront Scenario Planner] and the information in this area:

* An access level with at least [!UICONTROL View] access to [!DNL Scenario Planner].

  For information about the access level to [!DNL Scenario Planner], see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* An access level with at least [!UICONTROL View] access to [!UICONTROL Financial Data] if you need to also view financial information about the plan and the initiatives. Some examples of financial information are budgets, costs, or job role rates.

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

  >[!TIP]
  >
  >[!UICONTROL Requestors] and [!UICONTROL External] Users do not have access to view the [!DNL Scenario Planner].

* View permissions to the plan. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

## Access needed to manage plans and initiatives

Your [!DNL Workfront] administrator must assign you the following access so you can manage plans and their information in the [!DNL Scenario Planner]:

* A [!UICONTROL Plan] or [!UICONTROL Work] license type with Edit access to the [!DNL Scenario Planner] in your access level.

  All other license types do not have access to manage plans.

  For information about granting access to [!DNL Scenario Planner] from the Access Level, see [Grant access to [!DNL Scenario Planner]](../administration-and-setup/add-users/configure-and-grant-access/grant-access-sp.md).

* A [!UICONTROL Plan] license type with [!UICONTROL Edit] access to [!UICONTROL Financial Data] in your access level, if you need to also update financial information about the plan.

  Some examples of financial information that you can edit are [!UICONTROL Budget], [!UICONTROL Planned Benefit], and [!UICONTROL Fixed Costs].

  >[!TIP]
  >
  >Only [!UICONTROL Plan] license holders have [!UICONTROL Edit] access to [!UICONTROL Financial Data].

  For information about the [!UICONTROL Financial Data] access level, see [Grant access to financial data](../administration-and-setup/add-users/configure-and-grant-access/grant-access-financial.md).

* Manage permissions to a plan that you didn't create. For information about the permissions needed to access plans and initiatives that you didn't create, see the [Permissions needed to access plans and initiatives](#permissions-needed-to-access-plans-and-initiatives) section in this article.

-->

## Behörigheter som krävs för att få tillgång till planer och initiativ

Åtkomstnivåer fungerar tillsammans med behörigheter i [!DNL Workfront] för att ge dig insyn i planer och initiativ som du inte har skapat. Förutom att du måste ha rätt åtkomstnivå för att få åtkomst till [!DNL Scenario Planner] måste du också ha rätt behörigheter till de planer som du vill visa eller hantera, om du inte är den som har skapat dessa planer.

Alla användare, inklusive systemadministratörer, har endast åtkomst till planer som de har skapat.

Om du vill visa planer som andra användare har skapat måste de dela sina planer med dig på följande sätt:

* Dela planen med dig

  Mer information om delningsplaner finns i [Dela en plan i  [!DNL Scenario Planner]](../scenario-planner/share-a-plan.md).

* Skicka en länk till en plan som de har skapat

  Om en användare delar en länk till en plan utan att också dela planen, kan du begära behörigheter till planen. Mer information om hur du begär behörigheter till planer finns i [Begär åtkomst till en plan i  [!DNL Scenario Planner]](../scenario-planner/request-access-to-plan.md).

>[!NOTE]
>
>När en användare inaktiveras har deras planer ingen ägare och går inte att komma åt om de inte tidigare delats med en länk.


